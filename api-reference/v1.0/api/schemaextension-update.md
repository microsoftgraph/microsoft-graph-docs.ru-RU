---
title: Обновление schemaExtension
description: Обновление свойств в определении указанной схемыExtension.
ms.localizationpriority: medium
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: d7f73406547770f8c24bbdafc311fd6a1e0a2e36
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764697"
---
# <a name="update-schemaextension"></a>Обновление schemaExtension

Пространство имен: microsoft.graph

Обновление свойств в определении указанной [схемыExtension](../resources/schemaextension.md). 

Это означает, что настраиваемые свойства или типы целевых ресурсов не могут быть удалены из определения, но можно добавить новые настраиваемые свойства и изменить описание расширения.

Присадки к расширению могут быть сделаны только в том случае, если расширение находится в состоянии **InDevelopment** или **Available.** 

Обновление применяется ко всем ресурсам, включенным в **свойство targetTypes** расширения. Эти ресурсы являются одними из [вспомогательных типов ресурсов.](/graph/extensibility-overview#supported-resources)

Для делегирования потоков подписанный пользователь может обновить расширение схемы  до тех пор, пока  свойство владельца расширения задано приложению, владельцем приложения, которое принадлежит подписанного пользователя. Это приложение может быть тем, которое изначально создало расширение, или каким-либо другим приложением, которое принадлежит подписанного пользователя. 

Этот критерий  для свойства владельца позволяет подписанного пользователя делать обновления через другие приложения, которыми они не владеют, например Microsoft Graph Explorer. При использовании Graph Explorer для обновления ресурса **schemaExtension** включаем свойство владельца в тело запроса PATCH.  Дополнительные сведения см. в разделе [Расширения](/graph/known-issues#extensions) в [разделе Известные](/graph/known-issues)проблемы с Microsoft Graph .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Application.ReadWrite.All, Directory.AccessAsUser.All    |
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
|properties|Коллекция [extensionSchemaProperty](../resources/extensionschemaproperty.md)|Коллекция типов и имен свойств, составляющих определение расширения схемы. Разрешены только изменения добавок. |
|status|String|Состояние жизненного цикла расширения схемы. Начальное состояние при создании — **InDevelopment**. Возможные переходы состояния из **InDevelopment** в **доступные и** **доступные** **для deprecated**.|
|targetTypes|Коллекция String|Набор типов Microsoft Graph (поддерживающих расширения), к которым можно применить это расширение схемы.  Разрешены только изменения добавок.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. Попытка выполнить этот запрос из приложения, которым вы не владеете (и  без настройки свойства владельца к приложению приложения, которым вы владеете) возвращает код  `403 Forbidden` ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса. Вы должны включить свойство **владельца,** если вы работаете с запросом из приложения, которым вы не владеете. В этом случае установите свойство **владельца** в **приложение,** которое принадлежит вам.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/schemaExtensions/exto6x7sfft_courses
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
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

