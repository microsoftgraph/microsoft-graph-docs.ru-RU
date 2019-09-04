---
title: Получение administrativeUnit
description: Получение простого каталога **administrativeUnit** , соответствующего этому **educationSchool**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6707717bf7cf3e98eabdb400d2d677c2e98b73fd
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720391"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="b98ab-103">Получение administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="b98ab-103">Get administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b98ab-104">Получение простого каталога **administrativeUnit** , соответствующего этому **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="b98ab-104">Retrieve the simple directory **administrativeUnit** that corresponds to this **educationSchool**.</span></span>

><span data-ttu-id="b98ab-105">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="b98ab-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="b98ab-106">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="b98ab-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="b98ab-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b98ab-107">Permissions</span></span>
<span data-ttu-id="b98ab-108">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="b98ab-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="b98ab-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b98ab-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b98ab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b98ab-110">Permission type</span></span>      | <span data-ttu-id="b98ab-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b98ab-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b98ab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b98ab-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="b98ab-113">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b98ab-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="b98ab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b98ab-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b98ab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b98ab-115">Not supported.</span></span>  |
|<span data-ttu-id="b98ab-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b98ab-116">Application</span></span> | <span data-ttu-id="b98ab-117">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b98ab-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="b98ab-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b98ab-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/administrativeUnit
```
## <a name="request-headers"></a><span data-ttu-id="b98ab-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b98ab-119">Request headers</span></span>
| <span data-ttu-id="b98ab-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b98ab-120">Header</span></span>       | <span data-ttu-id="b98ab-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b98ab-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b98ab-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b98ab-122">Authorization</span></span>  | <span data-ttu-id="b98ab-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b98ab-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b98ab-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b98ab-125">Request body</span></span>
<span data-ttu-id="b98ab-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b98ab-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b98ab-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b98ab-127">Response</span></span>
<span data-ttu-id="b98ab-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [administrativeUnit](../resources/administrativeunit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b98ab-128">If successful, this method returns a `200 OK` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b98ab-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b98ab-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b98ab-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b98ab-130">Request</span></span>
<span data-ttu-id="b98ab-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b98ab-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b98ab-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b98ab-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_get_administrativeUnit"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/2961761D-8094-4183-A9F6-8E36E966C7D9/administrativeUnit
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b98ab-133">C#</span><span class="sxs-lookup"><span data-stu-id="b98ab-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b98ab-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b98ab-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b98ab-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b98ab-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b98ab-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b98ab-136">Response</span></span>
<span data-ttu-id="b98ab-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b98ab-137">The following is an example of the response.</span></span> 

><span data-ttu-id="b98ab-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b98ab-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

<!-- uuid: A681726F-B4A7-4BCF-9407-F87CB9A4771D
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
