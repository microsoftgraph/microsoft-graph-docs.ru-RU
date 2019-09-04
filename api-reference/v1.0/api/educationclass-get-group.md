---
title: Вывод группы
description: Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 50cfc3962c04ac525196bda8f3b502eac9255005
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721063"
---
# <a name="get-group"></a><span data-ttu-id="13980-103">Получение группы</span><span class="sxs-lookup"><span data-stu-id="13980-103">Get group</span></span>

<span data-ttu-id="13980-104">Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="13980-104">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="13980-105">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="13980-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="13980-106">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="13980-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="13980-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13980-107">Permissions</span></span>
<span data-ttu-id="13980-108">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="13980-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="13980-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13980-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13980-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13980-110">Permission type</span></span>      | <span data-ttu-id="13980-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13980-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13980-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13980-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="13980-113">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="13980-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="13980-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13980-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="13980-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13980-115">Not supported.</span></span>  |
|<span data-ttu-id="13980-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13980-116">Application</span></span> | <span data-ttu-id="13980-117">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="13980-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="13980-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13980-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="13980-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13980-119">Request headers</span></span>
| <span data-ttu-id="13980-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13980-120">Header</span></span>       | <span data-ttu-id="13980-121">Значение</span><span class="sxs-lookup"><span data-stu-id="13980-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="13980-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13980-122">Authorization</span></span>  | <span data-ttu-id="13980-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13980-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="13980-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="13980-125">Request body</span></span>
<span data-ttu-id="13980-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13980-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="13980-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="13980-127">Response</span></span>
<span data-ttu-id="13980-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="13980-128">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="13980-129">Пример</span><span class="sxs-lookup"><span data-stu-id="13980-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13980-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="13980-130">Request</span></span>
<span data-ttu-id="13980-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13980-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="13980-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="13980-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationclass_get_group"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/group
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="13980-133">C#</span><span class="sxs-lookup"><span data-stu-id="13980-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationclass-get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="13980-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13980-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationclass-get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="13980-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="13980-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationclass-get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="13980-136">Java</span><span class="sxs-lookup"><span data-stu-id="13980-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationclass-get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="13980-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="13980-137">Response</span></span>
<span data-ttu-id="13980-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="13980-138">The following is an example of the response.</span></span> 

><span data-ttu-id="13980-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13980-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
