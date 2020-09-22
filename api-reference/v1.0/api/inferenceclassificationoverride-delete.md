---
title: Удаление объекта inferenceClassificationOverride
description: Удаление переопределения по идентификатору.
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: f9a08903a7e96f7ab06bfea66b1058b7f393b696
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033358"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="28281-103">Удаление объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="28281-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="28281-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28281-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28281-105">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="28281-105">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="28281-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28281-106">Permissions</span></span>
<span data-ttu-id="28281-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28281-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28281-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28281-109">Permission type</span></span>      | <span data-ttu-id="28281-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28281-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28281-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28281-111">Delegated (work or school account)</span></span> | <span data-ttu-id="28281-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28281-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="28281-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28281-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28281-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28281-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="28281-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28281-115">Application</span></span> | <span data-ttu-id="28281-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28281-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="28281-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28281-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="28281-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28281-118">Request headers</span></span>
| <span data-ttu-id="28281-119">Имя</span><span class="sxs-lookup"><span data-stu-id="28281-119">Name</span></span>       | <span data-ttu-id="28281-120">Тип</span><span class="sxs-lookup"><span data-stu-id="28281-120">Type</span></span> | <span data-ttu-id="28281-121">Описание</span><span class="sxs-lookup"><span data-stu-id="28281-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="28281-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28281-122">Authorization</span></span>  | <span data-ttu-id="28281-123">string</span><span class="sxs-lookup"><span data-stu-id="28281-123">string</span></span>  | <span data-ttu-id="28281-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28281-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28281-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="28281-126">Request body</span></span>
<span data-ttu-id="28281-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28281-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28281-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="28281-128">Response</span></span>

<span data-ttu-id="28281-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="28281-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28281-131">Пример</span><span class="sxs-lookup"><span data-stu-id="28281-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28281-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="28281-132">Request</span></span>
<span data-ttu-id="28281-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28281-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28281-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="28281-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
# <a name="c"></a>[<span data-ttu-id="28281-135">C#</span><span class="sxs-lookup"><span data-stu-id="28281-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28281-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28281-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28281-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28281-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28281-138">Java</span><span class="sxs-lookup"><span data-stu-id="28281-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-inferenceclassificationoverride-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28281-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="28281-139">Response</span></span>
<span data-ttu-id="28281-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28281-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

