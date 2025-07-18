## SQL setting

```
CREATE DATABASE StaticResource;
GO

CREATE LOGIN StaticResourceSa WITH PASSWORD = '!QAZPass@WSX';
GO

USE StaticResource;
GO

CREATE USER StaticResourceSa FOR LOGIN StaticResourceSa;
GO

ALTER ROLE db_owner ADD MEMBER StaticResourceSa;
GO
```