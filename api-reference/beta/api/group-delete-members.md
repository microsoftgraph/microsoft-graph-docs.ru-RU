---
title: Удаление участника
description: Используйте этот API, чтобы удалить участника из группы Microsoft 365, группы безопасности или группы безопасности с включенной поддержкой почты с помощью свойства навигации **Members** . Вы можете удалять пользователей или другие группы.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e4d91d97f48f1a0adec10c0d42d51be399fb0f28
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895869"
---
# <a name="remove-member"></a><span data-ttu-id="c2b5e-104">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="c2b5e-104">Remove member</span></span>

<span data-ttu-id="c2b5e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2b5e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2b5e-106">С помощью этого API можно удалить участника из группы через свойство навигации **members**.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-106">Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2b5e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2b5e-107">Permissions</span></span>
<span data-ttu-id="c2b5e-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c2b5e-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2b5e-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2b5e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2b5e-110">Permission type</span></span>      | <span data-ttu-id="c2b5e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2b5e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2b5e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2b5e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c2b5e-113">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c2b5e-113">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c2b5e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2b5e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2b5e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-115">Not supported.</span></span> |
|<span data-ttu-id="c2b5e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c2b5e-116">Application</span></span> | <span data-ttu-id="c2b5e-117">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2b5e-117">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2b5e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2b5e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c2b5e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2b5e-119">Request headers</span></span>
| <span data-ttu-id="c2b5e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c2b5e-120">Name</span></span>       | <span data-ttu-id="c2b5e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c2b5e-121">Type</span></span> | <span data-ttu-id="c2b5e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c2b5e-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c2b5e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2b5e-123">Authorization</span></span>  | <span data-ttu-id="c2b5e-124">string</span><span class="sxs-lookup"><span data-stu-id="c2b5e-124">string</span></span>  | <span data-ttu-id="c2b5e-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-125">Bearer {token}.</span></span> <span data-ttu-id="c2b5e-126">Required.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2b5e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2b5e-127">Request body</span></span>
<span data-ttu-id="c2b5e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2b5e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2b5e-129">Response</span></span>
<span data-ttu-id="c2b5e-130">If successful, this method returns `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-130">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="c2b5e-131">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-131">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2b5e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c2b5e-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c2b5e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2b5e-133">Request</span></span>
<span data-ttu-id="c2b5e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2b5e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2b5e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_member_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="c2b5e-136">C#</span><span class="sxs-lookup"><span data-stu-id="c2b5e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2b5e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2b5e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2b5e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2b5e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c2b5e-139">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-139">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="c2b5e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2b5e-140">Response</span></span>
<span data-ttu-id="c2b5e-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-141">The following is an example of the response.</span></span>
><span data-ttu-id="c2b5e-142">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c2b5e-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
