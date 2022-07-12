---
author: JeremyKelley
description: Ресурсы sharingLink группирует связанные элементы данных в одну структуру.
ms.date: 09/10/2017
title: SharingLink
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 27d9b586c0fe992075ee61424133e9b16259977c
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66731918"
---
# <a name="sharinglink-resource-type"></a>Тип ресурса sharingLink

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурсы **sharingLink** группирует связанные элементы данных в одну структуру.

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

| Свойство       | Тип          | Описание
|:---------------|:--------------|:-------------------------------------
| application    | [identity][]  | Приложение, с которым сопоставлена ссылка.
| type           | String        | Тип созданной ссылки.
| scope          | String        | Область ссылки, представленная этим разрешением. Значение `anonymous` указывает, что ссылку может использовать любой пользователь, значение `organization` указывает, что ссылку могут использовать только пользователи, выполнившие вход в один и тот же клиент.
| preventsDownload | Логическое       | Если значение равно true, пользователь может использовать эту ссылку только для просмотра элемента в Интернете и не может использовать его для скачивания содержимого элемента. Только для OneDrive для бизнеса и SharePoint.
| webHtml        | String        | Для ссылок `embed` это свойство содержит HTML-код элемента `<iframe>`, который внедряет элемент на веб-страницу.
| webUrl         | String        | URL-адрес, который открывает элемент в браузере на веб-сайте OneDrive.

[Identity]: identity.md

### <a name="type-options"></a>Параметры типа

В следующей таблице определены возможные значения для **свойства** типа.

| Значение    | Роль     | Описание
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | Ссылка для совместного доступа на просмотр, разрешающая доступ только для чтения.
| `edit`   | `write`  | Ссылка для редактирования, разрешающая доступ для чтения и записи.
| `embed`  | `read`   | Ссылка только для просмотра, с помощью которой можно внедрять содержимое в ведущую веб-страницу. Внедряемые ссылки недоступны в OneDrive для бизнеса и SharePoint.

### <a name="scope-options"></a>Параметры области

В следующей таблице определены возможные значения для **свойства области** .

| Значение            | Описание
|:-----------------|:------------------------------------------------------------
| `anonymous`      | Любой пользователь со ссылкой обладает правом доступа без необходимости входа в систему. Это также относится к людям вне вашей организации.
| `organization`   | Любой пользователь, вошедший в вашу организацию (клиент), может использовать ссылку для получения доступа. Доступно только в OneDrive для бизнеса и SharePoint.
| `existingAccess` | Только пользователи, которым уже был предоставлен доступ к элементу с помощью других средств, могут получить доступ к элементу по этой ссылке. Доступно только в OneDrive для бизнеса и SharePoint.
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
  "suppressions": []
}
-->


