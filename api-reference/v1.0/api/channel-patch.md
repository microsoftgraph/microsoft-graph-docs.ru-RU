---
title: Канал патчей
description: Обновление свойств указанного канала.
author: anandjo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4c611ea955c82be94f5e0220fe0632d2c5791fc8
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51506879"
---
# <a name="patch-channel"></a><span data-ttu-id="bac2f-103">Канал патчей</span><span class="sxs-lookup"><span data-stu-id="bac2f-103">Patch channel</span></span>

<span data-ttu-id="bac2f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bac2f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bac2f-105">Обновление свойств указанного [канала.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="bac2f-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bac2f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bac2f-106">Permissions</span></span>

<span data-ttu-id="bac2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bac2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bac2f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bac2f-109">Permission type</span></span>      | <span data-ttu-id="bac2f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bac2f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bac2f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bac2f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bac2f-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bac2f-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="bac2f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bac2f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bac2f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bac2f-114">Not supported.</span></span>    |
|<span data-ttu-id="bac2f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bac2f-115">Application</span></span> | <span data-ttu-id="bac2f-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bac2f-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="bac2f-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="bac2f-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="bac2f-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="bac2f-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="bac2f-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="bac2f-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="bac2f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bac2f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{team-id}/channels/{channel-id}
```

## <a name="request-headers"></a><span data-ttu-id="bac2f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bac2f-121">Request headers</span></span>
| <span data-ttu-id="bac2f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bac2f-122">Header</span></span>       | <span data-ttu-id="bac2f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="bac2f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bac2f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bac2f-124">Authorization</span></span>  | <span data-ttu-id="bac2f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bac2f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bac2f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bac2f-127">Content-Type</span></span>  | <span data-ttu-id="bac2f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bac2f-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bac2f-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bac2f-130">Request body</span></span>

<span data-ttu-id="bac2f-131">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bac2f-131">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="bac2f-132">**Примечание:** Невозможно обновить `membershipType` значение для существующего канала.</span><span class="sxs-lookup"><span data-stu-id="bac2f-132">**Note:** You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="bac2f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bac2f-133">Response</span></span>

<span data-ttu-id="bac2f-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bac2f-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bac2f-135">Пример</span><span class="sxs-lookup"><span data-stu-id="bac2f-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="bac2f-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="bac2f-136">Request</span></span>

<span data-ttu-id="bac2f-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bac2f-137">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bac2f-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="bac2f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
```
# <a name="objective-c"></a>[<span data-ttu-id="bac2f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bac2f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bac2f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="bac2f-140">Response</span></span>

<span data-ttu-id="bac2f-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bac2f-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 204 No Content
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
