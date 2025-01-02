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

# 3 ans 

    class Book:
    def __init__(self):
        self.book_list=[]
    
    def entry_book(self,book_id, titel, author, availability):
        item={
            "book_id":book_id,
            "titel":titel,
            "author":author,
            "availability":availability 
        }
        self.book_list.append(item)


# 4 ans 

    class Book:
        def __init__(self):
            self.book_list=[]
        
        def entry_book(self,book_id, titel, author, availability=True):
            item={
                "book_id":book_id,
                "titel":titel,
                "author":author,
                "availability":availability
            }
            self.book_list.append(item)
            
        def availabol(self,name):
            for item in self.book_list:
                if item["titel"]==name:
                    if item["availability"]==True:
                        print("Yes it availabil")
                        return
                    availability=False
                    print("sorry it ! Not availabil")
                    return
                print("sorry it ! Not availabil")
                return
            print("sorry it ! Not availabil")
            return
        def borrow_book(self,name):
            for item in self.book_list:
                if item["titel"]==name:
                    if item["availability"]==True:
                        item["availability"]=False
                        item["availability"]=item["availability"]-1
                        print(f"Thanks sir for take --> {name}")
                        return
                    print("sorry it ! Not availabil")
                    return
                print("sorry it ! Not availabil")
                return
            print("sorry it ! Not availabil")
            return
        
 
    ans=Book()
    ans.entry_book(12,"aaa","bbb",True)
    
    ans.availabol("aaa")
    ans.borrow_book("aaa")
    ans.availabol("aaa")

# 5 ans 
    class Book:
        def __init__(self):
            self.book_list=[]
        
        def entry_book(self,book_id, title, author, availability=True):
            item={
                "book_id":book_id,
                "title":title,
                "author":author,
                "availability":availability
            }
            self.book_list.append(item)
            
        def availabol(self,name):
            for item in self.book_list:
                if item["title"]==name:
                    if item["availability"]==True:
                        print("Yes it availabil")
                        return
                    availability=False
                    print("sorry it ! Not availabil")
                    return
                print("sorry it ! Not availabil")
                return
            print("sorry it ! Not availabil")
            return
        def borrow_book(self,name):
            for item in self.book_list:
                if item["title"]==name:
                    if item["availability"]==True:
                        item["availability"]=False
                        print(f"Thanks sir for take --> {name}")
                        return
                    print("sorry it ! Not availabil")
                    return
                print("sorry it ! Not availabil")
                return
            print("sorry it ! Not availabil")
            return
        def return_book(self,name):
            for item in self.book_list:
                if item["title"]==name:
                    item["availability"]=True
                    print("Thanks it back")
                    return
                else:
                    print("This book not borrowing")
                    return
 
    ans=Book()
    ans.entry_book(12,"aaa","bbb",True)
    
    ans.availabol("aaa")
    ans.borrow_book("aaa")
    ans.availabol("aaa")
    ans.return_book("aaa")
    ans.availabol("aaa")

# 6 ans

            
    class Book:
        def __init__(self):
            self.book_list=[]
        
        def entry_book(self,book_id, title, author, availability=True):
            item={
                "book_id":book_id,
                "title":title,
                "author":author,
                "availability":availability
            }
            self.book_list.append(item)
            
        def availabol(self,name):
            for item in self.book_list:
                if item["title"]==name:
                    if item["availability"]==True:
                        print("Yes it availabil")
                        return
                    availability=False
                    print("sorry it ! Not availabil")
                    return
                print("sorry it ! Not availabil")
                return
            print("sorry it ! Not availabil")
            return
        def borrow_book(self,name):
            for item in self.book_list:
                if item["title"]==name:
                    if item["availability"]==True:
                        item["availability"]=False
                        print(f"Thanks sir for take --> {name}")
                        return
                    print("sorry it ! Not availabil")
                    return
                print("sorry it ! Not availabil")
                return
            print("sorry it ! Not availabil")
            return
        def return_book(self,name):
            for item in self.book_list:
                if item["title"]==name:
                    item["availability"]=True
                    print("Thanks it back")
                    return
                else:
                    print("This book not borrowing")
                    return
                
        def book_info(self):
            for item in self.book_list:
                print(item)
     
    ans=Book()
    ans.entry_book(12,"aaa","bbb",True)
    
    ans.availabol("aaa")
    ans.borrow_book("aaa")
    ans.availabol("aaa")
    ans.return_book("aaa")
    ans.availabol("aaa")
    
    ans.book_info()



