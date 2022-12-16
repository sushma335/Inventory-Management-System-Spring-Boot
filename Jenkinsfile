node('') {
	stage ('checkout code'){
		git credentialsId: '5dd9c649-3a74-48ce-b82c-926e0e0bb79d', url: 'https://github.com/sushma335/Inventory-Management-System-Spring-Boot'
	}
	
	stage ('Build'){
		sh "mvn clean install -Dmaven.test.skip=true"
	}

	stage ('Test Cases Execution'){
		sh "mvn clean org.jacoco:jacoco-maven-plugin:prepare-agent install -Pcoverage-per-test"
	}
}
Footer
© 2022 GitHu
