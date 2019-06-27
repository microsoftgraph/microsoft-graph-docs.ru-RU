---
title: Удаление объекта inferenceClassificationOverride
description: Удаление переопределения по идентификатору.
localization_priority: Normal
ms.openlocfilehash: ae4043f0f118519de860c12431f0c6a80289a08f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277114"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="7149f-103">Удаление объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="7149f-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="7149f-104">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="7149f-104">Delete an override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="7149f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7149f-105">Permissions</span></span>
<span data-ttu-id="7149f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7149f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7149f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7149f-108">Permission type</span></span>      | <span data-ttu-id="7149f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7149f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7149f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7149f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7149f-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7149f-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7149f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7149f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7149f-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7149f-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7149f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7149f-114">Application</span></span> | <span data-ttu-id="7149f-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7149f-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7149f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7149f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7149f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7149f-117">Request headers</span></span>
| <span data-ttu-id="7149f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7149f-118">Name</span></span>       | <span data-ttu-id="7149f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7149f-119">Type</span></span> | <span data-ttu-id="7149f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7149f-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7149f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7149f-121">Authorization</span></span>  | <span data-ttu-id="7149f-122">string</span><span class="sxs-lookup"><span data-stu-id="7149f-122">string</span></span>  | <span data-ttu-id="7149f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7149f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7149f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7149f-125">Request body</span></span>
<span data-ttu-id="7149f-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7149f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7149f-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="7149f-127">Response</span></span>

<span data-ttu-id="7149f-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7149f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7149f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7149f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7149f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7149f-131">Request</span></span>
<span data-ttu-id="7149f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7149f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["98f5bdef-576a-404d-a2ea-07a3cf34af4r"],
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
##### <a name="response"></a><span data-ttu-id="7149f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7149f-133">Response</span></span>
<span data-ttu-id="7149f-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7149f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7149f-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="7149f-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7149f-138">C#</span><span class="sxs-lookup"><span data-stu-id="7149f-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_inferenceclassificationoverride-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7149f-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="7149f-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_inferenceclassificationoverride-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7149f-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7149f-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_inferenceclassificationoverride-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/inferenceclassificationoverride-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
