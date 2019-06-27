---
title: Удаление administrativeUnit
description: Удаление administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4ff922f73fcc5730452db5403a2db0439ea217fc
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258753"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="dede8-103">Удаление administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="dede8-103">Delete administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dede8-104">Удаление [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="dede8-104">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dede8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dede8-105">Permissions</span></span>
<span data-ttu-id="dede8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dede8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dede8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dede8-108">Permission type</span></span>      | <span data-ttu-id="dede8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dede8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dede8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dede8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dede8-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dede8-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dede8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dede8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dede8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dede8-113">Not supported.</span></span>    |
|<span data-ttu-id="dede8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dede8-114">Application</span></span> | <span data-ttu-id="dede8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dede8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dede8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dede8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="dede8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dede8-117">Request headers</span></span>
| <span data-ttu-id="dede8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="dede8-118">Name</span></span>       | <span data-ttu-id="dede8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="dede8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dede8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dede8-120">Authorization</span></span>  | <span data-ttu-id="dede8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dede8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dede8-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dede8-123">Request body</span></span>
<span data-ttu-id="dede8-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dede8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dede8-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="dede8-125">Response</span></span>

<span data-ttu-id="dede8-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dede8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dede8-128">Пример</span><span class="sxs-lookup"><span data-stu-id="dede8-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dede8-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="dede8-129">Request</span></span>
<span data-ttu-id="dede8-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dede8-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="dede8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="dede8-131">Response</span></span>
<span data-ttu-id="dede8-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dede8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dede8-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="dede8-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dede8-136">C#</span><span class="sxs-lookup"><span data-stu-id="dede8-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_administrativeunit-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dede8-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="dede8-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_administrativeunit-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dede8-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dede8-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_administrativeunit-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/administrativeunit-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