# 7 & 8 ans
        
    class Book:
        def __init__(self):
            self.book_list=[]
    
        def entry_book(self,book_id, title, author, availability=True):
            item={
                "book_id":book_id,
                "title":title,
                "author":author,
                "availability":availability
            }
            self.book_list.append(item)
            
        def availabol(self,name):
            for item in self.book_list:
                if item["title"]==name:
                    if item["availability"]==True:
                        print("Yes it availabil")
                        return
                    availability=False
                    print("sorry it ! Not availabil")
                    return
                print("sorry it ! Not availabil")
                return
            print("sorry it ! Not availabil")
            return
        def borrow_book(self,name):
            for item in self.book_list:
                if item["title"]==name:
                    if item["availability"]==True:
                        item["availability"]=False
                        print(f"Thanks sir for take --> {name}")
                        return
                    print("sorry it ! Not availabil")
                    return
                print("sorry it ! Not availabil")
                return
            print("sorry it ! Not availabil")
            return
        def return_book(self,name):
            for item in self.book_list:
                if item["title"]==name:
                    item["availability"]=True
                    print("Thanks it back")
                    return
                else:
                    print("This book not borrowing")
                    return
                
        def book_info(self):
            for item in self.book_list:
                print(item)
     
        ans=Book()
        ans.entry_book(12,"aaa","bbb",True)
        
    while True:
        n=int(input("Enter your menu digit : "))
        if n==1:
            ans.book_info()
        elif n==2:
            nam=input("Enter borrowing book name : ")
            ans.borrow_book(nam)
        elif n==3:
            nam=input("Enter return book name : ")
            ans.return_book(nam)
        elif n==4:
            break


# 9 ans 
    
    class Book:
        def __init__(self):
            self.book_list=[]
        
        def entry_book(self,book_id, title, author, availability=True):
            item={
                "_book_id":book_id,
                "_title":title,
                "_author":author,
                "_availability":availability
            }
            self.book_list.append(item)
            
        def availabol(self,name):
            for item in self.book_list:
                if item["_title"]==name:
                    if item["_availability"]==True:
                        print("Yes it availabil")
                        return
                    item["_availability"] = False
                    print("sorry it ! Not availabil")
                    return
                print("sorry it ! Not availabil")
                return
            print("sorry it ! Not availabil")
            return
        def borrow_book(self,name):
            for item in self.book_list:
                if item["_title"]==name:
                    if item["_availability"]==True:
                        item["_availability"]=False
                        print(f"Thanks sir for take --> {name}")
                        return
                    print("sorry it ! Not availabil")
                    return
                print("sorry it ! Not availabil")
                return
            print("sorry it ! Not availabil")
            return
        def return_book(self,name):
            for item in self.book_list:
                if item["_title"]==name:
                    item["_availability"]=True
                    print("Thanks it back")
                    return
                else:
                    print("This book not borrowing")
                    return
                
        def book_info(self):
            for item in self.book_list:
                print(item)

    ans=Book()
    ans.entry_book(12,"aaa","bbb",True)
    
    while True:
        n=int(input("Enter your menu digit : "))
        if n==1:
            ans.book_info()
        elif n==2:
            nam=input("Enter borrowing book name : ")
            ans.borrow_book(nam)
        elif n==3:
            nam=input("Enter return book name : ")
            ans.return_book(nam)
        elif n==4:
            break
    
    



    
