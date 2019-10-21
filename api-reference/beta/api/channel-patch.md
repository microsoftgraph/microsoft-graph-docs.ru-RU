---
title: Канал исправлений
description: Обновление свойств указанного канала.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b9b8abd495a9ce66458973360a93e47f0bddfdf9
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2019
ms.locfileid: "37275677"
---
# <a name="patch-channel"></a><span data-ttu-id="9dca6-103">Канал исправлений</span><span class="sxs-lookup"><span data-stu-id="9dca6-103">Patch channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dca6-104">Обновление свойств указанного [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="9dca6-104">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9dca6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9dca6-105">Permissions</span></span>

<span data-ttu-id="9dca6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dca6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dca6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9dca6-108">Permission type</span></span>      | <span data-ttu-id="9dca6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9dca6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9dca6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9dca6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9dca6-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dca6-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9dca6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9dca6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dca6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dca6-113">Not supported.</span></span>    |
|<span data-ttu-id="9dca6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9dca6-114">Application</span></span> | <span data-ttu-id="9dca6-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dca6-115">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="9dca6-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="9dca6-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9dca6-117">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="9dca6-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9dca6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9dca6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9dca6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9dca6-119">Request headers</span></span>
| <span data-ttu-id="9dca6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9dca6-120">Header</span></span>       | <span data-ttu-id="9dca6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9dca6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9dca6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9dca6-122">Authorization</span></span>  | <span data-ttu-id="9dca6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9dca6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9dca6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9dca6-125">Content-Type</span></span>  | <span data-ttu-id="9dca6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9dca6-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9dca6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9dca6-127">Request body</span></span>

<span data-ttu-id="9dca6-128">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9dca6-128">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="9dca6-129">Note: невозможно обновить `membershipType` значение существующего канала.</span><span class="sxs-lookup"><span data-stu-id="9dca6-129">Note: You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="9dca6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dca6-130">Response</span></span>

<span data-ttu-id="9dca6-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9dca6-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9dca6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9dca6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9dca6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9dca6-133">Request</span></span>

<span data-ttu-id="9dca6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9dca6-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9dca6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9dca6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9dca6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9dca6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9dca6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dca6-137">Response</span></span>

<span data-ttu-id="9dca6-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9dca6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
