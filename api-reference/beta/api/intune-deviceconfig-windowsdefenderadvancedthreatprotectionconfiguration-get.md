---
title: Получение объекта windowsDefenderAdvancedThreatProtectionConfiguration
description: Чтение свойств и связей объекта windowsDefenderAdvancedThreatProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 482a45275fa85ee14c76971a9fba9d09312da25f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982321"
---
# <a name="get-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="cba44-103">Получение объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="cba44-103">Get windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="cba44-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cba44-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cba44-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cba44-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cba44-106">Чтение свойств и связей объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cba44-106">Read properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cba44-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cba44-107">Prerequisites</span></span>
<span data-ttu-id="cba44-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cba44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cba44-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cba44-110">Permission type</span></span>|<span data-ttu-id="cba44-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cba44-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cba44-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cba44-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cba44-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cba44-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cba44-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cba44-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cba44-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cba44-115">Not supported.</span></span>|
|<span data-ttu-id="cba44-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cba44-116">Application</span></span>|<span data-ttu-id="cba44-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cba44-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cba44-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cba44-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cba44-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cba44-119">Optional query parameters</span></span>
<span data-ttu-id="cba44-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cba44-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cba44-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cba44-121">Request headers</span></span>
|<span data-ttu-id="cba44-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cba44-122">Header</span></span>|<span data-ttu-id="cba44-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cba44-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cba44-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cba44-124">Authorization</span></span>|<span data-ttu-id="cba44-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cba44-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cba44-126">Accept</span><span class="sxs-lookup"><span data-stu-id="cba44-126">Accept</span></span>|<span data-ttu-id="cba44-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cba44-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cba44-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cba44-128">Request body</span></span>
<span data-ttu-id="cba44-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cba44-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cba44-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="cba44-130">Response</span></span>
<span data-ttu-id="cba44-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cba44-131">If successful, this method returns a `200 OK` response code and [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cba44-132">Пример</span><span class="sxs-lookup"><span data-stu-id="cba44-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cba44-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="cba44-133">Request</span></span>
<span data-ttu-id="cba44-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cba44-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="cba44-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cba44-135">Response</span></span>
<span data-ttu-id="cba44-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cba44-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1872

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
    "id": "294373aa-73aa-2943-aa73-4329aa734329",
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
    "advancedThreatProtectionOnboardingBlob": "Advanced Threat Protection Onboarding Blob value",
    "advancedThreatProtectionOnboardingFilename": "Advanced Threat Protection Onboarding Filename value",
    "advancedThreatProtectionAutoPopulateOnboardingBlob": true,
    "allowSampleSharing": true,
    "enableExpeditedTelemetryReporting": true,
    "advancedThreatProtectionOffboardingBlob": "Advanced Threat Protection Offboarding Blob value",
    "advancedThreatProtectionOffboardingFilename": "Advanced Threat Protection Offboarding Filename value"
  }
}
```





