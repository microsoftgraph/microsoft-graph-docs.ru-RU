---
title: Получение канала
description: Получение свойств и связей канала.
author: nkramer
doc_type: apiPageType
ms.prod: microsoft-teams
localization_priority: Normal
ms.openlocfilehash: a7be2c2b5fe3db44e8c514f39731a56d859e1ce2
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202900"
---
# <a name="get-channel"></a><span data-ttu-id="94e71-103">Получение канала</span><span class="sxs-lookup"><span data-stu-id="94e71-103">Get channel</span></span>

<span data-ttu-id="94e71-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94e71-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94e71-105">Получение свойств и связей [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="94e71-105">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94e71-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94e71-106">Permissions</span></span>

<span data-ttu-id="94e71-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94e71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94e71-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94e71-109">Permission type</span></span>      | <span data-ttu-id="94e71-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94e71-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94e71-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94e71-111">Delegated (work or school account)</span></span> | <span data-ttu-id="94e71-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94e71-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="94e71-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94e71-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94e71-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94e71-114">Not supported.</span></span>    |
|<span data-ttu-id="94e71-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94e71-115">Application</span></span> | <span data-ttu-id="94e71-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94e71-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="94e71-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="94e71-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="94e71-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="94e71-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="94e71-119">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="94e71-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="94e71-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94e71-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94e71-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="94e71-121">Optional query parameters</span></span>

<span data-ttu-id="94e71-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="94e71-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94e71-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94e71-123">Request headers</span></span>

| <span data-ttu-id="94e71-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="94e71-124">Header</span></span>       | <span data-ttu-id="94e71-125">Значение</span><span class="sxs-lookup"><span data-stu-id="94e71-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="94e71-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94e71-126">Authorization</span></span>  | <span data-ttu-id="94e71-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94e71-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="94e71-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94e71-129">Request body</span></span>

<span data-ttu-id="94e71-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94e71-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94e71-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="94e71-131">Response</span></span>

<span data-ttu-id="94e71-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="94e71-132">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94e71-133">Пример</span><span class="sxs-lookup"><span data-stu-id="94e71-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="94e71-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="94e71-134">Request</span></span>

<span data-ttu-id="94e71-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94e71-135">Here is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->

```http
GET https://graph.microsoft.com/v1.0/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
```


### <a name="response"></a><span data-ttu-id="94e71-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="94e71-136">Response</span></span>

<span data-ttu-id="94e71-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="94e71-137">Here is an example of the response.</span></span>

><span data-ttu-id="94e71-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="94e71-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "id": "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2",
    "createdDateTime": "2020-05-27T19:22:25.692Z",
    "displayName": "General",
    "description": "AutoTestTeam_20210311_150740.2550_fim3udfdjen9",
    "membershipType": "standard"
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
