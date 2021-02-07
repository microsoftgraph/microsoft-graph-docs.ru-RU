---
title: Удаление объекта inferenceClassificationOverride
description: Удаление переопределения по идентификатору.
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 9c2f482ea1b7feb5db8895f4031f887500c54efa
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133863"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="6b53f-103">Удаление объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="6b53f-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="6b53f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b53f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b53f-105">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="6b53f-105">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b53f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b53f-106">Permissions</span></span>
<span data-ttu-id="6b53f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b53f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b53f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b53f-109">Permission type</span></span>      | <span data-ttu-id="6b53f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b53f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b53f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b53f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b53f-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b53f-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6b53f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b53f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b53f-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b53f-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6b53f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b53f-115">Application</span></span> | <span data-ttu-id="6b53f-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b53f-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b53f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b53f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6b53f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b53f-118">Request headers</span></span>
| <span data-ttu-id="6b53f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6b53f-119">Name</span></span>       | <span data-ttu-id="6b53f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="6b53f-120">Type</span></span> | <span data-ttu-id="6b53f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6b53f-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6b53f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b53f-122">Authorization</span></span>  | <span data-ttu-id="6b53f-123">string</span><span class="sxs-lookup"><span data-stu-id="6b53f-123">string</span></span>  | <span data-ttu-id="6b53f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b53f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b53f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b53f-126">Request body</span></span>
<span data-ttu-id="6b53f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6b53f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b53f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b53f-128">Response</span></span>

<span data-ttu-id="6b53f-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6b53f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b53f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6b53f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b53f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b53f-132">Request</span></span>
<span data-ttu-id="6b53f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b53f-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b53f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b53f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
# <a name="c"></a>[<span data-ttu-id="6b53f-135">C#</span><span class="sxs-lookup"><span data-stu-id="6b53f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b53f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b53f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b53f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b53f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b53f-138">Java</span><span class="sxs-lookup"><span data-stu-id="6b53f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-inferenceclassificationoverride-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6b53f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b53f-139">Response</span></span>
<span data-ttu-id="6b53f-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b53f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

