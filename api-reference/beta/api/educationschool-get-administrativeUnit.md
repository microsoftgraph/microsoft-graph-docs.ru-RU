---
title: Получение administrativeUnit
description: Получение простого каталога **administrativeUnit** , соответствующего этому **educationSchool**.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 624a487f12fe851646a8780f942bbe58bf42ddae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007401"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="f3c17-103">Получение administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="f3c17-103">Get administrativeUnit</span></span>

<span data-ttu-id="f3c17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3c17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3c17-105">Получение простого каталога **administrativeUnit** , соответствующего этому **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="f3c17-105">Retrieve the simple directory **administrativeUnit** that corresponds to this **educationSchool**.</span></span>

><span data-ttu-id="f3c17-106">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="f3c17-106">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="f3c17-107">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="f3c17-107">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3c17-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3c17-108">Permissions</span></span>
<span data-ttu-id="f3c17-109">Для вызова этого API требуется сочетание разрешений.</span><span class="sxs-lookup"><span data-stu-id="f3c17-109">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="f3c17-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3c17-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3c17-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3c17-111">Permission type</span></span>      | <span data-ttu-id="f3c17-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3c17-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3c17-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3c17-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="f3c17-114">EduRoster.ReadBasic, EduRoster.Read или EduRoster.Write плюс Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3c17-114">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="f3c17-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3c17-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f3c17-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3c17-116">Not supported.</span></span>  |
|<span data-ttu-id="f3c17-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3c17-117">Application</span></span> | <span data-ttu-id="f3c17-118">EduRoster.Read.All, EduRoster.ReadWrite.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3c17-118">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="f3c17-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3c17-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/administrativeUnit
```
## <a name="request-headers"></a><span data-ttu-id="f3c17-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3c17-120">Request headers</span></span>
| <span data-ttu-id="f3c17-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3c17-121">Header</span></span>       | <span data-ttu-id="f3c17-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3c17-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f3c17-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3c17-123">Authorization</span></span>  | <span data-ttu-id="f3c17-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3c17-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f3c17-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f3c17-126">Request body</span></span>
<span data-ttu-id="f3c17-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3c17-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f3c17-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3c17-128">Response</span></span>
<span data-ttu-id="f3c17-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [administrativeUnit](../resources/administrativeunit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f3c17-129">If successful, this method returns a `200 OK` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f3c17-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f3c17-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3c17-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3c17-131">Request</span></span>
<span data-ttu-id="f3c17-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3c17-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f3c17-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3c17-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_get_administrativeUnit"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/2961761D-8094-4183-A9F6-8E36E966C7D9/administrativeUnit
```
# <a name="c"></a>[<span data-ttu-id="f3c17-134">C#</span><span class="sxs-lookup"><span data-stu-id="f3c17-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f3c17-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3c17-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f3c17-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f3c17-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f3c17-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3c17-137">Response</span></span>
<span data-ttu-id="f3c17-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f3c17-138">The following is an example of the response.</span></span> 

><span data-ttu-id="f3c17-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3c17-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


