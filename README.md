# goproject_step

//go module use by go 1.13
//step:1:cd project dir
//step:2:execute:$env:GOPROXY=“https://goproxy.io” 解决下载包问题
//step3:go mod init projectname general go.mod
//step4:general exe icon
    1.prepare main.icon,main.rc 
      main.rc content: IDI_ICON1 ICON "main.ico"
    2 execute :windres -o main.syso main.rc
//step5:go build --window or go build -ldflags="-H windowsgui -s" --no window
