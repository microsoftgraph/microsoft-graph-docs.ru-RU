---
title: Получение Онпремисесажент
description: Получение свойств и связей объекта Онпремисесажент.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ba647ac06afdc91b812cf87b962013f5572320e1
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726013"
---
# <a name="get-onpremisesagent"></a><span data-ttu-id="e1e19-103">Получение Онпремисесажент</span><span class="sxs-lookup"><span data-stu-id="e1e19-103">Get onPremisesAgent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1e19-104">Получение свойств и связей объекта [онпремисесажент](../resources/onpremisesagent.md) .</span><span class="sxs-lookup"><span data-stu-id="e1e19-104">Retrieve the properties and relationships of an [onPremisesAgent](../resources/onpremisesagent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1e19-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1e19-105">Permissions</span></span>

<span data-ttu-id="e1e19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1e19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1e19-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1e19-108">Permission type</span></span>                        | <span data-ttu-id="e1e19-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1e19-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1e19-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1e19-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1e19-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e1e19-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="e1e19-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1e19-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1e19-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1e19-113">Not supported.</span></span> |
| <span data-ttu-id="e1e19-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1e19-114">Application</span></span>                            | <span data-ttu-id="e1e19-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1e19-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1e19-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1e19-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/agents/{id1}/?$expand=agentGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1e19-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e1e19-117">Optional query parameters</span></span>

<span data-ttu-id="e1e19-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e1e19-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1e19-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1e19-119">Request headers</span></span>

| <span data-ttu-id="e1e19-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e1e19-120">Name</span></span>      |<span data-ttu-id="e1e19-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e1e19-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e1e19-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1e19-122">Authorization</span></span> | <span data-ttu-id="e1e19-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="e1e19-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1e19-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e1e19-124">Request body</span></span>

<span data-ttu-id="e1e19-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1e19-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1e19-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1e19-126">Response</span></span>

<span data-ttu-id="e1e19-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [онпремисесажент](../resources/onpremisesagent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1e19-127">If successful, this method returns a `200 OK` response code and an [onPremisesAgent](../resources/onpremisesagent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1e19-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="e1e19-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e1e19-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1e19-129">Request</span></span>

<span data-ttu-id="e1e19-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1e19-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e1e19-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1e19-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onpremisesagent"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/?$expand=agentGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e1e19-132">C#</span><span class="sxs-lookup"><span data-stu-id="e1e19-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onpremisesagent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1e19-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1e19-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e1e19-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e1e19-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e1e19-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1e19-135">Response</span></span>

<span data-ttu-id="e1e19-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e1e19-136">The following is an example of the response.</span></span>

> <span data-ttu-id="e1e19-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1e19-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgent"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "1234b780-965f-4149-85c5-a8c73e58b67d",
    "status": "Active",
    "machineName": "server1.local1.contoso.com",
    "externalIp": "153.69.23.122",
    "agentGroups": [
         {
            "id": "2d55ed41-1619-4848-92bb-0576d3038682",
            "displayName": "Group 1"
         }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onPremisesAgent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
