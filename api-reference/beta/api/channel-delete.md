---
title: Удаление канала
description: Удаление канала.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5511c19f23be69a2aad14acc35bbef9c3710fc88
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959312"
---
# <a name="delete-channel"></a><span data-ttu-id="fd6fa-103">Удаление канала</span><span class="sxs-lookup"><span data-stu-id="fd6fa-103">Delete channel</span></span>

<span data-ttu-id="fd6fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd6fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd6fa-105">Удаление [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="fd6fa-105">Delete the [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="fd6fa-106">**Примечание**. Существует известная проблема с разрешениями для приложений и этим API.</span><span class="sxs-lookup"><span data-stu-id="fd6fa-106">**Note** : There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="fd6fa-107">Дополнительные сведения см. в [списке известных проблем](/graph/known-issues#application-permissions).</span><span class="sxs-lookup"><span data-stu-id="fd6fa-107">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="fd6fa-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd6fa-108">Permissions</span></span>
<span data-ttu-id="fd6fa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd6fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd6fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd6fa-111">Permission type</span></span>      | <span data-ttu-id="fd6fa-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd6fa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd6fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd6fa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fd6fa-114">Channel. Delete. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fd6fa-114">Channel.Delete.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="fd6fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd6fa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd6fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd6fa-116">Not supported.</span></span>    |
|<span data-ttu-id="fd6fa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd6fa-117">Application</span></span> | <span data-ttu-id="fd6fa-118">Channel. Delete. Group \*, Channel. Delete. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fd6fa-118">Channel.Delete.Group\*, Channel.Delete.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="fd6fa-119">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="fd6fa-119">**Note** : Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="fd6fa-120">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="fd6fa-120">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="fd6fa-121">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="fd6fa-121">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="fd6fa-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd6fa-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fd6fa-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd6fa-123">Request headers</span></span>
| <span data-ttu-id="fd6fa-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd6fa-124">Header</span></span>       | <span data-ttu-id="fd6fa-125">Значение</span><span class="sxs-lookup"><span data-stu-id="fd6fa-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fd6fa-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd6fa-126">Authorization</span></span>  | <span data-ttu-id="fd6fa-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd6fa-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fd6fa-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd6fa-129">Request body</span></span>
<span data-ttu-id="fd6fa-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd6fa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd6fa-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd6fa-131">Response</span></span>

<span data-ttu-id="fd6fa-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fd6fa-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd6fa-134">Пример</span><span class="sxs-lookup"><span data-stu-id="fd6fa-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd6fa-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd6fa-135">Request</span></span>
<span data-ttu-id="fd6fa-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd6fa-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fd6fa-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd6fa-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_channel"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="c"></a>[<span data-ttu-id="fd6fa-138">C#</span><span class="sxs-lookup"><span data-stu-id="fd6fa-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd6fa-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd6fa-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd6fa-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd6fa-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fd6fa-141">Java</span><span class="sxs-lookup"><span data-stu-id="fd6fa-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fd6fa-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd6fa-142">Response</span></span>

<span data-ttu-id="fd6fa-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fd6fa-143">The following is an example of the response.</span></span> 
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


