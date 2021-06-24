---
title: Get serviceHealth
description: Извлечение свойств и связей объекта serviceHealth.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: f36a4f1787415956c486d2ed74a3ab0acb327c88
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107871"
---
# <a name="get-servicehealth"></a><span data-ttu-id="4ec1e-103">Get serviceHealth</span><span class="sxs-lookup"><span data-stu-id="4ec1e-103">Get serviceHealth</span></span>
<span data-ttu-id="4ec1e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ec1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ec1e-105">Извлечение свойств и связей объекта [serviceHealth.](../resources/servicehealth.md)</span><span class="sxs-lookup"><span data-stu-id="4ec1e-105">Retrieve the properties and relationships of a [serviceHealth](../resources/servicehealth.md) object.</span></span>

<span data-ttu-id="4ec1e-106">Эта операция предоставляет сведения о состоянии здоровья указанной службы для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ec1e-106">This operation provides the health information of a specified service for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ec1e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ec1e-107">Permissions</span></span>
<span data-ttu-id="4ec1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ec1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ec1e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ec1e-110">Permission type</span></span>|<span data-ttu-id="4ec1e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ec1e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ec1e-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ec1e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ec1e-113">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ec1e-113">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="4ec1e-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ec1e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ec1e-115">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ec1e-115">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="4ec1e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4ec1e-116">Application</span></span>|<span data-ttu-id="4ec1e-117">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ec1e-117">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ec1e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ec1e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /admin/serviceAnnouncement/healthOverviews/{ServiceName}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ec1e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4ec1e-119">Optional query parameters</span></span>
<span data-ttu-id="4ec1e-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4ec1e-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ec1e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ec1e-121">Request headers</span></span>
|<span data-ttu-id="4ec1e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4ec1e-122">Name</span></span>|<span data-ttu-id="4ec1e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4ec1e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4ec1e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ec1e-124">Authorization</span></span>|<span data-ttu-id="4ec1e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ec1e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ec1e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ec1e-127">Request body</span></span>
<span data-ttu-id="4ec1e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ec1e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ec1e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ec1e-129">Response</span></span>

<span data-ttu-id="4ec1e-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [serviceHealth](../resources/servicehealth.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4ec1e-130">If successful, this method returns a `200 OK` response code and a [serviceHealth](../resources/servicehealth.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4ec1e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="4ec1e-131">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-servicehealth-object"></a><span data-ttu-id="4ec1e-132">Пример 1. Получить свойства объекта serviceHealth</span><span class="sxs-lookup"><span data-stu-id="4ec1e-132">Example 1: Get the properties of a serviceHealth object</span></span>

#### <a name="request"></a><span data-ttu-id="4ec1e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ec1e-133">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["Microsoft 365 suite"],
  "name": "get_servicehealth"
}
-->

``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews/Microsoft 365 suite
```

#### <a name="response"></a><span data-ttu-id="4ec1e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ec1e-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealth"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/healthOverviews/$entity",
    "service": "Microsoft 365 suite",
    "status": "RestoringService",
    "id": "OSDPPlatform"
}
```

### <a name="example-2-include-navigation-property-issues"></a><span data-ttu-id="4ec1e-135">Пример 2. Включаем проблемы свойств навигации</span><span class="sxs-lookup"><span data-stu-id="4ec1e-135">Example 2: Include navigation property issues</span></span>

#### <a name="request"></a><span data-ttu-id="4ec1e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ec1e-136">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["Microsoft 365 suite"],
  "name": "get_servicehealth_with_issues"
}
-->

``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews/Microsoft 365 suite?$expand=issues
```

#### <a name="response"></a><span data-ttu-id="4ec1e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ec1e-137">Response</span></span>
><span data-ttu-id="4ec1e-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4ec1e-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealth"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/healthOverviews(issues())/$entity",
  "service": "Microsoft 365 suite",
  "status": "ServiceOperational",
  "id": "OSDPPlatform",
  "issues": [
        {
          "startDateTime": "2020-11-04T00:00:00Z",
          "endDateTime": "2020-11-20T17:00:00Z",
          "lastModifiedDateTime": "2020-11-20T17:56:31.39Z",
          "title": "Intermittently unable to access some Microsoft 365 services",
          "id": "MO226574",
          "impactDescription": "Users may have been intermittently unable to access some Microsoft 365 services.",
          "classification": "Advisory",
          "origin": "Microsoft",
          "status": "ServiceRestored",
          "service": "Exchange Online",
          "feature": "Tenant Administration (Provisioning, Remote PowerShell)",
          "featureGroup": "Management and Provisioning",
          "isResolved": true,
          "details": [],
          "posts": [
              {
                "createdDateTime": "2020-11-12T07:07:38.97Z",
                "postType": "Regular",
                "description": {
                    "contentType": "Text",
                    "content": "Users may have been intermittently unable to access some Microsoft 365 services. We'll provide an update within 30 minutes."
                  }
              }
          ]
        }
    ]
}
```