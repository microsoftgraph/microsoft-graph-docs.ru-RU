---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: c21c891981106faa4b631bb2713913bfa8ed0713
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521455"
---
# <a name="sharinglink-resource-type"></a>Тип ресурса SharingLink

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **SharingLink** группирует связанные со ссылками элементы данных в единую структуру.

Если у ресурса [**Permission**](permission.md) имеется аспект **sharingLink**, значение которого отлично от NULL, разрешение представляет ссылку для совместного доступа (а не разрешение, предоставляемое пользователю или группе).

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
| type           | Строка        | Тип созданной ссылки.
| scope          | String        | Область ссылки, представленная этим разрешением. Значение `anonymous` указывает, что ссылку может использовать любой пользователь, значение `organization` указывает, что ссылку могут использовать только пользователи, выполнившие вход в один и тот же клиент.
| preventsDownload | Логическое       | Если значение true, пользователь этой ссылки можно использовать только для просмотра элемента в Интернете и нельзя использовать для загрузки содержимого элемента. Только для OneDrive для бизнеса и SharePoint.
| webHtml        | String        | Для ссылок `embed` это свойство содержит HTML-код элемента `<iframe>`, который внедряет элемент на веб-страницу.
| webUrl         | Строка        | URL-адрес, который открывает элемент в браузере на веб-сайте OneDrive.

[Identity]: identity.md

### <a name="type-options"></a>Параметры типа

Следующая таблица определяет возможные значения для свойства **типа** .

| Значение    | Роль     | Описание
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | Ссылка только для просмотра, разрешающая доступ только для чтения.
| `edit`   | `write`  | Ссылка для редактирования, разрешающая доступ для чтения и записи.
| `embed`  | `read`   | Ссылка только для просмотра, с помощью которой можно внедрять содержимое в ведущую веб-страницу. Внедряемые ссылки недоступны в OneDrive для бизнеса и SharePoint.

### <a name="scope-options"></a>Параметры области

Следующая таблица определяет возможные значения для свойства **области** .

| Значение            | Описание
|:-----------------|:------------------------------------------------------------
| `anonymous`      | Лица, имеющие ссылку имеет доступ, без необходимости входа. Сюда может входить пользователям за пределами вашей организации.
| `organization`   | Любой пользователь вошел в вашей организации (клиента) используйте ссылку для доступа. Доступно только в OneDrive для бизнеса и SharePoint.
| `existingAccess` | Только тех пользователей, которые уже имеют доступ к элементу другими способами возможен доступ к элементу, с помощью этой ссылки. Доступно только в OneDrive для бизнеса и SharePoint.
| `users`          | Ссылка предоставляет доступ только к определенному списку людей. Доступно только в OneDrive для бизнеса и SharePoint.

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
