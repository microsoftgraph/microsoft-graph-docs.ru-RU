---
title: Канал исправлений
description: Обновление свойств указанного канала.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 68265b319fd567097b72c9eaad82275fd3faefab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518604"
---
# <a name="patch-channel"></a><span data-ttu-id="aae44-103">Канал исправлений</span><span class="sxs-lookup"><span data-stu-id="aae44-103">Patch channel</span></span>

<span data-ttu-id="aae44-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aae44-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aae44-105">Обновление свойств указанного [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="aae44-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="aae44-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aae44-106">Permissions</span></span>

<span data-ttu-id="aae44-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aae44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aae44-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aae44-109">Permission type</span></span>      | <span data-ttu-id="aae44-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aae44-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aae44-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aae44-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aae44-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aae44-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="aae44-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aae44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aae44-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aae44-114">Not supported.</span></span>    |
|<span data-ttu-id="aae44-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aae44-115">Application</span></span> | <span data-ttu-id="aae44-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aae44-116">Group.ReadWrite.All</span></span> |

> <span data-ttu-id="aae44-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="aae44-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="aae44-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="aae44-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="aae44-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aae44-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```

## <a name="request-headers"></a><span data-ttu-id="aae44-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aae44-120">Request headers</span></span>

| <span data-ttu-id="aae44-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aae44-121">Header</span></span>       | <span data-ttu-id="aae44-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aae44-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aae44-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aae44-123">Authorization</span></span>  | <span data-ttu-id="aae44-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aae44-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="aae44-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aae44-126">Content-Type</span></span>  | <span data-ttu-id="aae44-127">application/json</span><span class="sxs-lookup"><span data-stu-id="aae44-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aae44-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aae44-128">Request body</span></span>

<span data-ttu-id="aae44-129">Предоставьте в тексте запроса описание объекта [channel](../resources/channel.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aae44-129">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="aae44-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="aae44-130">Response</span></span>

<span data-ttu-id="aae44-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="aae44-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aae44-132">Пример</span><span class="sxs-lookup"><span data-stu-id="aae44-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="aae44-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="aae44-133">Request</span></span>

<span data-ttu-id="aae44-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aae44-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aae44-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="aae44-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```
# <a name="objective-c"></a>[<span data-ttu-id="aae44-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aae44-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="aae44-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="aae44-137">Response</span></span>

<span data-ttu-id="aae44-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aae44-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
