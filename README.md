<br>
<div align='center'>
	<h1>HandyHome Hub App Back-end (API)</h1>
  </div>
<a name="readme-top"></a>

# 📗 Table of Contents
- [📖 About the Project](#about-project)
  - [🛠 Built With](#built-with)
  - [Tech Stack](#tech-stack)
  - [Key Features](#key-features)
  - [🚀 Live Demo](#live-demo)
- [💻 Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Setup](#setup)
  - [Usage](#usage)
  - [Tests](#tests)
- [👥 Authors](#authors)
- [📈 Kanban Board](#kanban)
- [🔭 Future Features](#future-features)
- [🤝 Contributing](#contributing)
- [⭐️ Show your support](#support)
- [🙏 Acknowledgements](#acknowledgements)
- [📝 License](#license)


# ⚙️ "HandyHome Hub" Backend  <a name="about-project"></a>

**HandyHome Hub Back-End" is a Ruby on Rails application that serves as a RESTful API. It utilizes PostgreSQL as its database.
This API serves as the server-side component for booking appointments with home service providers, making it easy for users to schedule services such as house cleaning, plumbing, or any other home-related tasks.

## 🖥️Integration with Front-End

This back-end project is designed to seamlessly integrate with its counterpart *front-end project* 👉🏽[handyhommehub_frontend](https://github.com/jicamargo/handyhommehub_frontend). The front-end, built with React.js and Redux, consumes the API provided by this back-end to provide a user-friendly interface for booking appointments.
## 🛠 Built With <a name="built-with"></a>

### Tech Stack <a name="tech-stack"></a>
<details>
<summary>Ruby</summary>
  <ul>
    <li><a href="https://www.ruby-lang.org/">Ruby</a></li>
  </ul>
</details>
<details>
<summary>Rails</summary>
  <ul>
    <li><a href="https://rubyonrails.org/">Ruby</a></li>
  </ul>
</details>
<details>
<summary>RSpec</summary>
  <ul>
    <li><a href="https://rspec.info/">RSpec</a></li>
  </ul>
</details>
<details>
<summary>PostgreSQL</summary>
  <ul>
    <li><a href="https://www.postgresql.org/">PostgreSQL</a></li>
  </ul>
</details>
<details>
<summary>Swagger</summary>
  <ul>
    <li><a href="https://swagger.io/">Swagger</a></li>
  </ul>
</details>

#### Key Features <a name="key-features"></a>

- User authentication: Users can log in to the website using their username.
- User authorization: Users can only access their own appointments.
- Viewing home services: Users can see a list of available home services with details.
- Appointment booking: Users can book appointments with service providers.
- Services management: Service providers ("admin" users) can create, edit, and delete services.


<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- LIVE DEMO  -->

## 🚀 Live Demo <a name="live-demo"></a>

- Enjoy the live version of the API with its front-end counterpart [here](https://handyhomehub.netlify.app/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->

## 💻 Getting Started <a name="getting-started"></a>

### Prerequisites

In order to run this project you need the following installed locally:

```sh
 gem install ruby
```
```sh 
 gem install rails
```

- Linux:

```sh
  sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list'
  wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -
  sudo apt-get update
  sudo apt-get -y install postgresql
```
- Windows:
  [Visit this website for detailed instructions](https://www.postgresql.org/download/windows/)

- Mac:
  [Visit this website for detailed instructions](https://www.postgresql.org/download/macosx/)


### Setup

1. Clone the repository:

```
  git clone https://github.com/jicamargo/handyhommehub_backend.git
```

2. Install the dependencies:

```
  run bundle install
```

### Usage
1. Create a master key file in the config folder and add the master key to it. This key is used to decrypt the credentials.yml.enc file. You can use the following command to generate the key:

```
  1. Remove config/master.key and config/credentials.yml.enc if they exist.
  2. Run in the terminal: EDITOR=code rails credentials:edit 
  3. Close the editor that opens.
  4. This command will create a new master.key and credentials.yml.enc
   if they do not exist.
```

2. Configure the database.yml file with your database credentials
```
    development:
        <<: *default
        database: your_database_name
        username: your_username
        password: your_password
        port: 5432
         
    test:
        <<: *default
        database: your_database_name
        username: your_username
        password: your_password
        port: 5432
```
3. Set up the database

```
  rails db:create
  rails db:migrate
```

4. Start the server in your favorite terminal:

```
  rails server
```

5. Review the API documentation here: [Swagger API Documentation](https://appointments-ajt3.onrender.com/api-docs/index.html)


### Tests

You can run tests with the following command:
```sh 
  rspec
```

1. **Front End**: To install the front-end of this project, please visit the [handyhommehub_frontend](https://github.com/jicamargo/handyhommehub_frontend) repository and follow the instructions in the README.md file.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 👥 Authors (in alphabetical order)<a name="authors"></a>
>

👤 **Cosmos Hagan**
- GitHub: [cosmosha](https://github.com/Cosmosha)
- LinkedIn: [cosmoshagan](https://gh.linkedin.com/in/cosmoshagan)
- Twitter: [@hagancosmos](https://twitter.com/hagancosmos)

👤 **Ibrahim Hossain**
- GitHub: [ibugithub](https://github.com/ibugithub)
- LinkedIn: [ibuu](https://www.linkedin.com/in/ibuu/)
- Twitter: [@mdibrahimibuu](https://twitter.com/mdibrahimibuu)

👤 **Jorge Camargo**
- GitHub: [@jicamargo](https://github.com/jicamargo)
- LinkedIn: [Jorge Camargo](https://www.linkedin.com/in/jorgecamargog/?locale=en_US)
- Twitter: [@ji_camargo](https://twitter.com/ji_camargo)

👤 **Lincoln Gibson**
- GitHub: [lincoln1883](https://github.com/lincoln1883)
- LinkedIn: [lincoln-gibson](https://www.linkedin.com/in/lincoln-gibson)
- Twitter: [@lincolngibson7](https://twitter.com/lincolngibson7)

👤 **Moyasi Ginko**
- GitHub: [@MoyasiGinko](https://github.com/MoyasiGinko)
- LinkedIn: [moyasi](https://www.linkedin.com/in/moyasi/)
- Twitter: [@moyasi_ginko](https://twitter.com/moyasi_ginko)


<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 📈 Kanban Board<a name="kanban"></a>

The project's kanban board is available [here](https://github.com/lincoln1883/appointment-capstone-backend/projects/1)

You can see a screenshoot of the initial state of the board below:

![Kanban Board](./public/kanban-board-initial.png)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 🔭 Future Features <a name="future-features"></a>

- [ ] **Add categories to services**
- [ ] **Add payment processing**
- [ ] **Add user profiles**
- [ ] **Add user reviews and ratings**

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 🤝 Contributing <a name="contributing"></a>

Contributions, issues, and feature requests are welcome!

Feel free to check the [issues page](https://github.com/jicamargo/handyhommehub_backend/issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## ⭐️ Show your support <a name="support"></a>

- If you like this project please give it a ⭐️!

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 🙏 Acknowledgments <a name="acknowledgements"></a>

- We would like to thank to [microverse](https://www.microverse.org/) For teaching me the database and more things.
- Thank to Murat Korkmaz on Behance for the design of the website 👉🏽.(https://www.behance.net/gallery/26425031/Vespa-Responsive-Redesign)
- Thanks a lot to everyone who will get time to check this out.


<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 📝 License <a name="license"></a>

This project is [MIT](./LICENSE) licensed.

<p align="right">(<a href="#readme-top">back to top</a>)</p>
