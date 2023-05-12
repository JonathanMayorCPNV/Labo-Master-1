# Fork process

[Source](https://docs.github.com/en/get-started/quickstart/fork-a-repo)

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption><p>Git-flow scenario to master</p></figcaption></figure>

* [ ] Fork the "upstream" repository in your github organisation

```
![image](https://github.com/JonathanMayorCPNV/Labo-Master-1/assets/115776017/8d9f7f97-34f5-40bf-bbef-5d38591aa8f1)
```

* [ ] Clone your own repo in your local machine

```
![image](https://github.com/JonathanMayorCPNV/Labo-Master-1/assets/115776017/ca6d0153-a0da-41f4-9df7-16035e2f79d0)
```

* [ ] Init Git flow (with standard settings)

```
![image](https://github.com/JonathanMayorCPNV/Labo-Master-1/assets/115776017/cc9570f5-8930-4971-aba8-3f2ea0420a3d)
```

* [ ] Integrate updates from upstream (main) into your repository (develop)

```
![image](https://github.com/JonathanMayorCPNV/Labo-Master-1/assets/115776017/1317b7bc-a29e-4d4f-b131-3ff6900b5b25)
```

* [ ] Create a branch feature called "terraformBasicScript"

```
![image](https://github.com/JonathanMayorCPNV/Labo-Master-1/assets/115776017/1f73d6ae-770c-4c5a-ae57-f8193fbd2ed6)
```

* [ ] Add this code and commit it (feat:add basic terraform script")

```
terraform {
  required_providers {
    aws = {
      source  = "hashicorp/aws"
      version = "~> 4.16"
    }
  }

  required_version = ">= 1.2.0"
}

provider "aws" {
  region  = "us-west-2"
}

resource "aws_instance" "app_server" {
  ami           = "ami-830c94e3"
  instance_type = "t2.micro"

  tags = {
    Name = "ExampleAppServerInstance"
  }
}
```

```
[INPUT]
git commit -m "feat:add basic terraform script"

[OUTPUT]
![image](https://github.com/JonathanMayorCPNV/Labo-Master-1/assets/115776017/63f64f24-f987-48f5-a8cf-2eca97cc9254)
```

* [ ] Finish the feature

```
[INPUT]
//TODO

[OUTPUT]
//TODO
```

* Push this modification on your repository

```
[INPUT]
git flow feature finish terraformBasicScript

[OUTPUT]
J'ai fermer la console CMD j'abandonne ...
```

* What happens to the feature/branch ?

```
//TODO
Add your answer with command line used to validate your analysis.
```

* Open a pull request comparing your develop branch to your main
* Assign the pull request to your partner

```
//TODO
Screenshot pull request on github
```

* Notify him using a issue "Could you please review my pull request ?"

```
//TODO
Screenshot issue on github
```
