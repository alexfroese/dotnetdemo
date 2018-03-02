# dotnetdemo

you'll need to create a database file inside App_Data called "Sample" in order for this to work. then just run

```
CREATE TABLE CarMakes(
    ID int identity(1,1) not null,
    Name nvarchar(50) not null,
    CONSTRAINT PK_CarMakes primary key (ID asc)
);

INSERT INTO CarMakes (Name)
VALUES ('Alfa Romeo'), ('Alpina'), ('Aston Martin'), ('Audi'), ('Bentley'), ('BMW'), ('Citroen'), ('Dacia'), ('DS'), ('Ferrari'), ('Fiat'), ('Ford'), ('Honda'), ('Hyundai'), ('Infiniti'), ('Jaguar'), ('Jeep'), ('Kia'), ('Lamborghini'), ('Land Rover'), ('Lexus'), ('Lotus'), ('Maserati'), ('Mazda'), ('McLaren'), ('Mercedes'), ('MG'), ('Mini'), ('Mitsubishi'), ('Nissan'), ('Peugeot'), ('Porsche'), ('Renault'), ('Rolls-Royce'), ('Seat'), ('Skoda'), ('Smart'), ('SsangYong'), ('Subaru'), ('Suzuki'), ('Tesla'), ('Toyota'), ('Vauxhall'), ('Volkswagen'), ('Volvo');
```

it's also worth noting that when i was adding the entity framework file to the project, i went into the nuget package console thing and
entered the command

```
install-package entityframework
```

because i guess it isn't included by default
