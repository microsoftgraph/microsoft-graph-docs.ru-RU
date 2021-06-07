---
title: Get onPremisesPublishingProfile
description: Извлечение свойств и связей [объекта onPremisesPublishingProfile.](../resources/onpremisespublishingprofile.md)
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: e6dd4e1f3cba64236e438063b259906ea5a9ac15
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781011"
---
# <a name="get-onpremisespublishingprofile"></a><span data-ttu-id="ce68f-103">Get onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="ce68f-103">Get onPremisesPublishingProfile</span></span>

<span data-ttu-id="ce68f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce68f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce68f-105">Извлечение свойств и связей [объекта onPremisesPublishingProfile.](../resources/onpremisespublishingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ce68f-105">Retrieve the properties and relationships of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce68f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce68f-106">Permissions</span></span>

<span data-ttu-id="ce68f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce68f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce68f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce68f-109">Permission type</span></span>                        | <span data-ttu-id="ce68f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce68f-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="ce68f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce68f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce68f-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce68f-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="ce68f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce68f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce68f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce68f-114">Not supported.</span></span> |
| <span data-ttu-id="ce68f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce68f-115">Application</span></span>                            | <span data-ttu-id="ce68f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce68f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce68f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce68f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce68f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ce68f-118">Optional query parameters</span></span>

<span data-ttu-id="ce68f-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ce68f-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce68f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce68f-120">Request headers</span></span>

| <span data-ttu-id="ce68f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ce68f-121">Name</span></span>      |<span data-ttu-id="ce68f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ce68f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce68f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce68f-123">Authorization</span></span> | <span data-ttu-id="ce68f-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ce68f-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce68f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce68f-125">Request body</span></span>

<span data-ttu-id="ce68f-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce68f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce68f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce68f-127">Response</span></span>

<span data-ttu-id="ce68f-128">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ce68f-128">If successful, this method returns a `200 OK` response code and an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce68f-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="ce68f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce68f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce68f-130">Request</span></span>

<span data-ttu-id="ce68f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce68f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce68f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce68f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onpremisespublishingprofile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning?$expand=publishedResources,agents,agentGroups
```
# <a name="c"></a>[<span data-ttu-id="ce68f-133">C#</span><span class="sxs-lookup"><span data-stu-id="ce68f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onpremisespublishingprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce68f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce68f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onpremisespublishingprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce68f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce68f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onpremisespublishingprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce68f-136">Java</span><span class="sxs-lookup"><span data-stu-id="ce68f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onpremisespublishingprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ce68f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce68f-137">Response</span></span>

<span data-ttu-id="ce68f-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ce68f-138">The following is an example of the response.</span></span>

> <span data-ttu-id="ce68f-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ce68f-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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



