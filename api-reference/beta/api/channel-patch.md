---
title: Канал исправлений
description: Обновление свойств указанного канала.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8dc93cf3d301f2577076852024cfb535e3852741
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863118"
---
# <a name="patch-channel"></a><span data-ttu-id="f8a12-103">Канал исправлений</span><span class="sxs-lookup"><span data-stu-id="f8a12-103">Patch channel</span></span>

<span data-ttu-id="f8a12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8a12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8a12-105">Обновление свойств указанного [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="f8a12-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8a12-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8a12-106">Permissions</span></span>

<span data-ttu-id="f8a12-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f8a12-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f8a12-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8a12-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8a12-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8a12-109">Permission type</span></span>      | <span data-ttu-id="f8a12-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8a12-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8a12-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8a12-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f8a12-112">Чаннелсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f8a12-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="f8a12-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8a12-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8a12-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8a12-114">Not supported.</span></span>    |
|<span data-ttu-id="f8a12-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8a12-115">Application</span></span> | <span data-ttu-id="f8a12-116">Чаннелсеттингс. Edit. Group \*, Чаннелсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f8a12-116">ChannelSettings.Edit.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="f8a12-117">**Note**: разрешения, помеченные как \* использовать [согласие с определенным ресурсом]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="f8a12-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="f8a12-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="f8a12-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f8a12-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="f8a12-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f8a12-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8a12-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f8a12-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8a12-121">Request headers</span></span>
| <span data-ttu-id="f8a12-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8a12-122">Header</span></span>       | <span data-ttu-id="f8a12-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f8a12-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f8a12-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8a12-124">Authorization</span></span>  | <span data-ttu-id="f8a12-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="f8a12-125">Bearer {token}.</span></span> <span data-ttu-id="f8a12-126">Required.</span><span class="sxs-lookup"><span data-stu-id="f8a12-126">Required.</span></span>  |
| <span data-ttu-id="f8a12-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f8a12-127">Content-Type</span></span>  | <span data-ttu-id="f8a12-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f8a12-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f8a12-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8a12-129">Request body</span></span>

<span data-ttu-id="f8a12-130">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8a12-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="f8a12-131">Note: невозможно обновить `membershipType` значение существующего канала.</span><span class="sxs-lookup"><span data-stu-id="f8a12-131">Note: You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="f8a12-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8a12-132">Response</span></span>

<span data-ttu-id="f8a12-133">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f8a12-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f8a12-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f8a12-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8a12-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8a12-135">Request</span></span>

<span data-ttu-id="f8a12-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8a12-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f8a12-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8a12-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="objective-c"></a>[<span data-ttu-id="f8a12-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8a12-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f8a12-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8a12-139">Response</span></span>

<span data-ttu-id="f8a12-140">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="f8a12-140">Here is an example of the response.</span></span> <span data-ttu-id="f8a12-141">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="f8a12-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f8a12-142">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f8a12-142">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 204 No Content
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
