---
title: Удаление канала
description: Удаление канала.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b6a2e1f8c0eef45e227affdf0d73417ee90992b8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003884"
---
# <a name="delete-channel"></a><span data-ttu-id="c266a-103">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="c266a-103">Delete channel</span></span>



<span data-ttu-id="c266a-104">Удаление [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="c266a-104">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="c266a-105">**Примечание**. Существует известная проблема с разрешениями для приложений и этим API.</span><span class="sxs-lookup"><span data-stu-id="c266a-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="c266a-106">Дополнительные сведения см. в [списке известных проблем](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="c266a-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

> <span data-ttu-id="c266a-107">**Note**: данные в удаленных каналах продолжат храниться в течение нескольких недель, чтобы владелец группы мог восстановить удаленный канал.</span><span class="sxs-lookup"><span data-stu-id="c266a-107">**Note**: The data in deleted channels will continue to be stored for several weeks to allow team owner to recovery deleted channel.</span></span> <span data-ttu-id="c266a-108">В течение этого времени не создается новый канал с таким же отображаемым именем (displayName).</span><span class="sxs-lookup"><span data-stu-id="c266a-108">During that time, a new channel with the same displayName may not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="c266a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c266a-109">Permissions</span></span>
<span data-ttu-id="c266a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c266a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c266a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c266a-112">Permission type</span></span>      | <span data-ttu-id="c266a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c266a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c266a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c266a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c266a-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c266a-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c266a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c266a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c266a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c266a-117">Not supported.</span></span>    |
|<span data-ttu-id="c266a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c266a-118">Application</span></span> | <span data-ttu-id="c266a-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c266a-119">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="c266a-120">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="c266a-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c266a-121">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="c266a-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c266a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c266a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c266a-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c266a-123">Request headers</span></span>
| <span data-ttu-id="c266a-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c266a-124">Header</span></span>       | <span data-ttu-id="c266a-125">Значение</span><span class="sxs-lookup"><span data-stu-id="c266a-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c266a-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c266a-126">Authorization</span></span>  | <span data-ttu-id="c266a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c266a-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c266a-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c266a-129">Request body</span></span>
<span data-ttu-id="c266a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c266a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c266a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c266a-131">Response</span></span>

<span data-ttu-id="c266a-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c266a-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c266a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c266a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c266a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c266a-135">Request</span></span>
<span data-ttu-id="c266a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c266a-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c266a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c266a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c266a-138">C#</span><span class="sxs-lookup"><span data-stu-id="c266a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c266a-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="c266a-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c266a-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c266a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c266a-141">Java</span><span class="sxs-lookup"><span data-stu-id="c266a-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c266a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c266a-142">Response</span></span>

<span data-ttu-id="c266a-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c266a-143">The following is an example of the response.</span></span> 
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
  "description": "Delete channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
