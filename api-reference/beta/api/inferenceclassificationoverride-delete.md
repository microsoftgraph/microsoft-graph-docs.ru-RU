---
title: Удаление объекта inferenceClassificationOverride
description: Удаление отсортированного переопределения папки "Входящие", указанного с помощью идентификатора.
localization_priority: Normal
ms.openlocfilehash: 97ce2f0aab82e031fec2b2b96e3ffd8d08c92a3b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857508"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="3c1f6-103">Удаление объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="3c1f6-103">Delete inferenceClassificationOverride</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c1f6-104">Удаление отсортированного переопределения [папки "Входящие"](../resources/manage-focused-inbox.md) , указанного с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="3c1f6-104">Delete a [Focused Inbox](../resources/manage-focused-inbox.md) override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="3c1f6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c1f6-105">Permissions</span></span>
<span data-ttu-id="3c1f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c1f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c1f6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c1f6-108">Permission type</span></span>      | <span data-ttu-id="3c1f6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c1f6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c1f6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c1f6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3c1f6-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c1f6-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3c1f6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c1f6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c1f6-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c1f6-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3c1f6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c1f6-114">Application</span></span> | <span data-ttu-id="3c1f6-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c1f6-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c1f6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c1f6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3c1f6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c1f6-117">Request headers</span></span>
| <span data-ttu-id="3c1f6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3c1f6-118">Name</span></span>       | <span data-ttu-id="3c1f6-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3c1f6-119">Type</span></span> | <span data-ttu-id="3c1f6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3c1f6-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3c1f6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c1f6-121">Authorization</span></span>  | <span data-ttu-id="3c1f6-122">string</span><span class="sxs-lookup"><span data-stu-id="3c1f6-122">string</span></span>  | <span data-ttu-id="3c1f6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c1f6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c1f6-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3c1f6-125">Request body</span></span>
<span data-ttu-id="3c1f6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c1f6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c1f6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c1f6-127">Response</span></span>

<span data-ttu-id="3c1f6-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3c1f6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c1f6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3c1f6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c1f6-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c1f6-131">Request</span></span>
<span data-ttu-id="3c1f6-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c1f6-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3c1f6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c1f6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c1f6-134">C#</span><span class="sxs-lookup"><span data-stu-id="3c1f6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c1f6-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c1f6-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c1f6-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3c1f6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3c1f6-137">Java</span><span class="sxs-lookup"><span data-stu-id="3c1f6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-inferenceclassificationoverride-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3c1f6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c1f6-138">Response</span></span>
<span data-ttu-id="3c1f6-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c1f6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
