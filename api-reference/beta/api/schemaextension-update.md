---
title: Обновление schemaExtension
description: Обновление свойств в определении указанного ресурса schemaExtension.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: f457609af15716ef2ada3945132afd285fd2394c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515540"
---
# <a name="update-schemaextension"></a>Обновление schemaExtension

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств в определении указанного ресурса [schemaExtension](../resources/schemaextension.md).

Это обновление применяется ко всем ресурсам, включенным в свойство **targetTypes** расширения. Эти ресурсы входят в число [поддерживаемых](/graph/extensibility-overview#supported-resources).

Только приложение, которое создало расширение схемы (приложение-владелец), может внести дополнения в расширение, причем только тогда, когда расширение находится в состоянии **InDevelopment** или **Available**. Это означает, что приложению не удастся удалить настраиваемые свойства или целевые типы ресурсов из определения. Но приложение может изменить описание расширения.

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
|description|Строка|Описание расширения схемы.|
|properties|Коллекция [extensionSchemaProperty](../resources/extensionschemaproperty.md)|Коллекция имен и типов свойств, составляющих определение расширения схемы. Разрешено вносить изменения только в виде дополнений. |
|status|String|Состояние жизненного цикла расширения схемы. Начальное состояние после создания — **InDevelopment**. Смены состояний: от **InDevelopment** **доступен** и **доступен** для **устарел**.|
|targetTypes|Коллекция String|Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.  Разрешено вносить изменения только в виде дополнений.|

## <a name="response"></a>Отклик

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

##### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 204 No Content
```

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
    "Error: /api-reference/beta/api/schemaextension-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
