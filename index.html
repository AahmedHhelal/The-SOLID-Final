from abc import ABC, abstractmethod
from typing import List

# Single Responsibility Principle
class Task:
    def __init__(self , title , description):
        self.title = title
        self.description = description
        self.completed = False

    def complete(self):
        self.completed = True

# Open/Closed Principle
class TaskRepository(ABC):
    @abstractmethod
    def add_task(self , task):
        pass

    @abstractmethod
    def get_all_tasks(self):
        pass

class InMemoryTaskRepository(TaskRepository):
    def __init__(self):
        self.tasks = []

    def add_task(self , task):
        self.tasks.append(task)

    def get_all_tasks(self):
        return self.tasks

# Liskov Substitution Principle
def complete_task(task):
    task.complete()

# Interface Segregation Principle
class TaskNotifier(ABC):
    @abstractmethod
    def notify(self , task):
        pass

class EmailNotifier(TaskNotifier):
    def notify(self , task):
        print(f"Email: Task '{task.title}' has been completed.")

class SMSNotifier(TaskNotifier):
    def notify(self , task):
        print(f"SMS: Task '{task.title}' has been completed.")

# Dependency Inversion Principle
class TaskManager:
    def __init__(self , repository , notifier):
        self.repository = repository
        self.notifier = notifier

    def add_task(self , title , description):
        task = Task(title, description)
        self.repository.add_task(task)

    def complete_task(self , task):
        complete_task(task)
        self.notifier.notify(task)

# Function to demonstrate the usage of the TaskManager
def run_task_manager():
    # Create a task repository and notifier
    task_repository = InMemoryTaskRepository()
    email_notifier = EmailNotifier()

    # Create a task manager
    task_manager = TaskManager(task_repository, email_notifier)

    # Add a task
    task_manager.add_task("Write Code", "Implement SOLID principles in Python.")

    # Complete the task
    tasks = task_repository.get_all_tasks()
    for task in tasks:
        task_manager.complete_task(task)

# Call the function to run the task manager
run_task_manager()



# Explanation of SOLID Principles in the Code:

# 1) Single Responsibility Principle (SRP):
# The Task class is responsible for managing task details (title, description, completion status).
# The InMemoryTaskRepository class is responsible for storing and retrieving tasks.
# The EmailNotificationService and SMSNotificationService classes are responsible for sending notifications.
    
# 2) Open/Closed Principle (OCP):
# The TaskRepository is an abstract class that can be extended to create different types of repositories (e.g., a database repository) without modifying existing code.

# 3) Liskov Substitution Principle (LSP):
# The complete_task function can accept any Task object, ensuring that any subclass of Task can be used without affecting the correctness of the program.

# 4) Interface Segregation Principle (ISP):
# The NotificationService interface allows different notification methods to be implemented without forcing clients to depend on unused methods.

# 5) Dependency Inversion Principle (DIP):
# The TaskManager class depends on abstractions (TaskRepository and NotificationService) rather than concrete implementations, allowing for flexibility in how tasks are stored and how notifications are sent.