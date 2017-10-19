---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
ms.openlocfilehash: 7b7729899d134fa1d5de7debb1f209ec5aadd70d
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="sharinglink-resource-type"></a>Тип ресурса SharingLink

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
| webHtml     | String        | Для ссылок `embed` это свойство содержит HTML-код элемента `<iframe>`, который внедряет элемент на веб-страницу.
| webUrl      | Строка        | URL-адрес, который открывает элемент в браузере на веб-сайте OneDrive.

[Identity]: identity.md

## <a name="type-enumeration"></a>Перечисление type

В таблице ниже определены возможные значения свойства **type**.

| Значение   | Роль    | Описание
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | Ссылка только для просмотра, разрешающая доступ только для чтения.
| `edit`  | `write` | Ссылка для редактирования, разрешающая доступ для чтения и записи.
| `embed` | `read`  | Ссылка только для просмотра, с помощью которой можно внедрять содержимое в ведущую веб-страницу. Внедряемые ссылки недоступны в OneDrive для бизнеса и SharePoint.

## <a name="scope-enumeration"></a>Перечисление областей

| Значение          | Описание                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | Ссылку для общего доступа могут использовать все пользователи.                                                                            |
| `organization` | Ссылку для совместного доступа могут использовать все пользователи в одной и той же организации (клиенте). Эта функция недоступна в OneDrive персональный. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "Facets/SharingLink"
} -->
