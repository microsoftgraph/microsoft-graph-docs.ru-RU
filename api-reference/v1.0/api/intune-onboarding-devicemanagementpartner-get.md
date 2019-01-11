---
title: Получение deviceManagementPartner
description: Чтение свойств и связей объекта deviceManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5696ce5ad5a723ef7940c01353270fce50df2f2e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884233"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="568a9-103">Получение deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="568a9-103">Get deviceManagementPartner</span></span>

> <span data-ttu-id="568a9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="568a9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="568a9-105">Чтение свойств и связей объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="568a9-105">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="568a9-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="568a9-106">Prerequisites</span></span>
<span data-ttu-id="568a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="568a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="568a9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="568a9-109">Permission type</span></span>|<span data-ttu-id="568a9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="568a9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="568a9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="568a9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="568a9-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="568a9-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="568a9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="568a9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="568a9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="568a9-114">Not supported.</span></span>|
|<span data-ttu-id="568a9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="568a9-115">Application</span></span>|<span data-ttu-id="568a9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="568a9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="568a9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="568a9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="568a9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="568a9-118">Optional query parameters</span></span>
<span data-ttu-id="568a9-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="568a9-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="568a9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="568a9-120">Request headers</span></span>
|<span data-ttu-id="568a9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="568a9-121">Header</span></span>|<span data-ttu-id="568a9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="568a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="568a9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="568a9-123">Authorization</span></span>|<span data-ttu-id="568a9-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="568a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="568a9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="568a9-125">Accept</span></span>|<span data-ttu-id="568a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="568a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="568a9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="568a9-127">Request body</span></span>
<span data-ttu-id="568a9-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="568a9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="568a9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="568a9-129">Response</span></span>
<span data-ttu-id="568a9-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="568a9-130">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="568a9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="568a9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="568a9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="568a9-132">Request</span></span>
<span data-ttu-id="568a9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="568a9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="568a9-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="568a9-134">Response</span></span>
<span data-ttu-id="568a9-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="568a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementPartner",
    "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "unavailable",
    "partnerAppType": "singleTenantApp",
    "singleTenantAppId": "Single Tenant App Id value",
    "displayName": "Display Name value",
    "isConfigured": true,
    "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
    "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
  }
}
```



