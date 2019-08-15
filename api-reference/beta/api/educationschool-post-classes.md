---
title: Добавление educationClass к educationSchool
description: Добавление класса в учебное заведение.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 10b68bbad43fb0cc107d76f27f49ff0fd9b9442d
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416123"
---
# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="7a235-103">Добавление educationClass к educationSchool</span><span class="sxs-lookup"><span data-stu-id="7a235-103">Add educationClass to educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a235-104">Добавление класса в учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="7a235-104">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a235-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a235-105">Permissions</span></span>
<span data-ttu-id="7a235-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a235-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a235-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a235-108">Permission type</span></span>      | <span data-ttu-id="7a235-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a235-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a235-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a235-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7a235-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a235-111">Not supported.</span></span>  |
|<span data-ttu-id="7a235-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a235-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7a235-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a235-113">Not supported.</span></span>  |
|<span data-ttu-id="7a235-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a235-114">Application</span></span> | <span data-ttu-id="7a235-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a235-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7a235-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a235-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7a235-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a235-117">Request headers</span></span>
| <span data-ttu-id="7a235-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a235-118">Header</span></span>       | <span data-ttu-id="7a235-119">Значение</span><span class="sxs-lookup"><span data-stu-id="7a235-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7a235-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a235-120">Authorization</span></span>  | <span data-ttu-id="7a235-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a235-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7a235-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a235-123">Content-Type</span></span>  | <span data-ttu-id="7a235-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7a235-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7a235-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7a235-125">Request body</span></span>
<span data-ttu-id="7a235-126">В теле запроса предоставьте описание объекта [educationClass](../resources/educationclass.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a235-126">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="7a235-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a235-127">Response</span></span>
<span data-ttu-id="7a235-128">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7a235-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a235-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7a235-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a235-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a235-130">Request</span></span>
<span data-ttu-id="7a235-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a235-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7a235-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a235-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools/10002/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/beta/education/classes/11006"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a235-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a235-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7a235-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7a235-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="7a235-135">C#</span><span class="sxs-lookup"><span data-stu-id="7a235-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7a235-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a235-136">Response</span></span> 
<span data-ttu-id="7a235-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7a235-137">The following is an example of the response.</span></span> 

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
