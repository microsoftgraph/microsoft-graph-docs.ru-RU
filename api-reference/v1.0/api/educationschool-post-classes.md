---
title: Добавление educationClass к educationSchool
description: Добавление класса в учебное заведение.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f3ea3d025e55d9e56bc8488d404ca2c028f3bbb8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517462"
---
# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="802e4-103">Добавление educationClass к educationSchool</span><span class="sxs-lookup"><span data-stu-id="802e4-103">Add educationClass to educationSchool</span></span>

<span data-ttu-id="802e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="802e4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="802e4-105">Добавление класса в учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="802e4-105">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="802e4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="802e4-106">Permissions</span></span>
<span data-ttu-id="802e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="802e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="802e4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="802e4-109">Permission type</span></span>      | <span data-ttu-id="802e4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="802e4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="802e4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="802e4-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="802e4-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="802e4-112">Not supported.</span></span>  |
|<span data-ttu-id="802e4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="802e4-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="802e4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="802e4-114">Not supported.</span></span>  |
|<span data-ttu-id="802e4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="802e4-115">Application</span></span> | <span data-ttu-id="802e4-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="802e4-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="802e4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="802e4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="802e4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="802e4-118">Request headers</span></span>
| <span data-ttu-id="802e4-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="802e4-119">Header</span></span>       | <span data-ttu-id="802e4-120">Значение</span><span class="sxs-lookup"><span data-stu-id="802e4-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="802e4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="802e4-121">Authorization</span></span>  | <span data-ttu-id="802e4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="802e4-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="802e4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="802e4-124">Content-Type</span></span>  | <span data-ttu-id="802e4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="802e4-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="802e4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="802e4-126">Request body</span></span>
<span data-ttu-id="802e4-127">В теле запроса предоставьте описание объекта [educationClass](../resources/educationclass.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="802e4-127">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="802e4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="802e4-128">Response</span></span>
<span data-ttu-id="802e4-129">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="802e4-129">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="802e4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="802e4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="802e4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="802e4-131">Request</span></span>
<span data-ttu-id="802e4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="802e4-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="802e4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="802e4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/v1.0/education/classes/11006"
}
```
# <a name="javascript"></a>[<span data-ttu-id="802e4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="802e4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="802e4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="802e4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="802e4-136">C#</span><span class="sxs-lookup"><span data-stu-id="802e4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="802e4-137">Java</span><span class="sxs-lookup"><span data-stu-id="802e4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="802e4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="802e4-138">Response</span></span> 
<span data-ttu-id="802e4-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="802e4-139">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
