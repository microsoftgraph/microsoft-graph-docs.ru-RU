---
title: Перечисление объектов windows10TeamGeneralConfiguration
description: Перечисление свойств и связей объектов windows10TeamGeneralConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1eb2d7e72f1ac5aeedfc99c8bc0cb7ac4f2f9c0
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37182157"
---
# <a name="list-windows10teamgeneralconfigurations"></a><span data-ttu-id="20449-103">Перечисление объектов windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="20449-103">List windows10TeamGeneralConfigurations</span></span>

> <span data-ttu-id="20449-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20449-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20449-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20449-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20449-106">Перечисление свойств и связей объектов [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20449-106">List properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20449-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="20449-107">Prerequisites</span></span>
<span data-ttu-id="20449-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20449-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20449-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20449-110">Permission type</span></span>|<span data-ttu-id="20449-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20449-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20449-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20449-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20449-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="20449-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="20449-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20449-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20449-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20449-115">Not supported.</span></span>|
|<span data-ttu-id="20449-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20449-116">Application</span></span>|<span data-ttu-id="20449-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="20449-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20449-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20449-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="20449-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20449-119">Request headers</span></span>
|<span data-ttu-id="20449-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20449-120">Header</span></span>|<span data-ttu-id="20449-121">Значение</span><span class="sxs-lookup"><span data-stu-id="20449-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20449-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20449-122">Authorization</span></span>|<span data-ttu-id="20449-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20449-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20449-124">Accept</span><span class="sxs-lookup"><span data-stu-id="20449-124">Accept</span></span>|<span data-ttu-id="20449-125">application/json</span><span class="sxs-lookup"><span data-stu-id="20449-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20449-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="20449-126">Request body</span></span>
<span data-ttu-id="20449-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="20449-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20449-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="20449-128">Response</span></span>
<span data-ttu-id="20449-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="20449-129">If successful, this method returns a `200 OK` response code and a collection of [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20449-130">Пример</span><span class="sxs-lookup"><span data-stu-id="20449-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="20449-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="20449-131">Request</span></span>
<span data-ttu-id="20449-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20449-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="20449-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="20449-133">Response</span></span>
<span data-ttu-id="20449-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20449-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2428

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
      "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
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
      "azureOperationalInsightsBlockTelemetry": true,
      "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
      "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
      "connectAppBlockAutoLaunch": true,
      "maintenanceWindowBlocked": true,
      "maintenanceWindowDurationInHours": 0,
      "maintenanceWindowStartTime": "11:59:09.3130000",
      "miracastChannel": "one",
      "miracastBlocked": true,
      "miracastRequirePin": true,
      "settingsBlockMyMeetingsAndFiles": true,
      "settingsBlockSessionResume": true,
      "settingsBlockSigninSuggestions": true,
      "settingsDefaultVolume": 5,
      "settingsScreenTimeoutInMinutes": 14,
      "settingsSessionTimeoutInMinutes": 15,
      "settingsSleepTimeoutInMinutes": 13,
      "welcomeScreenBlockAutomaticWakeUp": true,
      "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
      "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
    }
  ]
}
```




