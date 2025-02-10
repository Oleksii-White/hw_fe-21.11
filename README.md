class Employee {
  constructor(name, surname, company) {
    this.name = name;
    this.surname = surname;
    this.company = company;
  }

  getFullName() {
    return `${this.name} ${this.surname}`;
  }
}

class Developer extends Employee {
  constructor(name, surname, company) {
    super(name, surname, company); 
  }

  getCompany() {
    return this.company;
  }
}

// Создаем объект Developer
const dev = new Developer("Иван", "Иванов", "TechCorp");

// Тестируем методы
console.log(dev.getFullName());
console.log(dev.getCompany());
