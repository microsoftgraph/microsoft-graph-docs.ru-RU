---
title: Канал исправлений
description: Обновление свойств указанного канала.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 930ed3298eff15303cd9a4dc228e5d7340a7af5a
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491597"
---
# <a name="patch-channel"></a><span data-ttu-id="0d6ae-103">Канал исправлений</span><span class="sxs-lookup"><span data-stu-id="0d6ae-103">Patch channel</span></span>

<span data-ttu-id="0d6ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d6ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d6ae-105">Обновление свойств указанного [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="0d6ae-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0d6ae-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d6ae-106">Permissions</span></span>

<span data-ttu-id="0d6ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d6ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d6ae-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d6ae-109">Permission type</span></span>      | <span data-ttu-id="0d6ae-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d6ae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d6ae-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d6ae-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0d6ae-112">Чаннелсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0d6ae-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="0d6ae-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d6ae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d6ae-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d6ae-114">Not supported.</span></span>    |
|<span data-ttu-id="0d6ae-115">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="0d6ae-115">Application</span></span> | <span data-ttu-id="0d6ae-116">Чаннелсеттингс. Edit. Group \*, Чаннелсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0d6ae-116">ChannelSettings.Edit.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="0d6ae-117">**Note**: разрешения, помеченные как \* использовать [согласие с определенным ресурсом]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="0d6ae-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="0d6ae-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="0d6ae-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0d6ae-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="0d6ae-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0d6ae-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d6ae-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0d6ae-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d6ae-121">Request headers</span></span>
| <span data-ttu-id="0d6ae-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d6ae-122">Header</span></span>       | <span data-ttu-id="0d6ae-123">Значение</span><span class="sxs-lookup"><span data-stu-id="0d6ae-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0d6ae-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d6ae-124">Authorization</span></span>  | <span data-ttu-id="0d6ae-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d6ae-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0d6ae-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d6ae-127">Content-Type</span></span>  | <span data-ttu-id="0d6ae-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0d6ae-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0d6ae-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d6ae-129">Request body</span></span>

<span data-ttu-id="0d6ae-130">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d6ae-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="0d6ae-131">Note: невозможно обновить `membershipType` значение существующего канала.</span><span class="sxs-lookup"><span data-stu-id="0d6ae-131">Note: You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="0d6ae-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d6ae-132">Response</span></span>

<span data-ttu-id="0d6ae-133">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0d6ae-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0d6ae-134">Пример</span><span class="sxs-lookup"><span data-stu-id="0d6ae-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d6ae-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d6ae-135">Request</span></span>

<span data-ttu-id="0d6ae-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d6ae-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d6ae-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d6ae-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="objective-c"></a>[<span data-ttu-id="0d6ae-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d6ae-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0d6ae-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d6ae-139">Response</span></span>

<span data-ttu-id="0d6ae-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d6ae-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
