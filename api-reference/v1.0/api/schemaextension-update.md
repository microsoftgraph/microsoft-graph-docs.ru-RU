---
title: Обновление schemaExtension
description: Обновление свойств в определении указанного schemaExtension.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 72b94f492947ef5853d14283eca33a682ea14b05
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603867"
---
# <a name="update-schemaextension"></a>Обновление schemaExtension

Обновление свойств в определении указанного [schemaExtension](../resources/schemaextension.md).

Обновление применяется ко всем ресурсам, включенным в свойство **TargetType** расширения. Эти ресурсы относятся к [типам вспомогательных ресурсов](/graph/extensibility-overview#supported-resources).

Только приложение, которое создало расширение схемы (приложение-владелец), может вносить добавочные обновления расширения, когда расширение находится в **** состоянии "разрабатывает" или " **доступно** ". Это означает, что приложение не может удалять настраиваемые свойства или целевые типы ресурсов из определения. Однако приложение может изменить описание расширения.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a>Необязательные заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Content-Type   | application/json |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|description|String|Описание расширения схемы.|
|properties|Коллекция [extensionSchemaProperty](../resources/extensionschemaproperty.md)|Коллекция типов и имен свойств, составляющих определение расширения схемы. Разрешены только добавочные изменения. |
|status|String|Состояние жизненного цикла расширения схемы. Начальное состояние при создании разрабатывается. **** Переход между состояниями возможен из **разработки** в **доступном** и **доступном** для **устаревших**состояниях.|
|targetTypes|Коллекция String|Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.  Разрешены только добавочные изменения.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```

##### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>Пример кода для SDK
# <a name="ctabcs"></a>[Языках](#tab/cs)
[!INCLUDE [sample-code](../includes/update_schemaextension-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Язык](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_schemaextension-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/schemaextension-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/schemaextension-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
