---
title: Получение объекта mobileThreatDefenseConnector
description: Чтение свойств и связей объекта mobileThreatDefenseConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d44272feadfee2c3aea06d9d75d601c3f2f54a4d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145336"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="98324-103">Получение объекта mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="98324-103">Get mobileThreatDefenseConnector</span></span>

<span data-ttu-id="98324-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98324-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98324-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98324-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98324-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98324-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98324-107">Чтение свойств и связей объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="98324-107">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98324-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="98324-108">Prerequisites</span></span>
<span data-ttu-id="98324-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98324-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98324-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98324-111">Permission type</span></span>|<span data-ttu-id="98324-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98324-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98324-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98324-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98324-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98324-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="98324-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98324-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98324-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98324-116">Not supported.</span></span>|
|<span data-ttu-id="98324-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="98324-117">Application</span></span>|<span data-ttu-id="98324-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98324-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98324-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98324-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="98324-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="98324-120">Optional query parameters</span></span>
<span data-ttu-id="98324-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="98324-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98324-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98324-122">Request headers</span></span>
|<span data-ttu-id="98324-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98324-123">Header</span></span>|<span data-ttu-id="98324-124">Значение</span><span class="sxs-lookup"><span data-stu-id="98324-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98324-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="98324-125">Authorization</span></span>|<span data-ttu-id="98324-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98324-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98324-127">Accept</span><span class="sxs-lookup"><span data-stu-id="98324-127">Accept</span></span>|<span data-ttu-id="98324-128">application/json</span><span class="sxs-lookup"><span data-stu-id="98324-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98324-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98324-129">Request body</span></span>
<span data-ttu-id="98324-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98324-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98324-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="98324-131">Response</span></span>
<span data-ttu-id="98324-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="98324-132">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98324-133">Пример</span><span class="sxs-lookup"><span data-stu-id="98324-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="98324-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="98324-134">Request</span></span>
<span data-ttu-id="98324-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98324-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="98324-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="98324-136">Response</span></span>
<span data-ttu-id="98324-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98324-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 828

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
    "id": "e4bede14-de14-e4be-14de-bee414debee4",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "available",
    "androidMobileApplicationManagementEnabled": true,
    "iosMobileApplicationManagementEnabled": true,
    "androidEnabled": true,
    "iosEnabled": true,
    "windowsEnabled": true,
    "macEnabled": true,
    "androidDeviceBlockedOnMissingPartnerData": true,
    "iosDeviceBlockedOnMissingPartnerData": true,
    "windowsDeviceBlockedOnMissingPartnerData": true,
    "macDeviceBlockedOnMissingPartnerData": true,
    "partnerUnsupportedOsVersionBlocked": true,
    "partnerUnresponsivenessThresholdInDays": 6,
    "allowPartnerToCollectIOSApplicationMetadata": true
  }
}
```




