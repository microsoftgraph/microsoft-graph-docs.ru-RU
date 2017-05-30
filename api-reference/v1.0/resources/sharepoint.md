# <a name="working-with-sharepoint-sites-in-microsoft-graph"></a>Работа с сайтами SharePoint в Microsoft Graph

API SharePoint в Microsoft Graph поддерживает следующие основные сценарии:

* доступ к ресурсам **drive** (библиотекам документов) и **site** для SharePoint;
* поддержка доступа к ресурсам **site** только для чтения (без возможности создавать сайты);
* поддержка доступа к ресурсам **driveItem** для чтения и записи;
* обращение к ресурсам с использованием идентификатора SharePoint, URL-адреса или относительного пути.

## <a name="sharepoint-api-root-resources"></a>Корневые ресурсы API SharePoint

Приведенные ниже примеры относятся к `https://graph.microsoft.com/v1.0`.

| Путь                                   | Описание
|:---------------------------------------|:------------------------------------
| /sites/root                            | Ресурс [site][] по умолчанию для организации.
| /sites/{site-id}                       | Доступ к определенному ресурсу [site][] с использованием его идентификатора.
| /sites/{site-id}/drive                 | Доступ к ресурсу [drive](drive.md) (библиотеке документов) для указанного ресурса [site][], заданному по умолчанию.
| /sites/{site-id}/drives                | Перечисление ресурсов [drive](drive.md) (библиотек документов) для [site][].
| /sites/{site-id}/sites                 | Перечисление дочерних сайтов для ресурса [site][].
| /groups/{group-id}/sites/root          | Доступ к ресурсу [site][] для ресурсов group (сайту группы).

К сайту также можно обратиться с помощью соответствующего пути. Для этого укажите имя узла SharePoint, за ним — двоеточие и относительный путь к сайту. При необходимости вы можете менять способ адресации (возвращаться к ресурсной модели), добавляя в конец двоеточие.

| Путь                                           | Описание
|:-----------------------------------------------|:-----------------------------------
| /sites/contoso.sharepoint.com:/teams/hr        | Сайт, связанный с https://contoso.sharepoint.com/teams/hr
| /sites/contoso.sharepoint.com:/teams/hr:/drive | Доступ к ресурсу [drive](drive.md), заданному по умолчанию.

## <a name="note-for-existing-sharepoint-developers"></a>Примечание, касающееся разработки решений для SharePoint

API SharePoint в Microsoft Graph имеет ряд ключевых отличий от API CSOM. Ресурс [site][] сопоставляется с `SPWeb`. Корневой ресурс [site][] (`SPWeb`) в семействе веб-сайтов имеет аспект [siteCollection](sitecollection.md), содержащий сведения о `SPSite`. Идентификатор сайта уникален только в пределах одного семейства веб-сайтов. Чтобы обратиться к сайту с использованием ИД, нужно предоставить два идентификатора — для семейства и для самого сайта.

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id},{spweb-id}/
```
URL-адрес, содержащий только имя узла, будет указывать на корневой сайт (`SPWeb`) в семействе веб-сайтов по умолчанию.

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname}
```

URL-адрес, содержащий только имя узла и идентификатор siteCollection (`SPSite`), будет указывать на корневой сайт (`SPWeb`) в указанном семействе веб-сайтов.

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id}
```

[site]: site.md
[drive]: drive.md
[siteCollection]: siteCollection.md

<!-- {
  "type": "#page.annotation",
  "description": "Getting started programming with the SharePoint API",
  "keywords": "getting started sharepoint rest api programming C# ios android rest http",
  "section": "documentation",
  "tocPath": "Getting Started",
  "tocIndex": -100
} -->
