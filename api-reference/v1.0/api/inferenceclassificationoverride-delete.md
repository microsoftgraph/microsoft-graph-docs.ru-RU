---
title: Удаление объекта inferenceClassificationOverride
description: Удаление переопределения по идентификатору.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 81b2c7b733078753eb51141cb6e970da91ef0b06
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016148"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="c862d-103">Удаление объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="c862d-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="c862d-104">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="c862d-104">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="c862d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c862d-105">Permissions</span></span>
<span data-ttu-id="c862d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c862d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c862d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c862d-108">Permission type</span></span>      | <span data-ttu-id="c862d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c862d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c862d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c862d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c862d-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c862d-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c862d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c862d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c862d-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c862d-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c862d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c862d-114">Application</span></span> | <span data-ttu-id="c862d-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c862d-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c862d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c862d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c862d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c862d-117">Request headers</span></span>
| <span data-ttu-id="c862d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c862d-118">Name</span></span>       | <span data-ttu-id="c862d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c862d-119">Type</span></span> | <span data-ttu-id="c862d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c862d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c862d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c862d-121">Authorization</span></span>  | <span data-ttu-id="c862d-122">string</span><span class="sxs-lookup"><span data-stu-id="c862d-122">string</span></span>  | <span data-ttu-id="c862d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c862d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c862d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c862d-125">Request body</span></span>
<span data-ttu-id="c862d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c862d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c862d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c862d-127">Response</span></span>

<span data-ttu-id="c862d-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c862d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c862d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c862d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c862d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c862d-131">Request</span></span>
<span data-ttu-id="c862d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c862d-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c862d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c862d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c862d-134">C#</span><span class="sxs-lookup"><span data-stu-id="c862d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c862d-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="c862d-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c862d-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c862d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c862d-137">Java</span><span class="sxs-lookup"><span data-stu-id="c862d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-inferenceclassificationoverride-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c862d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c862d-138">Response</span></span>
<span data-ttu-id="c862d-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c862d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
