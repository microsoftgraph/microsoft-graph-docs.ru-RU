---
title: Перечисление объектов windowsDefenderAdvancedThreatProtectionConfiguration
description: Список свойств и связей объектов windowsDefenderAdvancedThreatProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 89c6449f6424dbf847fc5d000188df2bd1bb1f50
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151006"
---
# <a name="list-windowsdefenderadvancedthreatprotectionconfigurations"></a><span data-ttu-id="ff6af-103">Перечисление объектов windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff6af-103">List windowsDefenderAdvancedThreatProtectionConfigurations</span></span>

<span data-ttu-id="ff6af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff6af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff6af-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff6af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff6af-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff6af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff6af-107">Список свойств и связей объектов [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ff6af-107">List properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff6af-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ff6af-108">Prerequisites</span></span>
<span data-ttu-id="ff6af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff6af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff6af-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff6af-111">Permission type</span></span>|<span data-ttu-id="ff6af-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff6af-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff6af-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff6af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff6af-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff6af-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ff6af-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff6af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff6af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff6af-116">Not supported.</span></span>|
|<span data-ttu-id="ff6af-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ff6af-117">Application</span></span>|<span data-ttu-id="ff6af-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff6af-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff6af-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff6af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ff6af-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ff6af-120">Request headers</span></span>
|<span data-ttu-id="ff6af-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff6af-121">Header</span></span>|<span data-ttu-id="ff6af-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ff6af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff6af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff6af-123">Authorization</span></span>|<span data-ttu-id="ff6af-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff6af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff6af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ff6af-125">Accept</span></span>|<span data-ttu-id="ff6af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff6af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff6af-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff6af-127">Request body</span></span>
<span data-ttu-id="ff6af-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff6af-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff6af-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff6af-129">Response</span></span>
<span data-ttu-id="ff6af-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ff6af-130">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff6af-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ff6af-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff6af-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff6af-132">Request</span></span>
<span data-ttu-id="ff6af-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff6af-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ff6af-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff6af-134">Response</span></span>
<span data-ttu-id="ff6af-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff6af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1964

{
  "value": [
    {
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
  ]
}
```




