---
title: Получение правила
description: Получение свойств и связей объекта messageRule.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: bbc7265346b3c9f99d0bf5ab4678b107050806e7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978776"
---
# <a name="get-rule"></a><span data-ttu-id="a8253-103">Получение правила</span><span class="sxs-lookup"><span data-stu-id="a8253-103">Get rule</span></span>


<span data-ttu-id="a8253-104">Получение свойств и связей объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="a8253-104">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="a8253-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8253-105">Permissions</span></span>
<span data-ttu-id="a8253-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8253-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8253-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8253-108">Permission type</span></span>      | <span data-ttu-id="a8253-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8253-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8253-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8253-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a8253-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="a8253-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="a8253-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8253-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8253-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="a8253-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="a8253-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8253-114">Application</span></span> | <span data-ttu-id="a8253-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="a8253-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8253-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8253-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a8253-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a8253-117">Optional query parameters</span></span>
<span data-ttu-id="a8253-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a8253-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8253-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8253-119">Request headers</span></span>
| <span data-ttu-id="a8253-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a8253-120">Name</span></span>      |<span data-ttu-id="a8253-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a8253-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a8253-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8253-122">Authorization</span></span>  | <span data-ttu-id="a8253-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8253-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="a8253-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a8253-125">Request body</span></span>
<span data-ttu-id="a8253-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8253-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a8253-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8253-127">Response</span></span>
<span data-ttu-id="a8253-128">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a8253-128">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a8253-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a8253-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8253-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8253-130">Request</span></span>
<span data-ttu-id="a8253-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8253-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZqA="],
  "name": "get_messagerule"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=
```
##### <a name="response"></a><span data-ttu-id="a8253-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8253-132">Response</span></span>
<span data-ttu-id="a8253-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a8253-133">Here is an example of the response.</span></span> <span data-ttu-id="a8253-134">По умолчанию свойства даты и времени в ответе возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="a8253-134">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="a8253-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8253-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
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
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
