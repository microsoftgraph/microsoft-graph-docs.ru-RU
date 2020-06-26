---
title: Вывод группы
description: Получите **группу** Microsoft 365, соответствующую этой **educationClass**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4d77f780d5827c065e7944e1d754d66d48b80002
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895743"
---
# <a name="get-group"></a><span data-ttu-id="b9deb-103">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="b9deb-103">Get group</span></span>

<span data-ttu-id="b9deb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9deb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9deb-105">Получите **группу** Microsoft 365, соответствующую этой **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="b9deb-105">Retrieve the Microsoft 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="b9deb-106">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="b9deb-106">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="b9deb-107">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="b9deb-107">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9deb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9deb-108">Permissions</span></span>
<span data-ttu-id="b9deb-109">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="b9deb-109">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="b9deb-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9deb-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9deb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9deb-111">Permission type</span></span>      | <span data-ttu-id="b9deb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9deb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9deb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9deb-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="b9deb-114">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9deb-114">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="b9deb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9deb-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b9deb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9deb-116">Not supported.</span></span>  |
|<span data-ttu-id="b9deb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b9deb-117">Application</span></span> | <span data-ttu-id="b9deb-118">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9deb-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="b9deb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9deb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="b9deb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9deb-120">Request headers</span></span>
| <span data-ttu-id="b9deb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9deb-121">Header</span></span>       | <span data-ttu-id="b9deb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b9deb-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b9deb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9deb-123">Authorization</span></span>  | <span data-ttu-id="b9deb-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="b9deb-124">Bearer {token}.</span></span> <span data-ttu-id="b9deb-125">Required.</span><span class="sxs-lookup"><span data-stu-id="b9deb-125">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b9deb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9deb-126">Request body</span></span>
<span data-ttu-id="b9deb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9deb-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b9deb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9deb-128">Response</span></span>
<span data-ttu-id="b9deb-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b9deb-129">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9deb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b9deb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9deb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9deb-131">Request</span></span>
<span data-ttu-id="b9deb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9deb-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9deb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9deb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationclass_get_group"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/2961761D-8094-4183-A9F6-8E36E966C7D9/group
```
# <a name="c"></a>[<span data-ttu-id="b9deb-134">C#</span><span class="sxs-lookup"><span data-stu-id="b9deb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationclass-get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9deb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9deb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationclass-get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9deb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9deb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationclass-get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b9deb-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9deb-137">Response</span></span>
<span data-ttu-id="b9deb-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b9deb-138">The following is an example of the response.</span></span> 

><span data-ttu-id="b9deb-139">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="b9deb-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b9deb-140">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b9deb-140">All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
