---
title: Создание authoredNote
description: Создание нового объекта authoredNote.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 783384d3f762f01b773a585cfab79b3d9dbdb342
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561810"
---
# <a name="create-authorednote"></a>Создание authoredNote
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового [объекта authoredNote.](../resources/authorednote.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|SubjectRightsRequest.ReadWrite.All*|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|Не поддерживается|

>[!IMPORTANT]
>Разрешения, отмеченные звездочкой (*), в настоящее время недоступны. Дополнительные сведения см. в статье [Известные проблемы](/graph/known-issues#compliance).

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /privacy/subjectRightsRequests/{subjectRightsRequestId}/notes
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [authoredNote.](../resources/authorednote.md)

В следующей таблице показаны свойства, необходимые при создании [authoredNote.](../resources/authorednote.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|content|[microsoft.graph.itemBody](../resources/itembody.md)|Содержимое заметки для запроса|


## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект authoredNote](../resources/authorednote.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_authorednote_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/privacy/subjectRightsRequests/{subjectRightsRequestId}/notes
Content-Type: application/json
Content-length: 203

{
"content": 
  {
    "content": "String",
    "contentType": "text"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-authorednote-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-authorednote-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-authorednote-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-authorednote-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authoredNote"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "id": "String (identifier)",
    "createdDateTime": "String (timestamp)",
    "author": { "@odata.type": "microsoft.graph.identitySet"},
    "content": {
          "@odata.type": "microsoft.graph.itemBody"
    }

}
```

