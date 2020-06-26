---
title: Добавление участника
description: Добавьте члена в группу Microsoft 365 или группу безопасности с помощью свойства навигации **Members** .
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: fe3f3a5fe1bde8c14e9dbc3a6e12e486dd7c1bd2
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895813"
---
# <a name="add-member"></a><span data-ttu-id="07efa-103">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="07efa-103">Add member</span></span>

<span data-ttu-id="07efa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07efa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07efa-105">Добавьте члена в группу Microsoft 365 или группу безопасности с помощью свойства навигации **Members** .</span><span class="sxs-lookup"><span data-stu-id="07efa-105">Add a member to a Microsoft 365 group or security group through the **members** navigation property.</span></span>

<span data-ttu-id="07efa-106">Вы можете добавлять пользователей, участников служб или другие группы.</span><span class="sxs-lookup"><span data-stu-id="07efa-106">You can add users, service principals or other groups.</span></span> 

> [!Important]
> <span data-ttu-id="07efa-107">Вы можете добавлять пользователей только в группы безопасности и Microsoft 365, управляемые через облако.</span><span class="sxs-lookup"><span data-stu-id="07efa-107">You can only add users to security and Microsoft 365 groups managed through the cloud.</span></span>

## <a name="permissions"></a><span data-ttu-id="07efa-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="07efa-108">Permissions</span></span>
<span data-ttu-id="07efa-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="07efa-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="07efa-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07efa-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07efa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07efa-111">Permission type</span></span>      | <span data-ttu-id="07efa-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07efa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07efa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07efa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="07efa-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07efa-114">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="07efa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07efa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07efa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07efa-116">Not supported.</span></span>    |
|<span data-ttu-id="07efa-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="07efa-117">Application</span></span> | <span data-ttu-id="07efa-118">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07efa-118">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07efa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07efa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="07efa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07efa-120">Request headers</span></span>
| <span data-ttu-id="07efa-121">Имя</span><span class="sxs-lookup"><span data-stu-id="07efa-121">Name</span></span> | <span data-ttu-id="07efa-122">Описание</span><span class="sxs-lookup"><span data-stu-id="07efa-122">Description</span></span>|
|:---- |:-----------|
| <span data-ttu-id="07efa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07efa-123">Authorization</span></span> | <span data-ttu-id="07efa-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="07efa-124">Bearer {token}.</span></span> <span data-ttu-id="07efa-125">Required.</span><span class="sxs-lookup"><span data-stu-id="07efa-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07efa-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07efa-126">Request body</span></span>
<span data-ttu-id="07efa-127">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) или [group](../resources/group.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07efa-127">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) or [group](../resources/group.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="07efa-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="07efa-128">Response</span></span>
<span data-ttu-id="07efa-129">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="07efa-129">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="07efa-130">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="07efa-130">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07efa-131">Пример</span><span class="sxs-lookup"><span data-stu-id="07efa-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="07efa-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="07efa-132">Request</span></span>
<span data-ttu-id="07efa-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07efa-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="07efa-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="07efa-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/members/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="07efa-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07efa-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07efa-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07efa-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="07efa-137">C#</span><span class="sxs-lookup"><span data-stu-id="07efa-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-group-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="07efa-138">В тексте запроса `id` добавьте представление объекта [directoryObject](../resources/directoryobject.md), [пользователя](../resources/user.md)или [группы](../resources/group.md) , который вы хотите добавить, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07efa-138">In the request body, supply a JSON representation of the `id` of the [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="07efa-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="07efa-139">Response</span></span>
<span data-ttu-id="07efa-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="07efa-140">The following is an example of the response.</span></span>
><span data-ttu-id="07efa-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="07efa-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="07efa-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07efa-142">All the properties will be returned from an actual call.</span></span>
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
