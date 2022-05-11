---
title: Создание accessReview
description: В Azure AD проверки доступа создайте объект accessReview.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bfddca0486d9f622107b4e234c5baa6ab66cbaa0
ms.sourcegitcommit: de9df4bf6313b49afba74b6e9ef819907669c662
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2022
ms.locfileid: "65314542"
---
# <a name="create-accessreview"></a>Создание accessReview

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

В Azure AD [проверки доступа](../resources/accessreviews-root.md) создайте объект [accessReview](../resources/accessreview.md).

Перед выполнением этого запроса вызывающий объект должен получить список шаблонов бизнес-потока [, чтобы](businessflowtemplate-list.md) включить в запрос значение **businessFlowTemplateId** .

После выполнения этого запроса вызывающий объект должен [создать programControl](programcontrol-create.md), чтобы связать проверку доступа с программой.  

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение                            | AccessReview.ReadWrite.Membership |

Вызывающий объект также должен иметь разрешение ProgramControl.ReadWrite.All, чтобы после создания проверки доступа вызывающий объект можно было [создать programControl](../resources/programcontrol.md).
Кроме того, пользователь, выполнив вход, также должен быть в роли каталога, которая позволяет ему создать проверку доступа.  Дополнительные сведения см. в разделе о требованиях к роли и разрешениям для [проверок доступа](../resources/accessreviews-root.md).

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Описание |
|:-------------|:------------|
| Авторизация | Носитель \{токен\}. Обязательный. |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [accessReview в формате](../resources/accessreview.md) JSON.

В следующей таблице показаны свойства, необходимые при создании accessReview.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| displayName             |String                                                        | Имя проверки доступа.  |
| startDateTime           |DateTimeOffset                                                | Дата и время начала проверки.  Это должна быть дата в будущем.   |
| endDateTime             |DateTimeOffset                                                | Дата и время окончания проверки. Это значение должно быть по крайней мере на один день позже даты начала.   |
| description             |String                                                        | Описание, отображаемая рецензентам. |
| businessFlowTemplateId  |String                                                        | Идентификатор шаблона бизнес-потока, полученный из [businessFlowTemplate](../resources/businessflowtemplate.md).  |
| reviewerType            |String                                                        | Тип отношения рецензента с правами доступа проверяемого объекта, один из `self`, `delegated`или `entityOwners`. | 
| reviewedEntity          |[identity](../resources/identity.md)                                     | Объект, для которого создается проверка доступа, например членство в группе или назначение пользователей приложению. | 


Если свойство **reviewerType** `delegated`имеет значение, вызывающий объект также должен включать свойство **рецензентов** с коллекцией объектов [userIdentity](../resources/useridentity.md) , представляющих рецензентов.

Если приложение вызывает этот API без пользователя, выполнившего вход, вызывающий объект также должен включить свойство **createdBy** , значение которого является [userIdentity](../resources/useridentity.md) пользователя, который будет определен как создатель проверки.

Кроме того, вызывающий объект может включать **параметры, чтобы** создать повторяющийся ряд проверок или изменить поведение проверки по умолчанию. В частности, чтобы создать повторяющиеся проверки, вызывающий объект должен включить [accessReviewRecurrenceSettings](../resources/accessreviewrecurrencesettings.md) в параметры проверки доступа.


## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код `201 Created` отклика и объект [accessReview](../resources/accessreview.md) в тексте отклика.

## <a name="example"></a>Пример

Это пример создания однофакторной (не повторяющейся) проверки доступа, явно указав двух пользователей в качестве рецензентов.

### <a name="request"></a>Запрос
В тексте запроса добавьте представление объекта [accessReview в формате](../resources/accessreview.md) JSON.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReview_from_accessReviews"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews
Content-type: application/json

{
    "displayName":"TestReview",
    "startDateTime":"2017-02-10T00:35:53.214Z",
    "endDateTime":"2017-03-12T00:35:53.214Z",
    "reviewedEntity": {
        "id": "99025615-a0b1-47ec-9117-35377b10998b"
    },
    "reviewerType" : "delegated",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "description":"Sample description",
    "reviewers":
    [
        {
            "id":"f260246a-09b1-4fd5-8d18-daed736071ec"
        },
        {
            "id":"5a4e184c-4ee5-4883-96e9-b371f8da88e3"
        }
    ],
    "settings":
    {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval":true,
        "autoReviewEnabled":false,
        "activityDurationInDays":30,
        "autoApplyReviewResultsEnabled":false,
        "accessRecommendationsEnabled":false,
        "recurrenceSettings":{
            "recurrenceType":"onetime",
            "recurrenceEndType":"endBy",
            "durationInDays":0,
            "recurrenceCount":0
        },
        "autoReviewSettings":{
            "notReviewedResult":"Deny"
        }
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreview-from-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreview-from-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreview-from-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreview-from-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-accessreview-from-accessreviews-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-accessreview-from-accessreviews-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


