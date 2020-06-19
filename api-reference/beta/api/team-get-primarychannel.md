---
title: Получение Примаричаннел
description: Получение свойства навигации команды, позволяющей получить доступ к общему каналу по умолчанию.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8c9be54f744e596b41de1d2e994dfe51b0c95e6d
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791099"
---
# <a name="get-primarychannel"></a><span data-ttu-id="f8904-103">Получение Примаричаннел</span><span class="sxs-lookup"><span data-stu-id="f8904-103">Get primaryChannel</span></span>

<span data-ttu-id="f8904-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8904-104">Namespace: microsoft.graph</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8904-105">Получение свойства навигации [команды](../resources/team.md) , предоставляющей доступ к общему [каналу](../resources/channel.md)по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f8904-105">Retrieve the navigation property of a [team](../resources/team.md) that allows access to the default General [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8904-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8904-106">Permissions</span></span>
<span data-ttu-id="f8904-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f8904-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f8904-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8904-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8904-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8904-109">Permission type</span></span>      | <span data-ttu-id="f8904-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8904-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8904-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8904-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f8904-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8904-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f8904-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8904-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8904-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8904-114">Not supported.</span></span>    |
|<span data-ttu-id="f8904-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8904-115">Application</span></span> | <span data-ttu-id="f8904-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8904-116">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="f8904-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="f8904-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f8904-118">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="f8904-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f8904-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8904-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/primaryChannel

```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8904-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f8904-120">Optional query parameters</span></span>

<span data-ttu-id="f8904-121">Этот метод поддерживает `$filter` `$select` `$expand` [Параметры запроса](/graph/query-parameters) , и OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f8904-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8904-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8904-122">Request headers</span></span>
| <span data-ttu-id="f8904-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8904-123">Header</span></span>       | <span data-ttu-id="f8904-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f8904-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f8904-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8904-125">Authorization</span></span>  | <span data-ttu-id="f8904-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="f8904-126">Bearer {token}.</span></span> <span data-ttu-id="f8904-127">Required.</span><span class="sxs-lookup"><span data-stu-id="f8904-127">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f8904-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f8904-128">Request body</span></span>
<span data-ttu-id="f8904-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f8904-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8904-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8904-130">Response</span></span>

<span data-ttu-id="f8904-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f8904-131">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8904-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f8904-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8904-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8904-133">Request</span></span>
<span data-ttu-id="f8904-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8904-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_primaryChannel"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/primaryChannel
```
### <a name="response"></a><span data-ttu-id="f8904-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8904-135">Response</span></span>
<span data-ttu-id="f8904-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f8904-136">The following is an example of the response.</span></span> 

><span data-ttu-id="f8904-137">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="f8904-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f8904-138">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f8904-138">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('32e3b156-66b2-4135-9aeb-73295a35a55b')/primaryChannel/$entity",
    "id": "19:skypespaces_dd1e128ffa85453ab1f3015468e979d5@thread.skype",
    "displayName": "General",
    "description": "Microsoft Teams Platform team discussions",
    "isFavoriteByDefault": null,
    "email": "0686dc7a.microsoft.com@amer.teams.ms",
    "webUrl": "https://teams.microsoft.com/l/channel/19%3askypespaces_dd1e128ffa85453ab1f3015468e979d5%40thread.skype/General?groupId=32e3b156-66b2-4135-9aeb-73295a35a55b&tenantId=72f988bf-86f1-41af-91ab-2d7cd011db47",
    "membershipType": "standard"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "get primaryChannel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
