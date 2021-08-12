---
author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
description: Ресурс SharingLink группирует связанные ссылками элементы данных в единую структуру.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0f3af451817cbae0c4d4930b035792482e06afac07de77f1b4ff1c975d431a06
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237539"
---
# <a name="sharinglink-resource-type"></a>Тип ресурса SharingLink

Пространство имен: microsoft.graph

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

| Свойство    | Тип          | Описание
|:------------|:--------------|:-------------------------------------
| application | [identity][]  | Приложение, с которым сопоставлена ссылка.
| type        | String        | Тип созданной ссылки.
| scope       | String        | Область ссылки, представленная этим разрешением. Значение `anonymous` указывает, что ссылку может использовать любой пользователь, значение `organization` указывает, что ссылку могут использовать только пользователи, выполнившие вход в один и тот же клиент.
| preventsDownload | Логическое       | Если это верно, пользователь может использовать эту ссылку только для просмотра элемента в Интернете и не может использовать его для скачивания содержимого элемента. Только для OneDrive для бизнеса и SharePoint.
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

## <a name="scope-options"></a>Параметры Области

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

