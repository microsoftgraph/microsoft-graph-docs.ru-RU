---
title: Канал исправлений
description: Обновление свойств указанного канала.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b90e3abff3d0624b7639195f02e342f7fa11c5ee
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848929"
---
# <a name="patch-channel"></a><span data-ttu-id="ab6a4-103">Канал исправлений</span><span class="sxs-lookup"><span data-stu-id="ab6a4-103">Patch channel</span></span>

<span data-ttu-id="ab6a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab6a4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab6a4-105">Обновление свойств указанного [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="ab6a4-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ab6a4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab6a4-106">Permissions</span></span>

<span data-ttu-id="ab6a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab6a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab6a4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab6a4-109">Permission type</span></span>      | <span data-ttu-id="ab6a4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab6a4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab6a4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab6a4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ab6a4-112">Чаннелсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ab6a4-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="ab6a4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab6a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab6a4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab6a4-114">Not supported.</span></span>    |
|<span data-ttu-id="ab6a4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab6a4-115">Application</span></span> | <span data-ttu-id="ab6a4-116">Чаннелсеттингс. ReadWrite. Group \*, Чаннелсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ab6a4-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="ab6a4-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="ab6a4-117">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="ab6a4-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="ab6a4-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ab6a4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab6a4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ab6a4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab6a4-120">Request headers</span></span>
| <span data-ttu-id="ab6a4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab6a4-121">Header</span></span>       | <span data-ttu-id="ab6a4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ab6a4-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ab6a4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab6a4-123">Authorization</span></span>  | <span data-ttu-id="ab6a4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab6a4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ab6a4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab6a4-126">Content-Type</span></span>  | <span data-ttu-id="ab6a4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ab6a4-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab6a4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab6a4-128">Request body</span></span>

<span data-ttu-id="ab6a4-129">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab6a4-129">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="ab6a4-130">**Примечание:** Вы не можете обновить `membershipType` значение для существующего канала.</span><span class="sxs-lookup"><span data-stu-id="ab6a4-130">**Note:** You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="ab6a4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab6a4-131">Response</span></span>

<span data-ttu-id="ab6a4-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ab6a4-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ab6a4-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ab6a4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab6a4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab6a4-134">Request</span></span>

<span data-ttu-id="ab6a4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab6a4-135">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```

<!-- {
  "blockType": "request",
  "name": "update_channel"
}-->

### <a name="response"></a><span data-ttu-id="ab6a4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab6a4-136">Response</span></span>

<span data-ttu-id="ab6a4-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab6a4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
