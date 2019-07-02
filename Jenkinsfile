library 'BanzaiCICD@master'

banzai([
    gitOps:[
        envs: [
            'dev' : [:],
            'qa' : [
                approverIds: ['<jenkins-id>']
            ]
        ],
        autoDeploy: [
            /develop/ : 'dev'
        ]
    ]
])
