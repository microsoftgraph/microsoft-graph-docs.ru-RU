---
title: Удаление объекта Скопедролемембер
description: Удаление члена с областью ролей из единицы админстративе.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 71ef52be4cbda5cc0e3ed1d9da7145b50ce8f006
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258767"
---
# <a name="remove-a-scopedrolemember"></a><span data-ttu-id="19551-103">Удаление объекта Скопедролемембер</span><span class="sxs-lookup"><span data-stu-id="19551-103">Remove a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19551-104">Удаление члена с областью ролей из единицы админстративе.</span><span class="sxs-lookup"><span data-stu-id="19551-104">Remove a scoped-role member from an adminstrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="19551-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19551-105">Permissions</span></span>
<span data-ttu-id="19551-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19551-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="19551-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19551-108">Permission type</span></span>      | <span data-ttu-id="19551-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19551-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19551-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19551-110">Delegated (work or school account)</span></span> | <span data-ttu-id="19551-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19551-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="19551-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19551-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19551-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19551-113">Not supported.</span></span>    |
|<span data-ttu-id="19551-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19551-114">Application</span></span> | <span data-ttu-id="19551-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19551-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19551-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19551-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/scopedRoleMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="19551-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19551-117">Request headers</span></span>
| <span data-ttu-id="19551-118">Имя</span><span class="sxs-lookup"><span data-stu-id="19551-118">Name</span></span>       | <span data-ttu-id="19551-119">Описание</span><span class="sxs-lookup"><span data-stu-id="19551-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="19551-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19551-120">Authorization</span></span>  | <span data-ttu-id="19551-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19551-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19551-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="19551-123">Request body</span></span>
<span data-ttu-id="19551-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="19551-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19551-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="19551-125">Response</span></span>

<span data-ttu-id="19551-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="19551-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19551-128">Пример</span><span class="sxs-lookup"><span data-stu-id="19551-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19551-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="19551-129">Request</span></span>
<span data-ttu-id="19551-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19551-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_scopedrolemember"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="19551-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="19551-131">Response</span></span>
<span data-ttu-id="19551-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19551-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="19551-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="19551-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="19551-136">C#</span><span class="sxs-lookup"><span data-stu-id="19551-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_scopedrolemember-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19551-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="19551-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_scopedrolemember-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="19551-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="19551-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_scopedrolemember-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/administrativeunit-delete-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/administrativeunit-delete-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-delete-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
