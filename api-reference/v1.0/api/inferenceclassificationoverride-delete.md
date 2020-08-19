---
title: Удаление объекта inferenceClassificationOverride
description: Удаление переопределения по идентификатору.
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: dccd9fe08f62ecdff65f2f5d5437f9f8472f2ba2
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806165"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="4599e-103">Удаление объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="4599e-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="4599e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4599e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4599e-105">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="4599e-105">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="4599e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4599e-106">Permissions</span></span>
<span data-ttu-id="4599e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4599e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4599e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4599e-109">Permission type</span></span>      | <span data-ttu-id="4599e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4599e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4599e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4599e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4599e-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4599e-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4599e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4599e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4599e-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4599e-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4599e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4599e-115">Application</span></span> | <span data-ttu-id="4599e-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4599e-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4599e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4599e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4599e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4599e-118">Request headers</span></span>
| <span data-ttu-id="4599e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4599e-119">Name</span></span>       | <span data-ttu-id="4599e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4599e-120">Type</span></span> | <span data-ttu-id="4599e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4599e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4599e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4599e-122">Authorization</span></span>  | <span data-ttu-id="4599e-123">string</span><span class="sxs-lookup"><span data-stu-id="4599e-123">string</span></span>  | <span data-ttu-id="4599e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4599e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4599e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4599e-126">Request body</span></span>
<span data-ttu-id="4599e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4599e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4599e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4599e-128">Response</span></span>

<span data-ttu-id="4599e-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4599e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4599e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4599e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4599e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4599e-132">Request</span></span>
<span data-ttu-id="4599e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4599e-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4599e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4599e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
# <a name="c"></a>[<span data-ttu-id="4599e-135">C#</span><span class="sxs-lookup"><span data-stu-id="4599e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4599e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4599e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4599e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4599e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4599e-138">Java</span><span class="sxs-lookup"><span data-stu-id="4599e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-inferenceclassificationoverride-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4599e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4599e-139">Response</span></span>
<span data-ttu-id="4599e-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4599e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
