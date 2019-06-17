---
title: Перечисление объектов windowsDefenderAdvancedThreatProtectionConfiguration
description: Список свойств и связей объектов windowsDefenderAdvancedThreatProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 653729fb13a4bb4f101b69fde8e37e58de5a7480
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977634"
---
# <a name="list-windowsdefenderadvancedthreatprotectionconfigurations"></a><span data-ttu-id="b1c51-103">Перечисление объектов windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="b1c51-103">List windowsDefenderAdvancedThreatProtectionConfigurations</span></span>

> <span data-ttu-id="b1c51-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1c51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1c51-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1c51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1c51-106">Список свойств и связей объектов [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b1c51-106">List properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1c51-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b1c51-107">Prerequisites</span></span>
<span data-ttu-id="b1c51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1c51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1c51-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1c51-110">Permission type</span></span>|<span data-ttu-id="b1c51-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1c51-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1c51-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1c51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1c51-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1c51-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b1c51-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1c51-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1c51-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1c51-115">Not supported.</span></span>|
|<span data-ttu-id="b1c51-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1c51-116">Application</span></span>|<span data-ttu-id="b1c51-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1c51-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1c51-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1c51-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b1c51-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1c51-119">Request headers</span></span>
|<span data-ttu-id="b1c51-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1c51-120">Header</span></span>|<span data-ttu-id="b1c51-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b1c51-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1c51-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1c51-122">Authorization</span></span>|<span data-ttu-id="b1c51-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1c51-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1c51-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b1c51-124">Accept</span></span>|<span data-ttu-id="b1c51-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b1c51-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1c51-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b1c51-126">Request body</span></span>
<span data-ttu-id="b1c51-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1c51-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1c51-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1c51-128">Response</span></span>
<span data-ttu-id="b1c51-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1c51-129">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1c51-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b1c51-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1c51-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1c51-131">Request</span></span>
<span data-ttu-id="b1c51-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1c51-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b1c51-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1c51-133">Response</span></span>
<span data-ttu-id="b1c51-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1c51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





