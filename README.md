# mid_exam

# 1 ans 

class Library:
    book_list = [] 

    @classmethod
    def entry_book(cls, name):
        item = {"name": name}
        cls.book_list.append(item)



# 2 ans 

class Book:
    def __init__(self, book_id, title, author, availability=True):
        self.book_id = book_id
        self.title = title
        self.author = author
        self.availability = availability

    def borrow(self):
        if self.availability:
            self.availability = False
            print(f"The book '{self.title}' has been borrowed.")
        else:
            print(f"Sorry, the book '{self.title}' is not available.")

    def __repr__(self):
        return f"Book({self.book_id}, '{self.title}', '{self.author}')"

