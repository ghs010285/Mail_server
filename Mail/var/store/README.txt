$JAMES_ROOT/var/store

     This folder contains the files related to database, activemq,... needed by James.
     James Server default settings comes with a embedded Derby database that stores the 
     users, domains and mailboxes (the user mails) (see store/derby folder).

     Of course, if you changed database.properties and still use a database for the mailboxes,
     you will have to look for the users, domains and mailboxes in your database, whatever,
     wherever it is.

     You can find in store folder sub-folders such as:
     
      * activemq
        +-brokers
          +-james
        +-blob-transfer
          +-outgoing
          +-spool
          
          The activemq component is configured to use this folder
          for queues (and topics if any) processing.
