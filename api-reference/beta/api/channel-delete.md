---
title: Удаление канала
description: Удаление канала.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6e360f34bffc9545844b3261433d061956145041
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635521"
---
# <a name="delete-channel"></a><span data-ttu-id="b3cfe-103">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="b3cfe-103">Delete channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3cfe-104">Удаление [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="b3cfe-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="b3cfe-105">**Примечание**. Существует известная проблема с разрешениями для приложений и этим API.</span><span class="sxs-lookup"><span data-stu-id="b3cfe-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="b3cfe-106">Дополнительные сведения см. в [списке известных проблем](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="b3cfe-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="b3cfe-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3cfe-107">Permissions</span></span>
<span data-ttu-id="b3cfe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3cfe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3cfe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3cfe-110">Permission type</span></span>      | <span data-ttu-id="b3cfe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3cfe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3cfe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3cfe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b3cfe-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3cfe-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b3cfe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3cfe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3cfe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3cfe-115">Not supported.</span></span>    |
|<span data-ttu-id="b3cfe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3cfe-116">Application</span></span> | <span data-ttu-id="b3cfe-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3cfe-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="b3cfe-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="b3cfe-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b3cfe-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="b3cfe-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b3cfe-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3cfe-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b3cfe-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3cfe-121">Request headers</span></span>
| <span data-ttu-id="b3cfe-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3cfe-122">Header</span></span>       | <span data-ttu-id="b3cfe-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b3cfe-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b3cfe-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3cfe-124">Authorization</span></span>  | <span data-ttu-id="b3cfe-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3cfe-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b3cfe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3cfe-127">Request body</span></span>
<span data-ttu-id="b3cfe-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3cfe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3cfe-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3cfe-129">Response</span></span>

<span data-ttu-id="b3cfe-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b3cfe-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3cfe-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b3cfe-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3cfe-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3cfe-133">Request</span></span>
<span data-ttu-id="b3cfe-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3cfe-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

#### <a name="response"></a><span data-ttu-id="b3cfe-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3cfe-135">Response</span></span>

<span data-ttu-id="b3cfe-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b3cfe-136">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b3cfe-137">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="b3cfe-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b3cfe-138">Языках</span><span class="sxs-lookup"><span data-stu-id="b3cfe-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_channel-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b3cfe-139">Язык</span><span class="sxs-lookup"><span data-stu-id="b3cfe-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_channel-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/channel-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
