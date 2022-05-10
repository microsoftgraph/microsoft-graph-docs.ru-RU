---
title: Обновление schemaExtension
description: Обновление свойств в определении указанной схемыExtension.
ms.localizationpriority: medium
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 70f8277e7400c2369adac3da7b03354602e36f33
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296495"
---
# <a name="update-schemaextension"></a>Обновление schemaExtension

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств в определении указанной [схемыExtension](../resources/schemaextension.md). Аддитивные обновления расширения могут выполняться только в том случае, если расширение находится в состоянии `InDevelopment` или состоянии `Available` . Это означает, что пользовательские свойства или типы целевых ресурсов нельзя удалить из определения, но можно добавить новые настраиваемые свойства и изменить описание расширения.

Обновление применяется ко всем ресурсам, включенным в свойство **targetTypes** расширения. Эти ресурсы являются одними из [поддерживаемых типов ресурсов](/graph/extensibility-overview#supported-resources).

Для делегированных потоков пользователь, выполнив вход, может обновить расширение схемы, если для  свойства владельца расширения задано значение **appId** приложения, которое принадлежит вошедему пользователю. Это приложение может быть приложением, которое изначально создало расширение, или другим приложением, принадлежащим вошедему пользователю. 

Этот критерий для  свойства владельца позволяет вошедаму пользователю выполнять обновления через другие приложения, которыми он не владеет, например Microsoft Graph Explorer. При использовании Graph Explorer для обновления **ресурса schemaExtension** включите свойство владельца в текст  запроса PATCH. Дополнительные сведения см. в разделе ["Расширения](/graph/known-issues#extensions)" статьи ["Известные проблемы с microsoft Graph"](/graph/known-issues).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Application.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Application.ReadWrite.All и Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a>Необязательные заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {token}. Обязательный. |
| Content-Type   | application/json |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|description|String|Описание расширения схемы.|
|properties|Коллекция [extensionSchemaProperty](../resources/extensionschemaproperty.md)|Коллекция имен и типов свойств, составляющих определение расширения схемы. Допускаются только аддитивные изменения. |
|status|String|Состояние жизненного цикла расширения схемы. Начальное состояние при создании — `InDevelopment`.. Возможные переходы состояний : " `InDevelopment` в" и `Available` `Available` "в" `Deprecated`.|
|targetTypes|Коллекция String|Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.  Допускаются только аддитивные изменения.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. Попытка выполнить этот запрос из приложения, которым вы не владеете (и без установки свойства владельца на **appId** приложения, которым вы владеете) `403 Forbidden` возвращает код отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса. Если вы выполняете  запрос от приложения, которому вы не владеете, необходимо включить свойство владельца. В этом случае задайте для **свойства владельца** **appId** приложения, которое вы владеете.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/schemaExtensions/exto6x7sfft_courses
Content-type: application/json

{
    "owner": "ef4cb9a8-97c3-4ca7-854b-5cb5ced376fa",
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        },
        {
            "name": "courseSupervisors",
            "type": "String"
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-schemaextension-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-schemaextension-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
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
  ]
}
-->


