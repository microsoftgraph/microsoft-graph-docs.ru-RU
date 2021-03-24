---
title: Get deviceConfigurationGroupAssignment
description: Чтение свойств и связей объекта deviceConfigurationGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e7ce74a4dc2f4757888d4b6624083752e6d3a41
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131584"
---
# <a name="get-deviceconfigurationgroupassignment"></a><span data-ttu-id="cf14a-103">Get deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="cf14a-103">Get deviceConfigurationGroupAssignment</span></span>

<span data-ttu-id="cf14a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf14a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf14a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf14a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf14a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf14a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf14a-107">Чтение свойств и связей [объекта deviceConfigurationGroupAssignment.](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cf14a-107">Read properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf14a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cf14a-108">Prerequisites</span></span>
<span data-ttu-id="cf14a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf14a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf14a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf14a-111">Permission type</span></span>|<span data-ttu-id="cf14a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf14a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf14a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf14a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf14a-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf14a-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf14a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf14a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf14a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf14a-116">Not supported.</span></span>|
|<span data-ttu-id="cf14a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cf14a-117">Application</span></span>|<span data-ttu-id="cf14a-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf14a-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf14a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf14a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf14a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cf14a-120">Optional query parameters</span></span>
<span data-ttu-id="cf14a-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cf14a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf14a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf14a-122">Request headers</span></span>
|<span data-ttu-id="cf14a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf14a-123">Header</span></span>|<span data-ttu-id="cf14a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="cf14a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf14a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf14a-125">Authorization</span></span>|<span data-ttu-id="cf14a-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf14a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf14a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="cf14a-127">Accept</span></span>|<span data-ttu-id="cf14a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cf14a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf14a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf14a-129">Request body</span></span>
<span data-ttu-id="cf14a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf14a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf14a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf14a-131">Response</span></span>
<span data-ttu-id="cf14a-132">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cf14a-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf14a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="cf14a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf14a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf14a-134">Request</span></span>
<span data-ttu-id="cf14a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf14a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="cf14a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf14a-136">Response</span></span>
<span data-ttu-id="cf14a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf14a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 222

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
    "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
    "targetGroupId": "Target Group Id value",
    "excludeGroup": true
  }
}
```




