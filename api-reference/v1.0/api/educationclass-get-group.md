---
title: Вывод группы
description: Извлечение Microsoft 365 **группы,** соответствующей **данному классу educationClass.**
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6439e460bcd1e32780540de4bce3f36d432c75a0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035570"
---
# <a name="get-group"></a><span data-ttu-id="943ee-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="943ee-103">Get group</span></span>

<span data-ttu-id="943ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="943ee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="943ee-105">Извлечение Microsoft 365 **группы,** соответствующей **данному классу educationClass.**</span><span class="sxs-lookup"><span data-stu-id="943ee-105">Retrieve the Microsoft 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="943ee-106">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="943ee-106">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="943ee-107">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="943ee-107">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="943ee-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="943ee-108">Permissions</span></span>
<span data-ttu-id="943ee-109">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="943ee-109">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="943ee-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="943ee-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="943ee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="943ee-111">Permission type</span></span>      | <span data-ttu-id="943ee-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="943ee-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="943ee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="943ee-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="943ee-114">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="943ee-114">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="943ee-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="943ee-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="943ee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="943ee-116">Not supported.</span></span>  |
|<span data-ttu-id="943ee-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="943ee-117">Application</span></span> | <span data-ttu-id="943ee-118">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="943ee-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="943ee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="943ee-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="943ee-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="943ee-120">Request headers</span></span>
| <span data-ttu-id="943ee-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="943ee-121">Header</span></span>       | <span data-ttu-id="943ee-122">Значение</span><span class="sxs-lookup"><span data-stu-id="943ee-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="943ee-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="943ee-123">Authorization</span></span>  | <span data-ttu-id="943ee-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="943ee-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="943ee-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="943ee-126">Request body</span></span>
<span data-ttu-id="943ee-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="943ee-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="943ee-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="943ee-128">Response</span></span>
<span data-ttu-id="943ee-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="943ee-129">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="943ee-130">Пример</span><span class="sxs-lookup"><span data-stu-id="943ee-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="943ee-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="943ee-131">Request</span></span>
<span data-ttu-id="943ee-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="943ee-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="943ee-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="943ee-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationclass_get_group"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/group
```
# <a name="c"></a>[<span data-ttu-id="943ee-134">C#</span><span class="sxs-lookup"><span data-stu-id="943ee-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationclass-get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="943ee-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="943ee-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationclass-get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="943ee-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="943ee-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationclass-get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="943ee-137">Java</span><span class="sxs-lookup"><span data-stu-id="943ee-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationclass-get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="943ee-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="943ee-138">Response</span></span>
<span data-ttu-id="943ee-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="943ee-139">The following is an example of the response.</span></span> 

><span data-ttu-id="943ee-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="943ee-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

<!-- uuid: 0087D9B3-1418-4C87-91C9-A18C6D93706B
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

