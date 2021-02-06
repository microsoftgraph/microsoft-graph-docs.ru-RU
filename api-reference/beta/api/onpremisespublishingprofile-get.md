---
title: Get onPremisesPublishingProfile
description: Извлечение свойств и связей объекта [onPremisesPublishingProfile.](../resources/onpremisespublishingprofile.md)
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: b7eec602f502f1501b8cfab96a5cc0de0c2faa8c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136369"
---
# <a name="get-onpremisespublishingprofile"></a><span data-ttu-id="eb1ea-103">Get onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="eb1ea-103">Get onPremisesPublishingProfile</span></span>

<span data-ttu-id="eb1ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb1ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb1ea-105">Извлечение свойств и связей объекта [onPremisesPublishingProfile.](../resources/onpremisespublishingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="eb1ea-105">Retrieve the properties and relationships of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb1ea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb1ea-106">Permissions</span></span>

<span data-ttu-id="eb1ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb1ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eb1ea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb1ea-109">Permission type</span></span>                        | <span data-ttu-id="eb1ea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb1ea-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="eb1ea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb1ea-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb1ea-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb1ea-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="eb1ea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb1ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb1ea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb1ea-114">Not supported.</span></span> |
| <span data-ttu-id="eb1ea-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb1ea-115">Application</span></span>                            | <span data-ttu-id="eb1ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb1ea-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb1ea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb1ea-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb1ea-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eb1ea-118">Optional query parameters</span></span>

<span data-ttu-id="eb1ea-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="eb1ea-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb1ea-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb1ea-120">Request headers</span></span>

| <span data-ttu-id="eb1ea-121">Имя</span><span class="sxs-lookup"><span data-stu-id="eb1ea-121">Name</span></span>      |<span data-ttu-id="eb1ea-122">Описание</span><span class="sxs-lookup"><span data-stu-id="eb1ea-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eb1ea-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb1ea-123">Authorization</span></span> | <span data-ttu-id="eb1ea-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="eb1ea-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb1ea-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb1ea-125">Request body</span></span>

<span data-ttu-id="eb1ea-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb1ea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb1ea-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb1ea-127">Response</span></span>

<span data-ttu-id="eb1ea-128">В случае успеха этот метод возвращает код отклика и объект `200 OK` [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eb1ea-128">If successful, this method returns a `200 OK` response code and an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb1ea-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="eb1ea-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb1ea-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb1ea-130">Request</span></span>

<span data-ttu-id="eb1ea-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb1ea-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eb1ea-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb1ea-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onpremisespublishingprofile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning?$expand=publishedResources,agents,agentGroups
```
# <a name="c"></a>[<span data-ttu-id="eb1ea-133">C#</span><span class="sxs-lookup"><span data-stu-id="eb1ea-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb1ea-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb1ea-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb1ea-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb1ea-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb1ea-136">Java</span><span class="sxs-lookup"><span data-stu-id="eb1ea-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb1ea-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb1ea-137">Response</span></span>

<span data-ttu-id="eb1ea-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eb1ea-138">The following is an example of the response.</span></span>

> <span data-ttu-id="eb1ea-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eb1ea-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```json
HTTP/1.1 200 OK

{
    "publishedResources": [
        {
            "publishingType": "provisioning",
            "displayName": "Demo Provisioning",
            "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
            "resourceName": "domain1.contoso.com",
            "agentGroups": [
                {
                    "id": "2d55ed41-1619-4848-92bb-0576d3038682",
                    "displayName": "Group 1"
                }
            ]
        }
    ],
    "agents": [
        {
            "id": "1234b780-965f-4149-85c5-a8c73e58b67d",
            "status": "Active",
            "machineName": "server 1",
            "externalIp": "1.0.0.127",
            "agentGroups": [
                 {
                    "id": "2d55ed41-1619-4848-92bb-0576d3038682",
                    "displayName": "Group 1"
                 }
            ]
        }
    ],
    "agentGroups": [
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
    ],
  "hybridAgentUpdaterConfiguration": {
       "deferUpdateDateTime" : "2018-08-12T12:00",
       "updateWindow" :
          {
            "updateWindowStartTime" : "0:00:00",
            "updateWindowEndTime" : "23:59:00.0000000"
          },
       "allowUpdateConfigurationOverride" : false
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onPremisesPublishingProfile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



