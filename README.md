#Juho Chat

This app is a chat application that utilizes a database and various 3rd-party libraries. I installed the CLTypeingLabel library, a 3rd-party library, using CocoaPods, and employed timers and loops to add motion when displaying the app name on the launch screen. I downloaded the pod file and applied the library accordingly.

On the main screen, new users can register using their email and password, while existing users can sign in with their respective email and password. I managed the systems using the navigation controller stack. Upon successful login, the chat screen is loaded. Additionally, I integrated Firebase into the app. When the chat screen loads, it accesses the Firestore cloud database system, retrieves message details such as body, sender, time, etc., and displays previous chats on the screen. The messages are sorted by time using the TimeInterval function, listing message cells in chronological order. Using the Cocoa Touch class, I created the MessageCell.swift and MessageCell.xib files, loading messages using a table view. During this process, I analyzed the message data from Firestore; if messages are sent by the current user, the message cells are displayed on the right side with the "Me" avatar; otherwise, they are displayed on the left side with the "You" avatar.

The upper-right navigation bar features a logout button. Clicking on it triggers the logout process using Firebase's logout method, returning the user to the main screen. Additionally, I utilized Package dependencies and integrated the 3rd-party library called IQKeyboardManager to manage keyboard behavior.

The Firebase project management page is used to oversee all messages and users.


https://github.com/dlwngh1367/FlashChat/assets/107776511/26c599ee-d30e-4722-93a6-5ffc831836f6  https://github.com/dlwngh1367/Juho-Chat/assets/107776511/e07bef36-51ff-430d-adbb-a2eac097f2e8


