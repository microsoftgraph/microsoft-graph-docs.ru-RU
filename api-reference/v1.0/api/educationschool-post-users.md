---
title: Добавление educationUser в educationSchool
description: Добавление пользователя в учебное заведение.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ee59a78c572344f105d4826c4312626e85c3b25e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783633"
---
# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="36f0c-103">Добавление educationUser в educationSchool</span><span class="sxs-lookup"><span data-stu-id="36f0c-103">Add educationUser to an educationSchool</span></span>

<span data-ttu-id="36f0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36f0c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36f0c-105">Добавление пользователя в учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="36f0c-105">Add a user to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="36f0c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36f0c-106">Permissions</span></span>
<span data-ttu-id="36f0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36f0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36f0c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36f0c-109">Permission type</span></span>      | <span data-ttu-id="36f0c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36f0c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36f0c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36f0c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="36f0c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36f0c-112">Not supported.</span></span>  |
|<span data-ttu-id="36f0c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36f0c-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="36f0c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36f0c-114">Not supported.</span></span>  |
|<span data-ttu-id="36f0c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36f0c-115">Application</span></span> | <span data-ttu-id="36f0c-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36f0c-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="36f0c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36f0c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```
## <a name="request-headers"></a><span data-ttu-id="36f0c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36f0c-118">Request headers</span></span>
| <span data-ttu-id="36f0c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36f0c-119">Header</span></span>       | <span data-ttu-id="36f0c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="36f0c-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="36f0c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36f0c-121">Authorization</span></span>  | <span data-ttu-id="36f0c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36f0c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="36f0c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="36f0c-124">Content-Type</span></span>  | <span data-ttu-id="36f0c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36f0c-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36f0c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="36f0c-126">Request body</span></span>
<span data-ttu-id="36f0c-127">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36f0c-127">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="36f0c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="36f0c-128">Response</span></span>
<span data-ttu-id="36f0c-129">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="36f0c-129">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36f0c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="36f0c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36f0c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="36f0c-131">Request</span></span>
<span data-ttu-id="36f0c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36f0c-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="36f0c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="36f0c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools/{id}/users/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/14008"
}
```
# <a name="javascript"></a>[<span data-ttu-id="36f0c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36f0c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36f0c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36f0c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="36f0c-136">C#</span><span class="sxs-lookup"><span data-stu-id="36f0c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36f0c-137">Java</span><span class="sxs-lookup"><span data-stu-id="36f0c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="36f0c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="36f0c-138">Response</span></span>
<span data-ttu-id="36f0c-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="36f0c-139">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

