VScode����CMD�������л���(2.0)
[�ٷ�Task.json˵��](https://code.visualstudio.com/docs/editor/tasks)
[������Task.json������Ϣ](https://code.visualstudio.com/docs/editor/tasks-appendix)
[Task.jsonԤ�������](https://code.visualstudio.com/docs/editor/variables-reference)
    ���˺ܶ����ϵĽ̶̳�˵��Ҫ����VScode��python�����Ȼ����ֻ��������һ����ʹ�������ն�����������о���һ��ʱ�䷢����ʵ��������cmd���е�����ֱ������һ��task.json���ɣ���pythonΪ������
    ��û�б��뻷����.py�ļ��а���CTRL + SHIFT + B,�ͻ��ڹ����ռ����һ��.vscode�ļ��У������б����й����ռ䣨�����ļ��е������ռ䣩�����û�е���һ���ļ��м��ɡ�����.vscode�м�����task.json�ļ��������������á�
    

```
{
    // See https://go.microsoft.com/fwlink/?LinkId=733558
    // for the documentation about the tasks.json format
    "version": "2.0.0",
    "tasks": [
        {
            "label": "Python",
            "type": "shell",
            "command": "python",
            "args": [
                "${fileBasename}"
            ],
            "presentation": {
                "reveal": "always",
                "panel": "shared"
            },
            "options": {
                "cwd": "${fileDirname}"
            },
            "group": {
                "kind": "build",
                "isDefault": true
            },
            "problemMatcher": ["$tsc"]
        }
    ]
}
```
   �ȹ���һ����Ӿ������û�� "cwd": "${fileDirname}" �ͻ��ڹ����ռ�Ŀ¼��ִ�У���������ʶ����֤��ʹ�����·�������Ҳ���������������֤�롣������Ҫ������Ŀ¼ָ�����ļ�����Ŀ¼��Ȼ����൱��ִ�� python xxx.py��
   ������������CMD�������е����������ô���ã�����C++��php��   ������������CMD�������е����������ô���ã�����C++��php��