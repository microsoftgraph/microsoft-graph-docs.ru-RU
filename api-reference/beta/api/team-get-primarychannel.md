---
title: Получение primaryChannel
description: Получение свойства навигации команды, разрешающего доступ к стандартному каналу "Общий".
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 87b68bc313fbfc03e9ab52d8e9a77ea8b4fbebab
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050817"
---
# <a name="get-primarychannel"></a><span data-ttu-id="73d7e-103">Получение primaryChannel</span><span class="sxs-lookup"><span data-stu-id="73d7e-103">Get primaryChannel</span></span>

<span data-ttu-id="73d7e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73d7e-104">Namespace: microsoft.graph</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73d7e-105">Получение стандартного [канала](../resources/channel.md) (**Общий**) [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="73d7e-105">Get the default [channel](../resources/channel.md), **General**, of a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="73d7e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73d7e-106">Permissions</span></span>
<span data-ttu-id="73d7e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73d7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73d7e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73d7e-109">Permission type</span></span>      | <span data-ttu-id="73d7e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73d7e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73d7e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73d7e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="73d7e-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73d7e-112">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="73d7e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73d7e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73d7e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73d7e-114">Not supported.</span></span>    |
|<span data-ttu-id="73d7e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73d7e-115">Application</span></span> | <span data-ttu-id="73d7e-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73d7e-116">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span></span> |

> <span data-ttu-id="73d7e-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="73d7e-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="73d7e-p102">**Примечание**. Этот API поддерживает разрешения администратора. Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="73d7e-p102">**Note**: This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="73d7e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73d7e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/primaryChannel
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73d7e-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="73d7e-121">Optional query parameters</span></span>

<span data-ttu-id="73d7e-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="73d7e-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73d7e-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73d7e-123">Request headers</span></span>
| <span data-ttu-id="73d7e-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73d7e-124">Header</span></span>       | <span data-ttu-id="73d7e-125">Значение</span><span class="sxs-lookup"><span data-stu-id="73d7e-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="73d7e-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73d7e-126">Authorization</span></span>  | <span data-ttu-id="73d7e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73d7e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="73d7e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73d7e-129">Request body</span></span>
<span data-ttu-id="73d7e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73d7e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73d7e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="73d7e-131">Response</span></span>

<span data-ttu-id="73d7e-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [channel](../resources/channel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73d7e-132">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73d7e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="73d7e-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="73d7e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="73d7e-134">Request</span></span>
<span data-ttu-id="73d7e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73d7e-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="73d7e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="73d7e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_primaryChannel"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/primaryChannel
```
# <a name="c"></a>[<span data-ttu-id="73d7e-137">C#</span><span class="sxs-lookup"><span data-stu-id="73d7e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-primarychannel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73d7e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73d7e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-primarychannel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73d7e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73d7e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-primarychannel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73d7e-140">Java</span><span class="sxs-lookup"><span data-stu-id="73d7e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-primarychannel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="73d7e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="73d7e-141">Response</span></span>
<span data-ttu-id="73d7e-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="73d7e-142">The following is an example of the response.</span></span> 

><span data-ttu-id="73d7e-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="73d7e-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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


