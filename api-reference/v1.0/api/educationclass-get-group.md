---
title: Вывод группы
description: Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d4af0b3e960e3c3243d3570a7fb0df9706fb4c71
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422248"
---
# <a name="get-group"></a><span data-ttu-id="bdaf1-103">Получение группы</span><span class="sxs-lookup"><span data-stu-id="bdaf1-103">Get group</span></span>

<span data-ttu-id="bdaf1-104">Получение **группы** Office 365, которая соответствует этому объекту **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="bdaf1-104">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="bdaf1-105">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="bdaf1-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="bdaf1-106">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="bdaf1-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdaf1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bdaf1-107">Permissions</span></span>
<span data-ttu-id="bdaf1-108">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="bdaf1-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="bdaf1-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdaf1-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdaf1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdaf1-110">Permission type</span></span>      | <span data-ttu-id="bdaf1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdaf1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdaf1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdaf1-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="bdaf1-113">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdaf1-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="bdaf1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdaf1-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bdaf1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdaf1-115">Not supported.</span></span>  |
|<span data-ttu-id="bdaf1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdaf1-116">Application</span></span> | <span data-ttu-id="bdaf1-117">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdaf1-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="bdaf1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdaf1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="bdaf1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdaf1-119">Request headers</span></span>
| <span data-ttu-id="bdaf1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bdaf1-120">Header</span></span>       | <span data-ttu-id="bdaf1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bdaf1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bdaf1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bdaf1-122">Authorization</span></span>  | <span data-ttu-id="bdaf1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdaf1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bdaf1-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bdaf1-125">Request body</span></span>
<span data-ttu-id="bdaf1-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bdaf1-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bdaf1-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdaf1-127">Response</span></span>
<span data-ttu-id="bdaf1-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bdaf1-128">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bdaf1-129">Пример</span><span class="sxs-lookup"><span data-stu-id="bdaf1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bdaf1-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdaf1-130">Request</span></span>
<span data-ttu-id="bdaf1-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdaf1-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bdaf1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdaf1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationclass_get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/group
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bdaf1-133">C#</span><span class="sxs-lookup"><span data-stu-id="bdaf1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationclass-get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bdaf1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdaf1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationclass-get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bdaf1-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bdaf1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationclass-get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bdaf1-136">Java</span><span class="sxs-lookup"><span data-stu-id="bdaf1-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationclass-get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bdaf1-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdaf1-137">Response</span></span>
<span data-ttu-id="bdaf1-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bdaf1-138">The following is an example of the response.</span></span> 

><span data-ttu-id="bdaf1-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bdaf1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
