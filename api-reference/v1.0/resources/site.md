# <a name="site-resource"></a>Ресурс site

Ресурс **site** предоставляет метаданные и связи для сайта SharePoint.

## <a name="tasks"></a>Задачи

Все приведенные ниже примеры относятся к `https://graph.microsoft.com/v1.0`.

| Имя задачи            | Пример запроса                                   |
| :------------------- | :------------------------------------------------ |
| [Получение корневого сайта][]    | GET /sites/root                                   |
| [Получение сайта][]         | GET /sites/{site-id}                              |
| [Получение сайта по пути][] | GET /sites/{hostname}:/{site-path}                |
| [Получение сайта для группы][] | GET /groups/{group-id}/sites/root             |

[Получение сайта]: ../api/site_get.md
[Получение корневого сайта]: ../api/site_get.md
[Получение сайта по пути]: ../api/site_get.md
[Получение сайта для группы]: ../api/site_get.md

## <a name="json-representation"></a>Представление JSON

Ниже показано представление ресурса **site** в формате JSON.

Ресурс **driveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.

<!-- { "blockType": "resource",
       "@odata.type": "microsoft.graph.site",
       "keyProperty": "id",
       "optionalProperties": [ "root", "sharepointIds", "siteCollection", "drive", "drives", "sites" ] } -->

```json
{
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},
  "displayName": "string",

  /* relationships */
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

## <a name="properties"></a>Свойства

| Имя свойства            | Тип                                | Описание                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| **id**                   | string                              | Уникальный идентификатор элемента. Только для чтения.                                                  |
| **createdDateTime**      | DateTimeOffset                      | Дата и время создания элемента. Только для чтения.                                             |
| **description**          | string                              | Текст с описанием сайта.                                                             |
| **displayName**          | string                              | Полное название сайта. Только для чтения.                                                        |
| **lastModifiedDateTime** | DateTimeOffset                      | Дата и время последнего изменения элемента. Только для чтения.                                       |
| **name**                 | string                              | Имя или название элемента.                                                                  |
| **root**                 | [root](root.md)                     | Если это свойство присутствует, оно указывает на то, что сайт — корневой в семействе веб-сайтов. Только для чтения.            |
| **sharepointIds**        | [sharepointIds](sharepointids.md)   | Возвращает идентификаторы, использующиеся для обеспечения совместимости с SharePoint REST. Только для чтения.                       |
| **siteCollection**       | [siteCollection](sitecollection.md) | Предоставляет сведения о семействе веб-сайтов сайта. Доступно только на корневом сайте. Только для чтения. |
| **webUrl**               | string (url)                        | URL-адрес для отображения элемента в браузере. Только для чтения.                                          |

## <a name="relationships"></a>Связи

| Имя связи | Тип                     | Описание
|:------------------|:-------------------------|:----------------------------------
| **drive**         | [drive][]                | Диск по умолчанию (библиотека документов) для этого сайта.
| **drives**        | Collection([drive][])    | Коллекция дисков (библиотек документов) на этом сайте.
| **items**         | Collection([baseItem][]) | Используется для адресации любого элемента, содержащегося на этом сайте. Вам не удастся выполнить перечисление этой коллекции.
| **sites**         | Collection([site][])     | Коллекция дочерних сайтов этого сайта.

[baseItem]: baseitem.md
[drive]: drive.md
[identitySet]: identityset.md
[site]: site.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Site",
  "tocBookmarks": {
    "Site": "#"
  }
} -->
