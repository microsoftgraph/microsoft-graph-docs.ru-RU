---
title: Получение канала
description: Получение свойств и связей канала.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8b08832ca7bcb02b62765c69ad1312753306f908
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289091"
---
# <a name="get-channel"></a><span data-ttu-id="1385e-103">Получение канала</span><span class="sxs-lookup"><span data-stu-id="1385e-103">Get channel</span></span>

<span data-ttu-id="1385e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1385e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1385e-105">Получение свойств и связей [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="1385e-105">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1385e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1385e-106">Permissions</span></span>

<span data-ttu-id="1385e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1385e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1385e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1385e-109">Permission type</span></span>      | <span data-ttu-id="1385e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1385e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1385e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1385e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1385e-112">Channel. ReadBasic. ALL, Чаннелсеттингс. Read. ALL, Чаннелсеттингс. ReadWrite. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1385e-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="1385e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1385e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1385e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1385e-114">Not supported.</span></span>    |
|<span data-ttu-id="1385e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1385e-115">Application</span></span> | <span data-ttu-id="1385e-116">Channel. ReadBasic. ALL, Чаннелсеттингс. Read. ALL, Чаннелсеттингс. ReadWrite. ALL, Чаннелсеттингс. Read. Group ([RSC](https://aka.ms/teams-rsc)), Чаннелсеттингс. Edit. Group ([RSC](https://aka.ms/teams-rsc)), Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1385e-116">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, ChannelSettings.Read.Group ([RSC](https://aka.ms/teams-rsc)), ChannelSettings.Edit.Group ([RSC](https://aka.ms/teams-rsc)), Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |

> <span data-ttu-id="1385e-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="1385e-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1385e-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="1385e-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1385e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1385e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="1385e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1385e-120">Optional query parameters</span></span>

<span data-ttu-id="1385e-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) $filter, $select и $expand для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1385e-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1385e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1385e-122">Request headers</span></span>

| <span data-ttu-id="1385e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1385e-123">Header</span></span>       | <span data-ttu-id="1385e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="1385e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1385e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1385e-125">Authorization</span></span>  | <span data-ttu-id="1385e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1385e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1385e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1385e-128">Request body</span></span>

<span data-ttu-id="1385e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1385e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1385e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1385e-130">Response</span></span>

<span data-ttu-id="1385e-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1385e-131">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1385e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1385e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1385e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1385e-133">Request</span></span>

<span data-ttu-id="1385e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1385e-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1385e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1385e-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```

# <a name="c"></a>[<span data-ttu-id="1385e-136">C#</span><span class="sxs-lookup"><span data-stu-id="1385e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1385e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1385e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1385e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1385e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="1385e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1385e-139">Response</span></span>

<span data-ttu-id="1385e-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1385e-140">Here is an example of the response.</span></span>

><span data-ttu-id="1385e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1385e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "id": "id-value",
    "membershipType": "membership-type-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
