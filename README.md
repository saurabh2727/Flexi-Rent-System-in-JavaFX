# FlexiRent
    open project in IntellijIDEA
    create database in mysql
    execute these query

    --------------------------------------------------
    CREATE TABLE `User` (
      `Id` int(11) NOT NULL,
      `UsrName` varchar(20) NOT NULL,
      `FullName` varchar(100) DEFAULT NULL,
      `EmailAddress` varchar(100) DEFAULT NULL,
      `ContactNumber` varchar(100) DEFAULT NULL,
      `Address` text,
      `Password` varchar(45) DEFAULT NULL,
      `Status` tinyint(1) NOT NULL DEFAULT '0',
      `UserImage` mediumblob,
      `Date` date NOT NULL,
      `CreatorId` int(11) DEFAULT NULL
    ) ENGINE=InnoDB DEFAULT CHARSET=latin1;

    --
    -- Dumping data for table `User`
    --

    INSERT INTO `User` (`Id`, `UsrName`, `FullName`, `EmailAddress`, `ContactNumber`, `Address`, `Password`, `Status`, `UserImage`, `Date`, `CreatorId`) VALUES
    (1, 'saurav', 'saurav', NULL, NULL, NULL, 'secret', 1, NULL, '2018-09-27', NULL);

    ALTER TABLE `User`
      ADD PRIMARY KEY (`Id`),
      ADD UNIQUE KEY `Id` (`Id`);

    --
    -- AUTO_INCREMENT for dumped tables
    --

    --
    -- AUTO_INCREMENT for table `User`
    --
    ALTER TABLE `User`
      MODIFY `Id` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=2;

    ----------------------------------------------------------------------------

    edit database.properties file according to your mysql

    run project RentSystem.java as java main file
