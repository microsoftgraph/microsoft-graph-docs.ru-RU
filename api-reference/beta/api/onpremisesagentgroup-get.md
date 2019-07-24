---
title: Получение Онпремисесажентграуп
description: Получение свойств и связей объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4243f0e16d432d9756ec2f414aae23ad8ed4730b
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841145"
---
# <a name="get-onpremisesagentgroup"></a><span data-ttu-id="990e0-103">Получение Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="990e0-103">Get onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="990e0-104">Получение свойств и связей объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="990e0-104">Retrieve the properties and relationships of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="990e0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="990e0-105">Permissions</span></span>

<span data-ttu-id="990e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="990e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="990e0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="990e0-108">Permission type</span></span>                        | <span data-ttu-id="990e0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="990e0-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="990e0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="990e0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="990e0-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="990e0-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="990e0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="990e0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="990e0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="990e0-113">Not supported.</span></span> |
| <span data-ttu-id="990e0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="990e0-114">Application</span></span>                            | <span data-ttu-id="990e0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="990e0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="990e0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="990e0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="990e0-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="990e0-117">Optional query parameters</span></span>

<span data-ttu-id="990e0-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="990e0-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="990e0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="990e0-119">Request headers</span></span>

| <span data-ttu-id="990e0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="990e0-120">Name</span></span>      |<span data-ttu-id="990e0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="990e0-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="990e0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="990e0-122">Authorization</span></span> | <span data-ttu-id="990e0-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="990e0-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="990e0-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="990e0-124">Request body</span></span>

<span data-ttu-id="990e0-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="990e0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="990e0-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="990e0-126">Response</span></span>

<span data-ttu-id="990e0-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [онпремисесажентграуп](../resources/onpremisesagentgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="990e0-127">If successful, this method returns a `200 OK` response code and the requested [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="990e0-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="990e0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="990e0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="990e0-129">Request</span></span>

<span data-ttu-id="990e0-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="990e0-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onpremisesagentgroup"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/2d55ed41-1619-4848-92bb-0576d3038682/?$expand=publishedResources,agents
```

### <a name="response"></a><span data-ttu-id="990e0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="990e0-131">Response</span></span>

<span data-ttu-id="990e0-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="990e0-132">The following is an example of the response.</span></span>

> <span data-ttu-id="990e0-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="990e0-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
            "displayName": "Provisioning",
            "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
            "resourceName": "domain1.contoso.com"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
