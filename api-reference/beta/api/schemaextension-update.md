---
title: Обновление schemaExtension
description: Обновление свойств в определении указанного schemaExtension.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 01d070a6a0e7be83ff1f50b48be75365f9041173
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267055"
---
# <a name="update-schemaextension"></a>Обновление schemaExtension

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

## <a name="request-body"></a>Тело запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|description|String|Описание расширения схемы.|
|properties|Коллекция [extensionSchemaProperty](../resources/extensionschemaproperty.md)|Коллекция типов и имен свойств, составляющих определение расширения схемы. Разрешены только добавочные изменения. |
|status|String|Состояние жизненного цикла расширения схемы. Начальное состояние при создании разрабатывается. **** Переход между состояниями возможен из **разработки** в **доступном** и **доступном** для **устаревших**состояниях.|
|targetTypes|Коллекция String|Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.  Разрешены только добавочные изменения.|

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/schemaExtensions/{id}
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
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/update_schemaextension-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_schemaextension-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_schemaextension-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schemaextension-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/schemaextension-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schemaextension-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
