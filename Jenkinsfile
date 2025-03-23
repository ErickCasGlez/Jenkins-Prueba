pipeline{
    agent any

    parameters{
        string(defaultValue: "Nombre", description: "Which environment to deploy in?", name: "deployEnv")
        choice(choices:["EU-WEST-2A", "EU-WEST-2B", "EU-WEST-2C"], description: "Which environment to deploy in?", name: "deployZone")
        booleanParam(defaultValue: false, description: "Confirm?", name: "confirm")
    }

    stages{
        stage ("Completa la info") {
            steps {
                echo "Nombre: ${deployEnv} \n"
                echo "Zona: ${deployZone}\n"
                echo "Confirma? ${confirm}"
            }
        }
    }
}
