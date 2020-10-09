---
title: Получение правила
description: Получение свойств и связей объекта messageRule.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 57ce155c0c096511f3c268e5a38cf95ceccde598
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402415"
---
# <a name="get-rule"></a><span data-ttu-id="72c6a-103">Получение правила</span><span class="sxs-lookup"><span data-stu-id="72c6a-103">Get rule</span></span>

<span data-ttu-id="72c6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72c6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72c6a-105">Получение свойств и связей объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="72c6a-105">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="72c6a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72c6a-106">Permissions</span></span>
<span data-ttu-id="72c6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72c6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72c6a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72c6a-109">Permission type</span></span>      | <span data-ttu-id="72c6a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72c6a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72c6a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72c6a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="72c6a-112">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="72c6a-112">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="72c6a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72c6a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72c6a-114">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="72c6a-114">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="72c6a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72c6a-115">Application</span></span> | <span data-ttu-id="72c6a-116">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="72c6a-116">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="72c6a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72c6a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="72c6a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="72c6a-118">Optional query parameters</span></span>
<span data-ttu-id="72c6a-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="72c6a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72c6a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72c6a-120">Request headers</span></span>
| <span data-ttu-id="72c6a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="72c6a-121">Name</span></span>      |<span data-ttu-id="72c6a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="72c6a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="72c6a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72c6a-123">Authorization</span></span>  | <span data-ttu-id="72c6a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72c6a-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="72c6a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72c6a-126">Request body</span></span>
<span data-ttu-id="72c6a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72c6a-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="72c6a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="72c6a-128">Response</span></span>
<span data-ttu-id="72c6a-129">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="72c6a-129">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="72c6a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="72c6a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72c6a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="72c6a-131">Request</span></span>
<span data-ttu-id="72c6a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72c6a-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72c6a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="72c6a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messagerule"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')
```
# <a name="c"></a>[<span data-ttu-id="72c6a-134">C#</span><span class="sxs-lookup"><span data-stu-id="72c6a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72c6a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72c6a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72c6a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72c6a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="72c6a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="72c6a-137">Response</span></span>
<span data-ttu-id="72c6a-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="72c6a-138">Here is an example of the response.</span></span> <span data-ttu-id="72c6a-139">По умолчанию свойства даты и времени в ответе возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="72c6a-139">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="72c6a-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72c6a-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->