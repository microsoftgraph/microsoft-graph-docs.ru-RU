---
title: Список Девицеконфигуратионграупассигнментс
description: Список свойств и связей объектов deviceConfigurationGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 420945e2e92465c13ffec7f35a69a078ed7bdb06
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433324"
---
# <a name="list-deviceconfigurationgroupassignments"></a><span data-ttu-id="75cd8-103">Список Девицеконфигуратионграупассигнментс</span><span class="sxs-lookup"><span data-stu-id="75cd8-103">List deviceConfigurationGroupAssignments</span></span>

<span data-ttu-id="75cd8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75cd8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75cd8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75cd8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75cd8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75cd8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75cd8-107">Список свойств и связей объектов [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="75cd8-107">List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75cd8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="75cd8-108">Prerequisites</span></span>
<span data-ttu-id="75cd8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75cd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75cd8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75cd8-111">Permission type</span></span>|<span data-ttu-id="75cd8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75cd8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75cd8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75cd8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75cd8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="75cd8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="75cd8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75cd8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75cd8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75cd8-116">Not supported.</span></span>|
|<span data-ttu-id="75cd8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="75cd8-117">Application</span></span>|<span data-ttu-id="75cd8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="75cd8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75cd8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75cd8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="75cd8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="75cd8-120">Request headers</span></span>
|<span data-ttu-id="75cd8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75cd8-121">Header</span></span>|<span data-ttu-id="75cd8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="75cd8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75cd8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="75cd8-123">Authorization</span></span>|<span data-ttu-id="75cd8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75cd8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75cd8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="75cd8-125">Accept</span></span>|<span data-ttu-id="75cd8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75cd8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75cd8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75cd8-127">Request body</span></span>
<span data-ttu-id="75cd8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75cd8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75cd8-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="75cd8-129">Response</span></span>
<span data-ttu-id="75cd8-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75cd8-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75cd8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="75cd8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="75cd8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="75cd8-132">Request</span></span>
<span data-ttu-id="75cd8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75cd8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="75cd8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="75cd8-134">Response</span></span>
<span data-ttu-id="75cd8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75cd8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 244

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
      "targetGroupId": "Target Group Id value",
      "excludeGroup": true
    }
  ]
}
```



