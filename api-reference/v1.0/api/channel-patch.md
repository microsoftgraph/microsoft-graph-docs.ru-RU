---
title: Канал исправлений
description: Обновление свойств указанного канала.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f31e4cb54c28cf2cfedae4f7c7fca8e95b62c44c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010159"
---
# <a name="patch-channel"></a><span data-ttu-id="cac0e-103">Канал исправлений</span><span class="sxs-lookup"><span data-stu-id="cac0e-103">Patch channel</span></span>

<span data-ttu-id="cac0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cac0e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cac0e-105">Обновление свойств указанного [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="cac0e-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cac0e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cac0e-106">Permissions</span></span>

<span data-ttu-id="cac0e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cac0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cac0e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cac0e-109">Permission type</span></span>      | <span data-ttu-id="cac0e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cac0e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cac0e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cac0e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cac0e-112">Чаннелсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cac0e-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="cac0e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cac0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cac0e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cac0e-114">Not supported.</span></span>    |
|<span data-ttu-id="cac0e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cac0e-115">Application</span></span> | <span data-ttu-id="cac0e-116">Чаннелсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cac0e-116">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="cac0e-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="cac0e-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="cac0e-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="cac0e-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cac0e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cac0e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cac0e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cac0e-120">Request headers</span></span>

| <span data-ttu-id="cac0e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cac0e-121">Header</span></span>       | <span data-ttu-id="cac0e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cac0e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cac0e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cac0e-123">Authorization</span></span>  | <span data-ttu-id="cac0e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cac0e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cac0e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cac0e-126">Content-Type</span></span>  | <span data-ttu-id="cac0e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cac0e-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cac0e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cac0e-128">Request body</span></span>

<span data-ttu-id="cac0e-129">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cac0e-129">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cac0e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="cac0e-130">Response</span></span>

<span data-ttu-id="cac0e-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cac0e-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cac0e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="cac0e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cac0e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="cac0e-133">Request</span></span>

<span data-ttu-id="cac0e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cac0e-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cac0e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="cac0e-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```
# <a name="objective-c"></a>[<span data-ttu-id="cac0e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cac0e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="cac0e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="cac0e-137">Response</span></span>

<span data-ttu-id="cac0e-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cac0e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

