---
title: Get deviceConfigurationAssignment
description: Чтение свойств и связей объекта deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 843921627051961058b6c5788633e5a05fd71da8
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123178"
---
# <a name="get-deviceconfigurationassignment"></a><span data-ttu-id="e2063-103">Get deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e2063-103">Get deviceConfigurationAssignment</span></span>

<span data-ttu-id="e2063-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2063-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2063-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2063-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2063-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2063-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2063-107">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e2063-107">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2063-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e2063-108">Prerequisites</span></span>
<span data-ttu-id="e2063-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e2063-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e2063-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2063-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2063-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2063-111">Permission type</span></span>|<span data-ttu-id="e2063-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2063-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2063-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2063-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2063-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2063-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e2063-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2063-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2063-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2063-116">Not supported.</span></span>|
|<span data-ttu-id="e2063-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2063-117">Application</span></span>|<span data-ttu-id="e2063-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2063-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2063-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2063-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2063-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e2063-120">Optional query parameters</span></span>
<span data-ttu-id="e2063-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e2063-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2063-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2063-122">Request headers</span></span>
|<span data-ttu-id="e2063-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2063-123">Header</span></span>|<span data-ttu-id="e2063-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e2063-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2063-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2063-125">Authorization</span></span>|<span data-ttu-id="e2063-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2063-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2063-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e2063-127">Accept</span></span>|<span data-ttu-id="e2063-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e2063-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2063-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2063-129">Request body</span></span>
<span data-ttu-id="e2063-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2063-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2063-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2063-131">Response</span></span>
<span data-ttu-id="e2063-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e2063-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2063-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e2063-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2063-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2063-134">Request</span></span>
<span data-ttu-id="e2063-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2063-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="e2063-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2063-136">Response</span></span>
<span data-ttu-id="e2063-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="e2063-137">Here is an example of the response.</span></span> <span data-ttu-id="e2063-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e2063-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e2063-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e2063-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "value": {
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
}
```



