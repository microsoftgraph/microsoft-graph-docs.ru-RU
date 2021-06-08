---
title: Добавление учащегося
description: Добавление участника курса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9e0b90e29019eea2e0b232f195017261974bed99
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788089"
---
# <a name="add-a-student"></a><span data-ttu-id="e52da-103">Добавление учащегося</span><span class="sxs-lookup"><span data-stu-id="e52da-103">Add a student</span></span>

<span data-ttu-id="e52da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e52da-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e52da-105">Добавление участника курса.</span><span class="sxs-lookup"><span data-stu-id="e52da-105">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="e52da-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e52da-106">Permissions</span></span>
<span data-ttu-id="e52da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e52da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e52da-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e52da-109">Permission type</span></span>      | <span data-ttu-id="e52da-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e52da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e52da-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e52da-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="e52da-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e52da-112">Not supported.</span></span>  |
|<span data-ttu-id="e52da-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e52da-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e52da-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e52da-114">Not supported.</span></span>  |
|<span data-ttu-id="e52da-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e52da-115">Application</span></span> | <span data-ttu-id="e52da-116">EduRoster.ReadWrite.All plus Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="e52da-116">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e52da-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e52da-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e52da-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e52da-118">Request headers</span></span>
| <span data-ttu-id="e52da-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e52da-119">Header</span></span>       | <span data-ttu-id="e52da-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e52da-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e52da-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e52da-121">Authorization</span></span>  | <span data-ttu-id="e52da-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e52da-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e52da-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e52da-124">Content-Type</span></span>  | <span data-ttu-id="e52da-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e52da-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e52da-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e52da-126">Request body</span></span>
<span data-ttu-id="e52da-127">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e52da-127">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="e52da-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e52da-128">Response</span></span>
<span data-ttu-id="e52da-129">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e52da-129">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e52da-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e52da-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e52da-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e52da-131">Request</span></span>
<span data-ttu-id="e52da-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e52da-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e52da-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e52da-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/13015"
}
```
# <a name="javascript"></a>[<span data-ttu-id="e52da-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e52da-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationclass-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e52da-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e52da-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationclass-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="e52da-136">C#</span><span class="sxs-lookup"><span data-stu-id="e52da-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationclass-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e52da-137">Java</span><span class="sxs-lookup"><span data-stu-id="e52da-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationclass-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e52da-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e52da-138">Response</span></span>
<span data-ttu-id="e52da-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e52da-139">The following is an example of the response.</span></span> 


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

