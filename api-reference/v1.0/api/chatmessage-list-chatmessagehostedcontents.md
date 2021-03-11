---
title: Список chatMessageHostedContents
description: Извлечение списка объектов chatMessageHostedContent из сообщения.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 16dc59427eeab168d816780c9fcdc5c6603a1955
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50634317"
---
# <a name="list-hostedcontents"></a><span data-ttu-id="cf2bc-103">Список hostedContents</span><span class="sxs-lookup"><span data-stu-id="cf2bc-103">List hostedContents</span></span>

<span data-ttu-id="cf2bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf2bc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cf2bc-105">Извлечение списка [объектов chatMessageHostedContent](../resources/chatmessagehostedcontent.md) из сообщения.</span><span class="sxs-lookup"><span data-stu-id="cf2bc-105">Retrieve the list of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects from a message.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf2bc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf2bc-106">Permissions</span></span>

<span data-ttu-id="cf2bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf2bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf2bc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf2bc-109">Permission type</span></span>                        | <span data-ttu-id="cf2bc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf2bc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="cf2bc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf2bc-111">Delegated (work or school account)</span></span>| <span data-ttu-id="cf2bc-112">Для **ресурса** канала: ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf2bc-112">For **channel** resource: ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="cf2bc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf2bc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf2bc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf2bc-114">Not supported.</span></span>|
|<span data-ttu-id="cf2bc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf2bc-115">Application</span></span>| <span data-ttu-id="cf2bc-116">Для **ресурса** канала: ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf2bc-116">For **channel** resource: ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span> |

> <span data-ttu-id="cf2bc-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="cf2bc-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="cf2bc-118">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="cf2bc-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="cf2bc-119">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="cf2bc-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="cf2bc-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf2bc-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/hostedContents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf2bc-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cf2bc-121">Optional query parameters</span></span>

<span data-ttu-id="cf2bc-122">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cf2bc-122">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf2bc-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf2bc-123">Request headers</span></span>

| <span data-ttu-id="cf2bc-124">Имя</span><span class="sxs-lookup"><span data-stu-id="cf2bc-124">Name</span></span>      |<span data-ttu-id="cf2bc-125">Описание</span><span class="sxs-lookup"><span data-stu-id="cf2bc-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cf2bc-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf2bc-126">Authorization</span></span> | <span data-ttu-id="cf2bc-127">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="cf2bc-127">Bearer {code}.</span></span> <span data-ttu-id="cf2bc-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="cf2bc-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf2bc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf2bc-129">Request body</span></span>

<span data-ttu-id="cf2bc-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf2bc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf2bc-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf2bc-131">Response</span></span>

<span data-ttu-id="cf2bc-132">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cf2bc-132">If successful, this method returns a `200 OK` response code and a collection of [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cf2bc-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="cf2bc-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cf2bc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf2bc-134">Request</span></span>

<span data-ttu-id="cf2bc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf2bc-135">The following is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1614618259349/hostedContents
```

### <a name="response"></a><span data-ttu-id="cf2bc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf2bc-136">Response</span></span>

<span data-ttu-id="cf2bc-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cf2bc-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="cf2bc-138">Объект отклика, показанный здесь, может быть сокращен для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf2bc-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cf2bc-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf2bc-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1614618259349')/hostedContents",
    "@odata.count": 1,
    "value": [
        {
            "id": "aWQ9eF8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNSx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNS92aWV3cy9pbWdv",
            "contentBytes": null,
            "contentType": null
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List hostedContents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


