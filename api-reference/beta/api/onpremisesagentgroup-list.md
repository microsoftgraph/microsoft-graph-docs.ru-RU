---
title: Список Онпремисесажентграупс
description: Получение списка объектов Онпремисесажентграуп.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 84177ae4054071fb60b6d323d034a6076eb8d9ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456464"
---
# <a name="list-onpremisesagentgroups"></a><span data-ttu-id="439e6-103">Список Онпремисесажентграупс</span><span class="sxs-lookup"><span data-stu-id="439e6-103">List onPremisesAgentGroups</span></span>

<span data-ttu-id="439e6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="439e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="439e6-105">Получение списка объектов [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="439e6-105">Retrieve a list of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="439e6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="439e6-106">Permissions</span></span>

<span data-ttu-id="439e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="439e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="439e6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="439e6-109">Permission type</span></span>                        | <span data-ttu-id="439e6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="439e6-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="439e6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="439e6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="439e6-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="439e6-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="439e6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="439e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="439e6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="439e6-114">Not supported.</span></span> |
| <span data-ttu-id="439e6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="439e6-115">Application</span></span>                            | <span data-ttu-id="439e6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="439e6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="439e6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="439e6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/agentGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="439e6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="439e6-118">Optional query parameters</span></span>

<span data-ttu-id="439e6-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="439e6-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="439e6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="439e6-120">Request headers</span></span>

| <span data-ttu-id="439e6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="439e6-121">Name</span></span>      |<span data-ttu-id="439e6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="439e6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="439e6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="439e6-123">Authorization</span></span> | <span data-ttu-id="439e6-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="439e6-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="439e6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="439e6-125">Request body</span></span>

<span data-ttu-id="439e6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="439e6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="439e6-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="439e6-127">Response</span></span>

<span data-ttu-id="439e6-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [онпремисесажентграуп](../resources/onpremisesagentgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="439e6-128">If successful, this method returns a `200 OK` response code and collection of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="439e6-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="439e6-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="439e6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="439e6-130">Request</span></span>

<span data-ttu-id="439e6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="439e6-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="439e6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="439e6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agentgroups"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups?$expand=agents,publishedResources
```
# <a name="c"></a>[<span data-ttu-id="439e6-133">C#</span><span class="sxs-lookup"><span data-stu-id="439e6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agentgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="439e6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="439e6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agentgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="439e6-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="439e6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agentgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="439e6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="439e6-136">Response</span></span>

<span data-ttu-id="439e6-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="439e6-137">The following is an example of the response.</span></span>

> <span data-ttu-id="439e6-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="439e6-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
            "id": "2d55ed41-1619-4848-92bb-0576d3038682",
            "displayName": "Group 1",
            "publishingType": "provisioning",
            "isDefault": false,
            "agents": [
                 {
                    "id": "1234b780-965f-4149-85c5-a8c73e58b67d",
                    "status": "Active"
                 }
            ],
            "publishedResources": [
                {
                    "displayName": "Demo Provisioning",
                    "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
                    "resourceName": "domain1.contoso.com"
                }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List agents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
