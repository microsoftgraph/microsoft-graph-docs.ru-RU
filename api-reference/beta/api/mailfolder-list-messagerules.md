---
title: Перечисление правил
description: Получение всех объектов messageRule, определенных для папки "Входящие" пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 5f63a6821055c0b3e724ae5d81c278b4f7238a6e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530099"
---
# <a name="list-rules"></a><span data-ttu-id="b7712-103">Перечисление правил</span><span class="sxs-lookup"><span data-stu-id="b7712-103">List rules</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7712-104">Получение всех объектов [messageRule](../resources/messagerule.md), определенных для папки "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="b7712-104">Get all the [messageRule](../resources/messagerule.md) objects defined for the user's Inbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7712-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7712-105">Permissions</span></span>
<span data-ttu-id="b7712-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7712-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7712-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7712-108">Permission type</span></span>      | <span data-ttu-id="b7712-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7712-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7712-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7712-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b7712-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="b7712-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="b7712-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7712-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7712-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="b7712-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="b7712-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7712-114">Application</span></span> | <span data-ttu-id="b7712-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="b7712-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7712-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7712-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b7712-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b7712-117">Optional query parameters</span></span>
<span data-ttu-id="b7712-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b7712-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b7712-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7712-119">Request headers</span></span>
| <span data-ttu-id="b7712-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b7712-120">Name</span></span>       | <span data-ttu-id="b7712-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b7712-121">Type</span></span> | <span data-ttu-id="b7712-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b7712-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b7712-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7712-123">Authorization</span></span>  | <span data-ttu-id="b7712-124">string</span><span class="sxs-lookup"><span data-stu-id="b7712-124">string</span></span>  | <span data-ttu-id="b7712-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7712-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7712-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7712-127">Request body</span></span>
<span data-ttu-id="b7712-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7712-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b7712-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7712-129">Response</span></span>
<span data-ttu-id="b7712-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b7712-130">If successful, this method returns a `200 OK` response code and collection of [messageRule](../resources/messagerule.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7712-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b7712-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7712-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7712-132">Request</span></span>
<span data-ttu-id="b7712-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7712-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messagerules"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/inbox/messagerules
```
##### <a name="response"></a><span data-ttu-id="b7712-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7712-134">Response</span></span>
<span data-ttu-id="b7712-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b7712-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules",
  "value":[
    {
      "id":"AQAAAJ5dZp8=",
      "displayName":"Remove spam",
      "sequence":1,
      "isEnabled":true,
      "hasError":false,
      "isReadOnly":false,
      "conditions":{
        "subjectContains":[
          "enter to win"
        ]
      },
      "actions":{
        "delete":true,
        "stopProcessingRules":true
      }
    },
    {
      "id":"AQAAAJ5dZqA=",
      "displayName":"From partner",
      "sequence":2,
      "isEnabled":true,
      "hasError":false,
      "isReadOnly":false,
      "conditions":{
        "senderContains":[
          "ADELE"
        ]
      },
      "actions":{
        "stopProcessingRules":true,
        "forwardTo":[
          {
            "emailAddress":{
              "name":"Alex Wilbur",
              "address":"AlexW@contoso.onmicrosoft.com"
            }
          }
        ]
      }
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List rules",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-list-messagerules.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
