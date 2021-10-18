---
title: Обновление subjectRightsRequest
description: Обновление свойств объекта subjectRightsRequest.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 9b7e10be0d5fd0eb99170aee4d77ba9feda39a70
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60448013"
---
# <a name="update-subjectrightsrequest"></a>Обновление subjectRightsRequest
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [subjectRightsRequest.](../resources/subjectRightsRequest.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|SubjectRightsRequest.ReadWrite.All*|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается|

>[!IMPORTANT]
>Разрешения, отмеченные звездочкой (*), в настоящее время недоступны. Дополнительные сведения см. в статье [Известные проблемы](/graph/known-issues#compliance).

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /privacy/subjectRightsRequests/{subjectRightsRequestId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [subjectRightsRequest.](../resources/subjectRightsRequest.md)

В следующей таблице показаны свойства, необходимые при обновлении [subjectRightsRequest.](../resources/subjectRightsRequest.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|assignedTo|[microsoft.graph.identity](../resources/identity.md)|Сведения о удостоверениях пользователя, на который назначен запрос.|
|description|String|Обновленное описание запроса.|
|displayName|String|Обновленное имя запроса.|
|internalDueDateTime|DateTimeOffset|Обновлена внутренняя дата задатки запроса.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект subjectRightsRequest](../resources/subjectRightsRequest.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "update_subjectRightsRequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/privacy/subjectRightsRequests/{subjectRightsRequestId}
Content-Type: application/json
Content-length: 837

{
  "@odata.type": "#microsoft.graph.subjectRightsRequest",
  "internalDueDateTime": "2021-08-30T00:00:00Z"
}
```

### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subjectRightsRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "type": "microsoft.graph.subjectRightsRequestType",
    "dataSubjectType": "microsoft.graph.dataSubjectType",
    "regulations": [
        "String"
    ],
    "displayName": "String",
    "description": "String",
    "status": "active",
    "internalDueDateTime": "String",
    "lastModifiedDateTime": "String",
    "id": "String",
    "createdDateTime": "String",
    "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
    },
    "dataSubject": {
        "firstName": "String",
        "lastName": "String",
        "email": "String",
        "residency": "String",
        "phoneNumber": "String",
        "SSN": "String"
    },
    "team": {
        "id": "String (identifier)",
        "webUrl": "String"
    }
}
```

