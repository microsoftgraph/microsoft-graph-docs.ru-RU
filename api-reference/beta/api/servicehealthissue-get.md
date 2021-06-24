---
title: Get serviceHealthIssue
description: Извлечение свойств и связей объекта serviceHealthIssue.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: a848773e047ed36cdd8aecd082aabffec7f1311b
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107859"
---
# <a name="get-servicehealthissue"></a><span data-ttu-id="a3a64-103">Get serviceHealthIssue</span><span class="sxs-lookup"><span data-stu-id="a3a64-103">Get serviceHealthIssue</span></span>
<span data-ttu-id="a3a64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3a64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3a64-105">Извлечение свойств и связей объекта [serviceHealthIssue.](../resources/servicehealthissue.md)</span><span class="sxs-lookup"><span data-stu-id="a3a64-105">Retrieve the properties and relationships of a [serviceHealthIssue](../resources/servicehealthissue.md) object.</span></span>

<span data-ttu-id="a3a64-106">Эта операция извлекает указанную проблему со здоровьем службы для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3a64-106">This operation retrieves a specified service health issue for tenant.</span></span> <span data-ttu-id="a3a64-107">Операция возвращает ошибку, если проблема не существует для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3a64-107">The operation returns an error if the issue does not exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3a64-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3a64-108">Permissions</span></span>
<span data-ttu-id="a3a64-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3a64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3a64-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3a64-111">Permission type</span></span>|<span data-ttu-id="a3a64-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3a64-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3a64-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3a64-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3a64-114">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3a64-114">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="a3a64-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3a64-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3a64-116">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3a64-116">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="a3a64-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a3a64-117">Application</span></span>|<span data-ttu-id="a3a64-118">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3a64-118">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3a64-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3a64-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/issues/{serviceHealthIssueId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3a64-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a3a64-120">Optional query parameters</span></span>
<span data-ttu-id="a3a64-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a3a64-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3a64-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3a64-122">Request headers</span></span>
|<span data-ttu-id="a3a64-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a3a64-123">Name</span></span>|<span data-ttu-id="a3a64-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a3a64-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a3a64-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3a64-125">Authorization</span></span>|<span data-ttu-id="a3a64-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3a64-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3a64-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3a64-128">Request body</span></span>
<span data-ttu-id="a3a64-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3a64-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3a64-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3a64-130">Response</span></span>

<span data-ttu-id="a3a64-131">В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [serviceHealthIssue](../resources/servicehealthissue.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a3a64-131">If successful, this method returns a `200 OK` response code and a [serviceHealthIssue](../resources/servicehealthissue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3a64-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a3a64-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3a64-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3a64-133">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["MO226784"],
  "name": "get_servicehealthissue"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/issues/MO226784
```


### <a name="response"></a><span data-ttu-id="a3a64-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3a64-134">Response</span></span>
><span data-ttu-id="a3a64-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a3a64-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealthIssue"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/issues/$entity",
  "startDateTime": "2020-11-14T08:15:00Z",
  "endDateTime": "2020-11-14T09:45:00Z",
  "lastModifiedDateTime": "2020-11-14T11:06:53.353Z",
  "title": "Intermittently unable to access some Microsoft 365 services",
  "id": "MO226784",
  "impactDescription": "Users may have been intermittently unable to access some Microsoft 365 services.",
  "classification": "Advisory",
  "origin": "Microsoft",
  "status": "ServiceRestored",
  "service": "Microsoft 365 suite",
  "feature": "Access",
  "featureGroup": "Portal",
  "isResolved": true,
  "details": [],
  "posts": [
    {
      "createdDateTime": "2020-11-12T07:07:38.97Z",
      "postType": "Regular",
      "description": {
        "contentType": "Text",
        "content": "Title: Intermittently unable to invite partners to meetings using some Microsoft 365 services\n\nUser Impact: Users may have been intermittently unable to invite partners to meetings using some Microsoft 365 services."
      }
    }
  ]
}
```

