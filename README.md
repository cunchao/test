自动化测试管理系统
var exec = require('child_process').exec;

//需要执行的命令字符串
var cli = 'ipconfig';

exec(cli,{encoding:'utf8'},function (err,stdout,stderr){
    if (err){
        console.log(err);
        return;
    }
    console.log('stdout'+stdout);
    console.log('stderr'+stderr);
})
