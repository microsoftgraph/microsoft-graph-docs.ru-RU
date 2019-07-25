---
title: Получение Онпремисеспублишингпрофиле
description: Получение свойств и связей объекта [онпремисеспублишингпрофиле](../resources/onpremisespublishingprofile.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fb3d6b43473ea1660976170625009ecea5c50baf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878444"
---
# <a name="get-onpremisespublishingprofile"></a><span data-ttu-id="d30d6-103">Получение Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="d30d6-103">Get onPremisesPublishingProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d30d6-104">Получение свойств и связей объекта [онпремисеспублишингпрофиле](../resources/onpremisespublishingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d30d6-104">Retrieve the properties and relationships of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d30d6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d30d6-105">Permissions</span></span>

<span data-ttu-id="d30d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d30d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d30d6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d30d6-108">Permission type</span></span>                        | <span data-ttu-id="d30d6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d30d6-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="d30d6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d30d6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d30d6-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d30d6-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="d30d6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d30d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d30d6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d30d6-113">Not supported.</span></span> |
| <span data-ttu-id="d30d6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d30d6-114">Application</span></span>                            | <span data-ttu-id="d30d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d30d6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d30d6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d30d6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d30d6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d30d6-117">Optional query parameters</span></span>

<span data-ttu-id="d30d6-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d30d6-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d30d6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d30d6-119">Request headers</span></span>

| <span data-ttu-id="d30d6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d30d6-120">Name</span></span>      |<span data-ttu-id="d30d6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d30d6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d30d6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d30d6-122">Authorization</span></span> | <span data-ttu-id="d30d6-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="d30d6-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d30d6-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d30d6-124">Request body</span></span>

<span data-ttu-id="d30d6-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d30d6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d30d6-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="d30d6-126">Response</span></span>

<span data-ttu-id="d30d6-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [онпремисеспублишингпрофиле](../resources/onpremisespublishingprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d30d6-127">If successful, this method returns a `200 OK` response code and an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d30d6-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="d30d6-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d30d6-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d30d6-129">Request</span></span>

<span data-ttu-id="d30d6-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d30d6-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d30d6-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="d30d6-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onpremisespublishingprofile"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning?$expand=publishedResources,agents,agentGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d30d6-132">C#</span><span class="sxs-lookup"><span data-stu-id="d30d6-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d30d6-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="d30d6-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d30d6-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d30d6-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d30d6-135">Java</span><span class="sxs-lookup"><span data-stu-id="d30d6-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d30d6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d30d6-136">Response</span></span>

<span data-ttu-id="d30d6-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d30d6-137">The following is an example of the response.</span></span>

> <span data-ttu-id="d30d6-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d30d6-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
