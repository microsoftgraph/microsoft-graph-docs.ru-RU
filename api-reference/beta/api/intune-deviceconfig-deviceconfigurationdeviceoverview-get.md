---
title: Get deviceConfigurationDeviceOverview
description: Чтение свойств и связей объекта deviceConfigurationDeviceOverview.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f2c6923edb955e82407bac1776bca29807e442b8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410198"
---
# <a name="get-deviceconfigurationdeviceoverview"></a><span data-ttu-id="219d7-103">Get deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="219d7-103">Get deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="219d7-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="219d7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="219d7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="219d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="219d7-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="219d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="219d7-107">Чтение свойств и связей объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="219d7-107">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="219d7-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="219d7-108">Prerequisites</span></span>
<span data-ttu-id="219d7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="219d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="219d7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="219d7-111">Permission type</span></span>|<span data-ttu-id="219d7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="219d7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="219d7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="219d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="219d7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="219d7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="219d7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="219d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="219d7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="219d7-116">Not supported.</span></span>|
|<span data-ttu-id="219d7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="219d7-117">Application</span></span>|<span data-ttu-id="219d7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="219d7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="219d7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="219d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="219d7-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="219d7-120">Optional query parameters</span></span>
<span data-ttu-id="219d7-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="219d7-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="219d7-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="219d7-122">Request headers</span></span>
|<span data-ttu-id="219d7-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="219d7-123">Header</span></span>|<span data-ttu-id="219d7-124">Значение</span><span class="sxs-lookup"><span data-stu-id="219d7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="219d7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="219d7-125">Authorization</span></span>|<span data-ttu-id="219d7-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="219d7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="219d7-127">Accept</span><span class="sxs-lookup"><span data-stu-id="219d7-127">Accept</span></span>|<span data-ttu-id="219d7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="219d7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="219d7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="219d7-129">Request body</span></span>
<span data-ttu-id="219d7-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="219d7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="219d7-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="219d7-131">Response</span></span>
<span data-ttu-id="219d7-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="219d7-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="219d7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="219d7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="219d7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="219d7-134">Request</span></span>
<span data-ttu-id="219d7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="219d7-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="219d7-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="219d7-136">Response</span></span>
<span data-ttu-id="219d7-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="219d7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 435

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
    "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```




