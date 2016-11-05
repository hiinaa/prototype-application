# protospace

User
---

###association

has_many prototypes,comments,coptureimages

table
---

nickname  
password  
email  
profile  
works  
top_aligned_media  
profile_image  

Prototype
---

###association

has_many coptureimages,comments,likes  
belongs_to user

###table
title  
catch_copy  
concept  
user_id

Captureimage
---

###association
belongs_to prototype

###table

main_image  
sub_image  
prototype_id    
user_id  

Like
---

###association
belongs_to user,prototype

###table

user_id  
prototype_id  

Comment
---

###association
belongs_to user,prototype

###table
title_id  
content  
user_id  
prototype_id
