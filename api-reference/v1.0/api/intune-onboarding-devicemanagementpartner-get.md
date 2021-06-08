---
title: Получение deviceManagementPartner
description: Чтение свойств и связей объекта deviceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b261567a1edeb26310ef696ab0f0a7e24a8b6d4a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758019"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="4d568-103">Получение deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="4d568-103">Get deviceManagementPartner</span></span>

<span data-ttu-id="4d568-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d568-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d568-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d568-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d568-106">Чтение свойств и связей объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="4d568-106">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d568-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4d568-107">Prerequisites</span></span>
<span data-ttu-id="4d568-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d568-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d568-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d568-110">Permission type</span></span>|<span data-ttu-id="4d568-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d568-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d568-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d568-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d568-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d568-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4d568-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d568-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d568-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d568-115">Not supported.</span></span>|
|<span data-ttu-id="4d568-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4d568-116">Application</span></span>|<span data-ttu-id="4d568-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d568-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d568-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d568-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4d568-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4d568-119">Optional query parameters</span></span>
<span data-ttu-id="4d568-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4d568-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d568-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d568-121">Request headers</span></span>
|<span data-ttu-id="4d568-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d568-122">Header</span></span>|<span data-ttu-id="4d568-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4d568-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d568-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d568-124">Authorization</span></span>|<span data-ttu-id="4d568-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d568-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d568-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4d568-126">Accept</span></span>|<span data-ttu-id="4d568-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4d568-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d568-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d568-128">Request body</span></span>
<span data-ttu-id="4d568-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4d568-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d568-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d568-130">Response</span></span>
<span data-ttu-id="4d568-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4d568-131">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d568-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4d568-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d568-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d568-133">Request</span></span>
<span data-ttu-id="4d568-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d568-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="4d568-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d568-135">Response</span></span>
<span data-ttu-id="4d568-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d568-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




