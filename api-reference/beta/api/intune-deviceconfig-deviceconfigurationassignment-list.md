---
title: Перечисление объектов deviceConfigurationAssignment
description: Список свойств и связей объектов deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 264a453491fb75c52777d9e8ba5a40cfba96505f
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123150"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="653c0-103">Перечисление объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="653c0-103">List deviceConfigurationAssignments</span></span>

<span data-ttu-id="653c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="653c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="653c0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="653c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="653c0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="653c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="653c0-107">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="653c0-107">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="653c0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="653c0-108">Prerequisites</span></span>
<span data-ttu-id="653c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="653c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="653c0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="653c0-111">Permission type</span></span>|<span data-ttu-id="653c0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="653c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="653c0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="653c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="653c0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="653c0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="653c0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="653c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="653c0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="653c0-116">Not supported.</span></span>|
|<span data-ttu-id="653c0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="653c0-117">Application</span></span>|<span data-ttu-id="653c0-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="653c0-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="653c0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="653c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="653c0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="653c0-120">Request headers</span></span>
|<span data-ttu-id="653c0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="653c0-121">Header</span></span>|<span data-ttu-id="653c0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="653c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="653c0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="653c0-123">Authorization</span></span>|<span data-ttu-id="653c0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="653c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="653c0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="653c0-125">Accept</span></span>|<span data-ttu-id="653c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="653c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="653c0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="653c0-127">Request body</span></span>
<span data-ttu-id="653c0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="653c0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="653c0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="653c0-129">Response</span></span>
<span data-ttu-id="653c0-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="653c0-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="653c0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="653c0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="653c0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="653c0-132">Request</span></span>
<span data-ttu-id="653c0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="653c0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="653c0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="653c0-134">Response</span></span>
<span data-ttu-id="653c0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="653c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 503

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```



