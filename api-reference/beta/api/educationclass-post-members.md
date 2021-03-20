---
title: Добавление учащегося
description: Добавление участника курса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 227b53f61c3083b2537d3d64d892c2d9364610f1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951579"
---
# <a name="add-a-student"></a><span data-ttu-id="6f60e-103">Добавление учащегося</span><span class="sxs-lookup"><span data-stu-id="6f60e-103">Add a student</span></span>

<span data-ttu-id="6f60e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f60e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f60e-105">Добавление участника курса.</span><span class="sxs-lookup"><span data-stu-id="6f60e-105">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f60e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f60e-106">Permissions</span></span>
<span data-ttu-id="6f60e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f60e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f60e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f60e-109">Permission type</span></span>      | <span data-ttu-id="6f60e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f60e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f60e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f60e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="6f60e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f60e-112">Not supported.</span></span>  |
|<span data-ttu-id="6f60e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f60e-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6f60e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f60e-114">Not supported.</span></span>  |
|<span data-ttu-id="6f60e-115">Application</span><span class="sxs-lookup"><span data-stu-id="6f60e-115">Application</span></span> | <span data-ttu-id="6f60e-116">EduRoster.ReadWrite.All plus Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="6f60e-116">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6f60e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f60e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="6f60e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f60e-118">Request headers</span></span>
| <span data-ttu-id="6f60e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f60e-119">Header</span></span>       | <span data-ttu-id="6f60e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6f60e-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6f60e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f60e-121">Authorization</span></span>  | <span data-ttu-id="6f60e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f60e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6f60e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6f60e-124">Content-Type</span></span>  | <span data-ttu-id="6f60e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6f60e-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6f60e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f60e-126">Request body</span></span>
<span data-ttu-id="6f60e-127">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f60e-127">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="6f60e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f60e-128">Response</span></span>
<span data-ttu-id="6f60e-129">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6f60e-129">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f60e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6f60e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f60e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f60e-131">Request</span></span>
<span data-ttu-id="6f60e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f60e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6f60e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f60e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass_1"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11011/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/13015"
}
```
# <a name="javascript"></a>[<span data-ttu-id="6f60e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f60e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationclass-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f60e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f60e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationclass-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="6f60e-136">C#</span><span class="sxs-lookup"><span data-stu-id="6f60e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationclass-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f60e-137">Java</span><span class="sxs-lookup"><span data-stu-id="6f60e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationclass-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6f60e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f60e-138">Response</span></span>
<span data-ttu-id="6f60e-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6f60e-139">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


