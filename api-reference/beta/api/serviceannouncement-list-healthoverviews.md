---
title: Список healthOverviews
description: Извлекать ресурсы serviceHealth из свойства навигации healthOverviews.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 3519620b9decc83596fbe9222eed4b9b24d84ac0
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109172"
---
# <a name="list-healthoverviews"></a><span data-ttu-id="8edb2-103">Список healthOverviews</span><span class="sxs-lookup"><span data-stu-id="8edb2-103">List healthOverviews</span></span>
<span data-ttu-id="8edb2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8edb2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8edb2-105">Извлекать [ресурсы serviceHealth](../resources/servicehealth.md) из **свойства навигации healthOverviews.**</span><span class="sxs-lookup"><span data-stu-id="8edb2-105">Retrieve the [serviceHealth](../resources/servicehealth.md) resources from the **healthOverviews** navigation property.</span></span>

<span data-ttu-id="8edb2-106">Эта операция предоставляет отчет о состоянии здоровья всех подписаных служб для клиента.</span><span class="sxs-lookup"><span data-stu-id="8edb2-106">This operation provides the health report of all subscribed services for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="8edb2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8edb2-107">Permissions</span></span>
<span data-ttu-id="8edb2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8edb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8edb2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8edb2-110">Permission type</span></span>|<span data-ttu-id="8edb2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8edb2-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8edb2-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8edb2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8edb2-113">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="8edb2-113">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="8edb2-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8edb2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8edb2-115">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="8edb2-115">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="8edb2-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8edb2-116">Application</span></span>|<span data-ttu-id="8edb2-117">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="8edb2-117">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8edb2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8edb2-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/healthOverviews
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8edb2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8edb2-119">Optional query parameters</span></span>
<span data-ttu-id="8edb2-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8edb2-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8edb2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8edb2-121">Request headers</span></span>
|<span data-ttu-id="8edb2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8edb2-122">Name</span></span>|<span data-ttu-id="8edb2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8edb2-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8edb2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8edb2-124">Authorization</span></span>|<span data-ttu-id="8edb2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8edb2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8edb2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8edb2-127">Request body</span></span>
<span data-ttu-id="8edb2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8edb2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8edb2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8edb2-129">Response</span></span>

<span data-ttu-id="8edb2-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [serviceHealth](../resources/servicehealth.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8edb2-130">If successful, this method returns a `200 OK` response code and a collection of [serviceHealth](../resources/servicehealth.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8edb2-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="8edb2-131">Examples</span></span>

### <a name="example-1-get-servicehealth-resources"></a><span data-ttu-id="8edb2-132">Пример 1. Получить ресурсы serviceHealth</span><span class="sxs-lookup"><span data-stu-id="8edb2-132">Example 1: Get serviceHealth resources</span></span>

#### <a name="request"></a><span data-ttu-id="8edb2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8edb2-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_healthoverviews"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews
```

#### <a name="response"></a><span data-ttu-id="8edb2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8edb2-134">Response</span></span>
><span data-ttu-id="8edb2-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8edb2-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealth",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/healthOverviews",
  "value": [
    {
        "service": "Exchange Online",
        "status": "ServicaOperational",
        "id": "Exchange"
    },
    {
        "service": "Identity Service",
        "status": "ServiceRestored",
        "id": "OrgLiveID"
    },
    {
        "service": "Microsoft 365 suite",
        "status": "ServiceOperational",
        "id": "OSDPPlatform"
    }
  ]
}
```

### <a name="example-2-include-navigation-property-issues"></a><span data-ttu-id="8edb2-136">Пример 2. Включаем проблемы свойств навигации</span><span class="sxs-lookup"><span data-stu-id="8edb2-136">Example 2: Include navigation property issues</span></span>

#### <a name="request"></a><span data-ttu-id="8edb2-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="8edb2-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_healthoverviews_with_issues"
}
-->

``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews?$expand=issues
```

#### <a name="response"></a><span data-ttu-id="8edb2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8edb2-138">Response</span></span>
><span data-ttu-id="8edb2-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8edb2-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealth",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/healthOverviews(issues())",
  "value": [
    {
      "service": "Exchange Online",
      "status": "ServiceOperational",
      "id": "Exchange",
      "issues": [
          {
              "startDateTime": "2020-11-04T00:00:00Z",
              "endDateTime": "2020-11-20T17:00:00Z",
              "lastModifiedDateTime": "2020-11-20T17:56:31.39Z",
              "title": "Admins are unable to migrate some user mailboxes from IMAP using the Exchange admin center or PowerShell",
              "id": "EX226574",
              "impactDescription": "Admins attempting to migrate some user mailboxes using the Exchange admin center or PowerShell experienced failures.",
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
                        "content": "Title: Exchange Online service has login issue. We'll provide an update within 30 minutes."
                    }
                  }
                ]
          }
        ]
    }
  ]
}
```
