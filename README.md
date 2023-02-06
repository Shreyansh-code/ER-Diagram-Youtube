 EER-Diagram-Youtube

 Entity 1 - Users
    Users can be distinguised as creators(who creates videos) and consumers(who consumes videos)
    It has attributes namely; User ID(primary Key), name of the user, age of the user,email of the user and the address of the user.

 Entity 2 - Channel
    Users can have multiple channels.
    It has the attributes namely; Channel ID(PK), Owner ID(FK from User table/entity(User ID)), Owner name, sub count, date and time of creation.

 Entity 3 - Video
    Channel can have multiple videos
    Video has the attributes namely; Video ID(PK), Uploader ID(FK from User table/entity(User ID)), URL, Title, Thumbnail, Category, Description, Upload       date and time, Duration of the video and Sponsor ID(Boolean value)

 Entity 4 - Video Stats
    1 Video can one 1 Video Stat 
    Video Stats has statstics of a particular video. It has attributes namely; Video ID(PK), Like Count, Dislike Count, Comment Count, View Count, Share       Count, Sponsor ID(can takle the value Null if sponsor is 'NO' in Video entity)
     
 Entity 5 - Comments
    1 Video can have multiple Comments
    Comments have attributes namely; Video ID(PK), Comment(the text itself), sentiment of comment, User ID(FK), date and time of creation.
    
 Entity 6 - Sponsors
    1 video can have many sponsors
    Sponsors have attributes namely; Video ID(FK), Sponsors ID(FK), User ID(FK), name of the sponsor, phone, address, amount sponsored.
