---
title: Получение educationSchool
description: Ознакомьтесь с свойствами и отношениями объекта educationSchool.
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 016333f6d5ee367377ff8cd9332969142c165843
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59050581"
---
# <a name="get-educationschool"></a>Получение educationSchool

Пространство имен: microsoft.graph

Ознакомьтесь с свойствами и отношениями объекта [educationSchool.](../resources/educationschool.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | EduRoster.ReadBasic                         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Для приложений                            | EduRoster.Read.All, EduRoster.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools/{educationSchoolId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает те же параметры запроса OData, что [и Get User.](../api/user-get.md#optional-query-parameters) Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationSchool](../resources/educationschool.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{educationSchoolId}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.educationSchool",
    "id": "1c23c12e-c12e-1c23-2ec1-231c2ec1231c",
    "displayName": "String",
    "description": "String",
    "externalSource": "String",
    "externalSourceDetail": "String",
    "principalEmail": "String",
    "principalName": "String",
    "externalPrincipalId": "String",
    "lowestGrade": "String",
    "highestGrade": "String",
    "schoolNumber": "String",
    "externalId": "String",
    "phone": "String",
    "fax": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress"
    }
  }
}
```
