---
title: Get windows10SecureAssessmentConfiguration
description: Чтение свойств и связей объекта windows10SecureAssessmentConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c8031d41a8573ec637e0f04655369fb098728ca7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127454"
---
# <a name="get-windows10secureassessmentconfiguration"></a><span data-ttu-id="93d21-103">Get windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="93d21-103">Get windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="93d21-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93d21-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93d21-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93d21-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93d21-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93d21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93d21-107">Чтение свойств и связей объекта [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="93d21-107">Read properties and relationships of the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93d21-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="93d21-108">Prerequisites</span></span>
<span data-ttu-id="93d21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93d21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93d21-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93d21-111">Permission type</span></span>|<span data-ttu-id="93d21-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93d21-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93d21-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93d21-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93d21-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93d21-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="93d21-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93d21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93d21-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93d21-116">Not supported.</span></span>|
|<span data-ttu-id="93d21-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="93d21-117">Application</span></span>|<span data-ttu-id="93d21-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93d21-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93d21-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93d21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="93d21-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="93d21-120">Optional query parameters</span></span>
<span data-ttu-id="93d21-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="93d21-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93d21-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93d21-122">Request headers</span></span>
|<span data-ttu-id="93d21-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93d21-123">Header</span></span>|<span data-ttu-id="93d21-124">Значение</span><span class="sxs-lookup"><span data-stu-id="93d21-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93d21-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="93d21-125">Authorization</span></span>|<span data-ttu-id="93d21-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93d21-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93d21-127">Accept</span><span class="sxs-lookup"><span data-stu-id="93d21-127">Accept</span></span>|<span data-ttu-id="93d21-128">application/json</span><span class="sxs-lookup"><span data-stu-id="93d21-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93d21-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93d21-129">Request body</span></span>
<span data-ttu-id="93d21-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93d21-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93d21-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="93d21-131">Response</span></span>
<span data-ttu-id="93d21-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="93d21-132">If successful, this method returns a `200 OK` response code and [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93d21-133">Пример</span><span class="sxs-lookup"><span data-stu-id="93d21-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="93d21-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="93d21-134">Request</span></span>
<span data-ttu-id="93d21-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93d21-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="93d21-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="93d21-136">Response</span></span>
<span data-ttu-id="93d21-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93d21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1674

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
    "id": "f60d71be-71be-f60d-be71-0df6be710df6",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "deviceManagementApplicabilityRuleOsEdition": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
      "osEditionTypes": [
        "windows10EnterpriseN"
      ],
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleOsVersion": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
      "minOSVersion": "Min OSVersion value",
      "maxOSVersion": "Max OSVersion value",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleDeviceMode": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
      "deviceMode": "sModeConfiguration",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "launchUri": "Launch Uri value",
    "configurationAccount": "Configuration Account value",
    "configurationAccountType": "domainAccount",
    "allowPrinting": true,
    "allowScreenCapture": true,
    "allowTextSuggestion": true,
    "localGuestAccountName": "Local Guest Account Name value",
    "assessmentAppUserModelId": "Assessment App User Model Id value"
  }
}
```




