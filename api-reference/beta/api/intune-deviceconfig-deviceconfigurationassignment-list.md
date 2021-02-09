---
title: Перечисление объектов deviceConfigurationAssignment
description: Список свойств и связей объектов deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a3f0060686f69b6c9e6196963a90c855a2b7384d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153979"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="f2a19-103">Перечисление объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f2a19-103">List deviceConfigurationAssignments</span></span>

<span data-ttu-id="f2a19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2a19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2a19-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2a19-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2a19-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2a19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2a19-107">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f2a19-107">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2a19-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f2a19-108">Prerequisites</span></span>
<span data-ttu-id="f2a19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2a19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2a19-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2a19-111">Permission type</span></span>|<span data-ttu-id="f2a19-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2a19-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2a19-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2a19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2a19-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2a19-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f2a19-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2a19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2a19-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2a19-116">Not supported.</span></span>|
|<span data-ttu-id="f2a19-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2a19-117">Application</span></span>|<span data-ttu-id="f2a19-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2a19-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2a19-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2a19-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f2a19-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f2a19-120">Request headers</span></span>
|<span data-ttu-id="f2a19-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f2a19-121">Header</span></span>|<span data-ttu-id="f2a19-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f2a19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2a19-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2a19-123">Authorization</span></span>|<span data-ttu-id="f2a19-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2a19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2a19-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f2a19-125">Accept</span></span>|<span data-ttu-id="f2a19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2a19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2a19-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2a19-127">Request body</span></span>
<span data-ttu-id="f2a19-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2a19-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2a19-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2a19-129">Response</span></span>
<span data-ttu-id="f2a19-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f2a19-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2a19-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f2a19-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2a19-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2a19-132">Request</span></span>
<span data-ttu-id="f2a19-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2a19-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="f2a19-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2a19-134">Response</span></span>
<span data-ttu-id="f2a19-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2a19-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 571

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```




