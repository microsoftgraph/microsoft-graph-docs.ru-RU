---
title: Канал исправлений
description: Обновление свойств указанного канала.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c6233c22cb5da1bc55079a048a6c86718bd686c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440229"
---
# <a name="patch-channel"></a><span data-ttu-id="4db5e-103">Канал исправлений</span><span class="sxs-lookup"><span data-stu-id="4db5e-103">Patch channel</span></span>

<span data-ttu-id="4db5e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4db5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4db5e-105">Обновление свойств указанного [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="4db5e-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4db5e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4db5e-106">Permissions</span></span>

<span data-ttu-id="4db5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4db5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4db5e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4db5e-109">Permission type</span></span>      | <span data-ttu-id="4db5e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4db5e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4db5e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4db5e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4db5e-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4db5e-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4db5e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4db5e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4db5e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4db5e-114">Not supported.</span></span>    |
|<span data-ttu-id="4db5e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4db5e-115">Application</span></span> | <span data-ttu-id="4db5e-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4db5e-116">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="4db5e-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="4db5e-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="4db5e-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="4db5e-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4db5e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4db5e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4db5e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4db5e-120">Request headers</span></span>
| <span data-ttu-id="4db5e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4db5e-121">Header</span></span>       | <span data-ttu-id="4db5e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4db5e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4db5e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4db5e-123">Authorization</span></span>  | <span data-ttu-id="4db5e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4db5e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4db5e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4db5e-126">Content-Type</span></span>  | <span data-ttu-id="4db5e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4db5e-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4db5e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4db5e-128">Request body</span></span>

<span data-ttu-id="4db5e-129">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4db5e-129">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="4db5e-130">Note: невозможно обновить `membershipType` значение существующего канала.</span><span class="sxs-lookup"><span data-stu-id="4db5e-130">Note: You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="4db5e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4db5e-131">Response</span></span>

<span data-ttu-id="4db5e-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4db5e-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4db5e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4db5e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4db5e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4db5e-134">Request</span></span>

<span data-ttu-id="4db5e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4db5e-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4db5e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4db5e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="objective-c"></a>[<span data-ttu-id="4db5e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4db5e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4db5e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4db5e-138">Response</span></span>

<span data-ttu-id="4db5e-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4db5e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
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
