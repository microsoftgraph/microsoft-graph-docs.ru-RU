---
title: Обновление реинтеграции рабочей силы
description: Обновление свойств объекта по реинтеграции рабочей силы.
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0786f0a80825b77cd5021ad1c978bdf053aa9c16
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101964"
---
# <a name="update-workforceintegration"></a>Обновление реинтеграции рабочей силы

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [по реинтеграции](../resources/workforceintegration.md) рабочей силы.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | WorkforceIntegration.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация | Bearer {token} |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|apiVersion|Int32|Версия API для URL-адреса обратного вызова. Начните с 1.|
|displayName|String|Имя интеграции рабочей силы.|
|шифрование|workforceIntegrationEncryption|Ресурс шифрования интеграции рабочей силы. |
|isActive|Логический|Указывает, является ли эта интеграция рабочей силы активной и доступной в настоящее время.|
|поддерживает|string| Возможные значения `none` , , , , `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` . Если выбрано несколько значений, все значения должны начинаться с первой буквы в верхнем шкафу.|
|supportedEntities|string| Это свойство заменит **поддержки** в v1.0. Рекомендуется использовать это свойство вместо **поддержки.** Свойство **поддерживается** в бета-версии в настоящее время. Возможные значения `none` , , , , `shift` `swapRequest` `openshift` `openShiftRequest` `userShiftPreferences` . Если выбрано несколько значений, все значения должны начинаться с первой буквы в верхнем шкафу.|
|url|String| URL-адрес интеграции рабочей силы для вызовов из службы Shift. |

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [workforceIntegration](../resources/workforceintegration.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-update-a-workforceintegration-object"></a>Пример 1. Обновление объекта workforceIntegration

В следующем примере обновляется **объект workforceIntegration.**

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_workforceintegration"
}-->

```http
PATCH https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceIntegrationId}
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-workforceintegration-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-workforceintegration-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```

### <a name="example-2-create-a-new-workforceintegration-with-swaprequest-enabled-for-eligibility-filtering"></a>Пример 2. Создание новой рабочей силыИнтеграция с помощью SwapRequest, включенной для фильтрации прав

В следующем примере создается новая **рабочая силаИнтеграция** с поддержкой SwapRequest для фильтрации прав.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса. 
```
POST https://graph.microsoft.com/beta/teamwork/workforceIntegrations/
Authorization: Bearer {token}
Content-type: application/json

{
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": "My Secret"
  },
  "url": "https://ABCWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}

```
#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
```
HTTP/1.1 200 OK
{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "ABCWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://abcWorkforceIntegration.com/Contoso/",
  "supports": "Shift,SwapRequest",
  "eligibilityFilteringEnabledEntities": "SwapRequest"
}

```
Чтобы создать новую **рабочую силуИнтеграция** с помощью SwapRequest, включенной для фильтрации прав, см. в [методе Create.](../api/workforceintegration-post.md)

### <a name="example-3-fetching-eligible-shifts-when-swaprequest-is-included-in-eligibilityfilteringenabledentities"></a>Пример 3. Получение подходящих сдвигов при включении SwapRequest в eligibilityFilteringEnabledEntities

Взаимодействие между конечными точками интеграции shifts и рабочей силой будет следовать существующему шаблону.

#### <a name="request"></a>Запрос

Ниже приводится пример запроса shifts to the workforce integration endpoint to fetch eligible shifts for a swap request.

```
POST https://abcWorkforceIntegration.com/Contoso/{apiVersion}/team/{teamId}/read
Accept-Language: en-us

{
  "requests": [
  {
     "id": "{shiftId}",
     "method": "GET”,
     "url": “/shifts/{shiftId}/requestableShifts?requestType={requestType}&startDateTime={startDateTime}&endDateTime={endDateTime}”
   }]
}
```
#### <a name="response"></a>Отклик

Ниже приводится пример ответа службы интеграции рабочей силы.
```
HTTP/1.1 200 OK
{
  "responses": [
  {
    "body": {
      "SHFT_6548f642-cbc1-4228-8621-054327576457",
      "SHFT_6548f642-cbc1-4228-8621-054327571234"
  }
    "id": "{shiftId}",
    "status: 200,
    "body": {
       "data": [{ShiftId}, {ShiftId}...]
       "error": null
    }
  ]
}
```

### <a name="example-4-shifts-synchronous-call-back-to-the-workforce-integration-endpoint-when-enabled-for-real-time-notifications-on-timecard-changes"></a>Пример 4. Перенос синхронного вызова обратно в конечную точку интеграции рабочей силы при включении уведомлений в режиме реального времени при изменениях timeCard.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса. 
```
POST https://foobarWorkforceIntegration.com/foobar/v1/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/update
Accept-Language: en-us
X-MS-WFMPassthrough: foobarvalue
Content-type: application/json
{
   "requests":[
      {
         "id":"1",
         "method":"POST",
         "url":"/timecards",
         "headers":{
            "X-MS-Transaction-ID":"1"
         },
         "body":{
            "id":"3895809b-a618-4c0d-86a0-d42b25b7d74f",
            "userId":"a3601044-a1b5-438e-b742-f78d01d68a67",
            "createdDateTime":"2019-03-18T00:00:00.000Z",
            "createdBy":{
               "user":{
                  "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
                  "displayName":"Dwight Schrute"
               }
            },
            "lastModifiedDateTime":"2019-03-18T00:00:00.000Z",
            "lastModifiedBy":{
               "user":{
                  "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
                  "displayName":"Dwight Schrute"
               }
            },
            "state":"onBreak",
            "clockIn":{
               "dateTime":"2019-03-18T00:00:00.000Z",
               "atApprovedLocation":true,
               "notes":null
            },
            "clockOut":null,
            "breaks":[
               {
                  "id":"string",
                  "notes":{
                     "content":"Lunch break",
                     "contentType":"text"
                  },
                  "start":{
                     "dateTime":"2019-03-18T00:00:00.000Z",
                     "atApprovedLocation":true,
                     "notes":{
                        "content":"Started my break 5 minutes early",
                        "contentType":"text"
                     }
                  },
                  "end":null
               }
            ],
            "notes":null,
            "originalEntry":{
               "clockIn":{
                  "dateTime":"2019-03-18T00:00:00.000Z",
                  "atApprovedLocation":true,
                  "notes":null
               },
               "clockOut":null,
               "breaks":[
                  {
                     "id":"4591109b-a618-3e0d-e6a0-d42b25b7231f",
                     "notes":{
                        "content":"Lunch break",
                        "contentType":"text"
                     },
                     "start":{
                        "dateTime":"2019-03-18T00:00:00.000Z",
                        "atApprovedLocation":true,
                        "notes":{
                           "content":"Started my break 5 minutes early",
                           "contentType":"text"
                        }
                     },
                     "end":null
                  }
               ]
            }
         }
      }
   ]
}

```
#### <a name="response"></a>Отклик

Ниже приведен пример ответа.
```
HTTP/1.1 200 OK
Content-type: application/json
{
  "responses":[
    {
      "id": "1",
      "status": 200,
      "body":{
        "eTag": "4000ee23-0000-0700-0000-5d1415f60000",
        "error": null
      }
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update workforceintegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


