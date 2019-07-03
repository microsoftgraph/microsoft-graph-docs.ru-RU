---
title: Удаление канала
description: Удаление канала.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b587ddb85f7a7911ffb2e964b45a6d3dacbf17b3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438540"
---
# <a name="delete-channel"></a><span data-ttu-id="87e34-103">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="87e34-103">Delete channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87e34-104">Удаление [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="87e34-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="87e34-105">**Примечание**. Существует известная проблема с разрешениями для приложений и этим API.</span><span class="sxs-lookup"><span data-stu-id="87e34-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="87e34-106">Дополнительные сведения см. в [списке известных проблем](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="87e34-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="87e34-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87e34-107">Permissions</span></span>
<span data-ttu-id="87e34-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87e34-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87e34-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87e34-110">Permission type</span></span>      | <span data-ttu-id="87e34-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87e34-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87e34-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87e34-112">Delegated (work or school account)</span></span> | <span data-ttu-id="87e34-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87e34-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="87e34-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87e34-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87e34-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87e34-115">Not supported.</span></span>    |
|<span data-ttu-id="87e34-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87e34-116">Application</span></span> | <span data-ttu-id="87e34-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87e34-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="87e34-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="87e34-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="87e34-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="87e34-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="87e34-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87e34-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="87e34-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87e34-121">Request headers</span></span>
| <span data-ttu-id="87e34-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87e34-122">Header</span></span>       | <span data-ttu-id="87e34-123">Значение</span><span class="sxs-lookup"><span data-stu-id="87e34-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="87e34-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87e34-124">Authorization</span></span>  | <span data-ttu-id="87e34-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87e34-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="87e34-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="87e34-127">Request body</span></span>
<span data-ttu-id="87e34-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87e34-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87e34-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="87e34-129">Response</span></span>

<span data-ttu-id="87e34-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="87e34-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87e34-132">Пример</span><span class="sxs-lookup"><span data-stu-id="87e34-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87e34-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="87e34-133">Request</span></span>
<span data-ttu-id="87e34-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87e34-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="87e34-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="87e34-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="87e34-136">C#</span><span class="sxs-lookup"><span data-stu-id="87e34-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="87e34-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="87e34-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="87e34-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="87e34-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="87e34-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="87e34-139">Response</span></span>

<span data-ttu-id="87e34-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="87e34-140">The following is an example of the response.</span></span> 
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
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
