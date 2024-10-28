## Case Study: Smart Home System

### Overview
Learners will build a simple smart home simulation, modelling devices such as lights, thermostats, security cameras, and speakers. The goal is to apply OOP principles to design a flexible and extensible system capable of managing different smart devices.

---

## Activity Outline

### 1. Abstraction

- **Objective**: Understand how to define essential characteristics and behaviour for each smart device, ignoring unnecessary details.
- **Task**: 
  - Create an abstract `Device` class that includes essential properties (e.g., `name`, `status`, `location`) and methods (`turnOn()`, `turnOff()`, `showStatus()`).
  - Focus on defining general methods common to all devices without worrying about specifics.
- **Learning Objective**: Learners should learn how abstraction helps simplify complex systems by focusing on relevant characteristics shared by all devices.
- **Follow-up Discussion**: Discuss how abstraction helps in maintenance and scalability.

---

### 2. Encapsulation

- **Objective**: Learn to protect data within classes and control access to it.
- **Task**: 
  - Implement private properties in each device class (e.g., `currentTemperature` in `Thermostat`, `brightnessLevel` in `Light`).
  - Create getter and setter methods to access these properties, allowing rules to prevent invalid data entries (e.g., temperature range).
- **Learning Objective**: By the end, learners should understand encapsulation's role in data protection, security, and stability.

- **Follow-up Discussion**: Reflect on why restricting access to certain data fields could be beneficial (e.g., preventing incorrect values for temperature or brightness).

---

### 3. Inheritance

- **Objective**: Understand how inheritance allows for code reuse and a natural hierarchy.
- **Task**: 
  - Create specific device classes (`Light`, `Thermostat`, `Camera`) that inherit from `Device`. Each subclass should have unique methods (e.g., `adjustBrightness()` for `Light`, `setTemperature()` for `Thermostat`).
- **Learning Objective**: Learners will see how inheritance helps avoid redundant code and makes code structure more intuitive.
- **Follow-up Discussion**: Discuss the benefits and limitations of inheritance. Consider situations where inheritance may or may not be the best approach.

---

### 4. Polymorphism

- **Objective**: Use polymorphism to allow different devices to behave differently while maintaining a unified interface.
- **Task**: 
  - Implement polymorphism by having a `turnOn()` and `turnOff()` method in each device class with different implementations. For example:
    - `turnOn()` in `Light` adjusts brightness.
    - `turnOn()` in `Thermostat` starts adjusting to a preset temperature.
  - Use a list of `Device` objects and iterate over them, calling `turnOn()` and `turnOff()` on each. Each device should perform its specific function despite being called through a common interface.
- **Learning Objective**: Learners should recognize polymorphism's value in creating flexible code that can handle multiple types of objects seamlessly.
- **Follow-up Discussion**: Discuss how this approach could help in real-world systems where new devices might be added without altering existing code.

---

## Practical Task and Reflection

1. **Practical Task**: Ask learners to add a new device class, such as `Speaker`, that plays music when turned on. This assessment gauges whether they understand how to extend the existing structure with minimal changes to other classes.

2. **Reflection**: Conclude the activity by having learners write a brief reflection on how each principle (Abstraction, Encapsulation, Inheritance, Polymorphism) supported the development of the smart home system. Encourage them to think about why OOP principles are crucial for building scalable and maintainable software systems.

---