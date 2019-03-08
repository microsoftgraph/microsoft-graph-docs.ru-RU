---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: 7f0ecdbb498ee75133ec9499027f7cfdc6191327
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480420"
---
# <a name="sharinglink-resource-type"></a>Тип ресурса sharingLink

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **sharingLink** группирует элементы данных, связанные с ссылками, в единую структуру.

Если ресурс [**Permission**](permission.md) имеет аспект **sharingLink** , отличный от NULL, разрешение представляет ссылку для совместного доступа (в отличие от разрешений, предоставленных пользователю или группе).

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": { "@odata.type": "microsoft.graph.identity" },
  "preventsDownload": false,
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a>Свойства

| Свойство       | Тип          | Описание
|:---------------|:--------------|:-------------------------------------
| application    | [identity][]  | Приложение, с которым сопоставлена ссылка.
| type           | String        | Тип созданной ссылки.
| scope          | String        | Область ссылки, представленная этим разрешением. Значение `anonymous` указывает, что ссылку может использовать любой пользователь, значение `organization` указывает, что ссылку могут использовать только пользователи, выполнившие вход в один и тот же клиент.
| Превентсдовнлоад | Boolean       | Если этот параметр имеет значение true, пользователь может использовать эту ссылку только для просмотра элемента в Интернете и не может использовать его для загрузки содержимого элемента. Только для OneDrive для бизнеса и SharePoint.
| webHtml        | String        | Для ссылок `embed` это свойство содержит HTML-код элемента `<iframe>`, который внедряет элемент на веб-страницу.
| webUrl         | Строка        | URL-адрес, который открывает элемент в браузере на веб-сайте OneDrive.

[Identity]: identity.md

### <a name="type-options"></a>Параметры типа

В приведенной ниже таблице определены возможные значения свойства **Type** .

| Значение    | Роль     | Описание
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | Ссылка для совместного доступа на просмотр, разрешающая доступ только для чтения.
| `edit`   | `write`  | Ссылка для редактирования, разрешающая доступ для чтения и записи.
| `embed`  | `read`   | Ссылка только для просмотра, с помощью которой можно внедрять содержимое в ведущую веб-страницу. Внедряемые ссылки недоступны в OneDrive для бизнеса и SharePoint.

### <a name="scope-options"></a>Параметры области

В приведенной ниже таблице определены возможные значения для свойства **Scope** .

| Значение            | Описание
|:-----------------|:------------------------------------------------------------
| `anonymous`      | Любой пользователь, у которого есть ссылка, имеет доступ, не требуя входа в систему. Сюда могут относиться пользователи за прев Организации.
| `organization`   | Любой пользователь, вошедший в организацию (клиент), может использовать эту ссылку для получения доступа. Доступно только в OneDrive для бизнеса и SharePoint.
| `existingAccess` | С помощью этой ссылки можно получить доступ к элементу только пользователям, у которых уже есть доступ к элементу. Доступно только в OneDrive для бизнеса и SharePoint.
| `users`          | Эта ссылка предоставляет доступ только к определенному списку пользователей. Доступно только в OneDrive для бизнеса и SharePoint.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharinglink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
