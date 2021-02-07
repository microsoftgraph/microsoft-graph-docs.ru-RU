---
title: Получение правила
description: Получение свойств и связей объекта messageRule.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8cc1f1a2670761a311993814d59419957857012b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132617"
---
# <a name="get-rule"></a><span data-ttu-id="9063f-103">Получение правила</span><span class="sxs-lookup"><span data-stu-id="9063f-103">Get rule</span></span>

<span data-ttu-id="9063f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9063f-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="9063f-105">Получение свойств и связей объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="9063f-105">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="9063f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9063f-106">Permissions</span></span>
<span data-ttu-id="9063f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9063f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9063f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9063f-109">Permission type</span></span>      | <span data-ttu-id="9063f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9063f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9063f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9063f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9063f-112">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="9063f-112">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="9063f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9063f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9063f-114">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="9063f-114">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="9063f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9063f-115">Application</span></span> | <span data-ttu-id="9063f-116">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="9063f-116">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="9063f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9063f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messageRules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9063f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9063f-118">Optional query parameters</span></span>
<span data-ttu-id="9063f-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9063f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9063f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9063f-120">Request headers</span></span>
| <span data-ttu-id="9063f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9063f-121">Name</span></span>      |<span data-ttu-id="9063f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9063f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9063f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9063f-123">Authorization</span></span>  | <span data-ttu-id="9063f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9063f-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="9063f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9063f-126">Request body</span></span>
<span data-ttu-id="9063f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9063f-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9063f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9063f-128">Response</span></span>
<span data-ttu-id="9063f-129">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9063f-129">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9063f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9063f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9063f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9063f-131">Request</span></span>
<span data-ttu-id="9063f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9063f-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9063f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9063f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZqA="],
  "name": "get_messagerule"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=
```
# <a name="c"></a>[<span data-ttu-id="9063f-134">C#</span><span class="sxs-lookup"><span data-stu-id="9063f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9063f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9063f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9063f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9063f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9063f-137">Java</span><span class="sxs-lookup"><span data-stu-id="9063f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9063f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9063f-138">Response</span></span>
<span data-ttu-id="9063f-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9063f-139">Here is an example of the response.</span></span> <span data-ttu-id="9063f-140">По умолчанию свойства даты и времени в ответе возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="9063f-140">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="9063f-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9063f-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
