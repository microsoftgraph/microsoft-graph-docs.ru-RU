---
author: JeremyKelley
title: Тип ресурса sharingLink
ms.localizationpriority: medium
description: Ресурсы sharingLink группирует связанные элементы данных в одну структуру.
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 95994292e4925e577c5ffe3dee4edb88fdeaf5a6
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034399"
---
# <a name="sharinglink-resource-type"></a>Тип ресурса sharingLink

Пространство имен: microsoft.graph

Группирует связанные элементы данных в одну структуру.

Если ресурс [**разрешений**](permission.md) имеет аспект **sharingLink** , отличный от NULL, разрешение представляет ссылку для общего доступа (в отличие от разрешений, предоставленных пользователю или группе).

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

| Свойство    | Тип          | Описание
|:------------|:--------------|:-------------------------------------
| application | [identity][]  | Приложение, с которым сопоставлена ссылка.
| type        | Строка        | Тип созданной ссылки.
| scope       | String        | Область ссылки, представленная этим разрешением. Значение `anonymous` указывает, что ссылку может использовать любой пользователь, значение `organization` указывает, что ссылку могут использовать только пользователи, выполнившие вход в один и тот же клиент.
| preventsDownload | Логическое       | Если значение равно true, пользователь может использовать эту ссылку только для просмотра элемента в Интернете и не может использовать его для скачивания содержимого элемента. Только для OneDrive для бизнеса и SharePoint.
| webHtml     | String        | Для ссылок `embed` это свойство содержит HTML-код элемента `<iframe>`, который внедряет элемент на веб-страницу.
| webUrl      | String        | URL-адрес, который открывает элемент в браузере на веб-сайте OneDrive.

[Identity]: identity.md

## <a name="type-options"></a>Параметры типа

В таблице ниже определены возможные значения свойства **type**.

| Значение   | Роль    | Описание
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | Ссылка для совместного доступа на просмотр, разрешающая доступ только для чтения.
| `edit`  | `write` | Ссылка для редактирования, разрешающая доступ для чтения и записи.
| `embed` | `read`  | Ссылка только для просмотра, с помощью которой можно внедрять содержимое в ведущую веб-страницу. Внедряемые ссылки недоступны в OneDrive для бизнеса и SharePoint.

## <a name="scope-options"></a>Параметры области

| Значение          | Описание
|:---------------|:------------------------------------------------------------
| `anonymous`    | Любой пользователь со ссылкой обладает правом доступа без необходимости входа в систему. Это также относится к людям вне вашей организации.
| `organization` | Любой пользователь, вошедший в вашу организацию (клиент), может использовать ссылку для получения доступа. Доступно только в OneDrive для бизнеса и SharePoint.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(view,edit,embed) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(anonymous,organization) are in resource, but () are in table"
  ],
  "tocPath": "Facets/SharingLink"
} -->

