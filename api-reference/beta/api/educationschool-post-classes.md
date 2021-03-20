---
title: Добавление educationClass к educationSchool
description: Добавление класса в учебное заведение.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 72a856314cec6ffed375bd14f1899aebf9256e8b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951320"
---
# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="a5515-103">Добавление educationClass к educationSchool</span><span class="sxs-lookup"><span data-stu-id="a5515-103">Add educationClass to educationSchool</span></span>

<span data-ttu-id="a5515-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5515-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5515-105">Добавление класса в учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="a5515-105">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5515-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5515-106">Permissions</span></span>
<span data-ttu-id="a5515-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5515-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5515-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5515-109">Permission type</span></span>      | <span data-ttu-id="a5515-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5515-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5515-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5515-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="a5515-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5515-112">Not supported.</span></span>  |
|<span data-ttu-id="a5515-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5515-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a5515-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5515-114">Not supported.</span></span>  |
|<span data-ttu-id="a5515-115">Application</span><span class="sxs-lookup"><span data-stu-id="a5515-115">Application</span></span> | <span data-ttu-id="a5515-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5515-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a5515-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5515-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="a5515-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5515-118">Request headers</span></span>
| <span data-ttu-id="a5515-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5515-119">Header</span></span>       | <span data-ttu-id="a5515-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a5515-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a5515-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5515-121">Authorization</span></span>  | <span data-ttu-id="a5515-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5515-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a5515-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5515-124">Content-Type</span></span>  | <span data-ttu-id="a5515-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5515-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5515-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5515-126">Request body</span></span>
<span data-ttu-id="a5515-127">В теле запроса предоставьте описание объекта [educationClass](../resources/educationclass.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5515-127">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="a5515-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5515-128">Response</span></span>
<span data-ttu-id="a5515-129">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a5515-129">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5515-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a5515-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5515-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5515-131">Request</span></span>
<span data-ttu-id="a5515-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5515-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5515-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5515-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool_5"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools/10002/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/beta/education/classes/11006"
}
```
# <a name="javascript"></a>[<span data-ttu-id="a5515-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5515-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5515-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5515-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="a5515-136">C#</span><span class="sxs-lookup"><span data-stu-id="a5515-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5515-137">Java</span><span class="sxs-lookup"><span data-stu-id="a5515-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a5515-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5515-138">Response</span></span> 
<span data-ttu-id="a5515-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a5515-139">The following is an example of the response.</span></span> 

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
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


