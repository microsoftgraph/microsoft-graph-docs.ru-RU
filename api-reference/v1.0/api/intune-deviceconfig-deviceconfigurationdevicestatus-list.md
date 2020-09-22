---
title: Перечисление объектов deviceConfigurationDeviceStatus
description: Список свойств и связей объектов deviceConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6c5dfe6ef0c355206151679c82f7231d9579400d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066945"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="2a192-103">Перечисление объектов deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="2a192-103">List deviceConfigurationDeviceStatuses</span></span>

<span data-ttu-id="2a192-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a192-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a192-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a192-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a192-106">Список свойств и связей объектов [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="2a192-106">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a192-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2a192-107">Prerequisites</span></span>
<span data-ttu-id="2a192-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a192-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a192-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a192-110">Permission type</span></span>|<span data-ttu-id="2a192-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a192-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a192-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a192-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a192-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a192-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2a192-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a192-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a192-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a192-115">Not supported.</span></span>|
|<span data-ttu-id="2a192-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a192-116">Application</span></span>|<span data-ttu-id="2a192-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a192-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a192-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a192-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="2a192-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2a192-119">Request headers</span></span>
|<span data-ttu-id="2a192-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a192-120">Header</span></span>|<span data-ttu-id="2a192-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2a192-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a192-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a192-122">Authorization</span></span>|<span data-ttu-id="2a192-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a192-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a192-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2a192-124">Accept</span></span>|<span data-ttu-id="2a192-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a192-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a192-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a192-126">Request body</span></span>
<span data-ttu-id="2a192-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a192-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a192-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a192-128">Response</span></span>
<span data-ttu-id="2a192-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2a192-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a192-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2a192-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a192-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a192-131">Request</span></span>
<span data-ttu-id="2a192-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a192-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="2a192-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a192-133">Response</span></span>
<span data-ttu-id="2a192-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a192-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
      "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```









