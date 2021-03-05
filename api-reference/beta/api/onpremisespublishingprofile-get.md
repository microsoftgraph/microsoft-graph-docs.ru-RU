---
title: Get onPremisesPublishingProfile
description: Извлечение свойств и связей [объекта onPremisesPublishingProfile.](../resources/onpremisespublishingprofile.md)
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 3c2b3c6010970290a7416f3080e8d60d51799ff3
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471889"
---
# <a name="get-onpremisespublishingprofile"></a><span data-ttu-id="609b7-103">Get onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="609b7-103">Get onPremisesPublishingProfile</span></span>

<span data-ttu-id="609b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="609b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="609b7-105">Извлечение свойств и связей [объекта onPremisesPublishingProfile.](../resources/onpremisespublishingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="609b7-105">Retrieve the properties and relationships of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="609b7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="609b7-106">Permissions</span></span>

<span data-ttu-id="609b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="609b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="609b7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="609b7-109">Permission type</span></span>                        | <span data-ttu-id="609b7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="609b7-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="609b7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="609b7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="609b7-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="609b7-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="609b7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="609b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="609b7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="609b7-114">Not supported.</span></span> |
| <span data-ttu-id="609b7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="609b7-115">Application</span></span>                            | <span data-ttu-id="609b7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="609b7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="609b7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="609b7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="609b7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="609b7-118">Optional query parameters</span></span>

<span data-ttu-id="609b7-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="609b7-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="609b7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="609b7-120">Request headers</span></span>

| <span data-ttu-id="609b7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="609b7-121">Name</span></span>      |<span data-ttu-id="609b7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="609b7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="609b7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="609b7-123">Authorization</span></span> | <span data-ttu-id="609b7-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="609b7-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="609b7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="609b7-125">Request body</span></span>

<span data-ttu-id="609b7-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="609b7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="609b7-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="609b7-127">Response</span></span>

<span data-ttu-id="609b7-128">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="609b7-128">If successful, this method returns a `200 OK` response code and an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="609b7-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="609b7-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="609b7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="609b7-130">Request</span></span>

<span data-ttu-id="609b7-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="609b7-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="609b7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="609b7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onpremisespublishingprofile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning?$expand=publishedResources,agents,agentGroups
```
# <a name="c"></a>[<span data-ttu-id="609b7-133">C#</span><span class="sxs-lookup"><span data-stu-id="609b7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="609b7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="609b7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="609b7-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="609b7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="609b7-136">Java</span><span class="sxs-lookup"><span data-stu-id="609b7-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="609b7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="609b7-137">Response</span></span>

<span data-ttu-id="609b7-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="609b7-138">The following is an example of the response.</span></span>

> <span data-ttu-id="609b7-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="609b7-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
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



