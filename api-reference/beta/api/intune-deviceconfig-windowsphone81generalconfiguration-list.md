---
title: Перечисление объектов windowsPhone81GeneralConfiguration
description: Список свойств и связей объектов windowsPhone81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6f8fcc5e97531712728c4393d7f3f58391dfa28c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154842"
---
# <a name="list-windowsphone81generalconfigurations"></a><span data-ttu-id="4c4e5-103">Перечисление объектов windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="4c4e5-103">List windowsPhone81GeneralConfigurations</span></span>

<span data-ttu-id="4c4e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c4e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c4e5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c4e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c4e5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c4e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c4e5-107">Список свойств и связей объектов [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c4e5-107">List properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c4e5-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4c4e5-108">Prerequisites</span></span>
<span data-ttu-id="4c4e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c4e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c4e5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c4e5-111">Permission type</span></span>|<span data-ttu-id="4c4e5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c4e5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c4e5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c4e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c4e5-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c4e5-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c4e5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c4e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c4e5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c4e5-116">Not supported.</span></span>|
|<span data-ttu-id="4c4e5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4c4e5-117">Application</span></span>|<span data-ttu-id="4c4e5-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c4e5-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c4e5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c4e5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4c4e5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4c4e5-120">Request headers</span></span>
|<span data-ttu-id="4c4e5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c4e5-121">Header</span></span>|<span data-ttu-id="4c4e5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4c4e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c4e5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c4e5-123">Authorization</span></span>|<span data-ttu-id="4c4e5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c4e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c4e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4c4e5-125">Accept</span></span>|<span data-ttu-id="4c4e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c4e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c4e5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c4e5-127">Request body</span></span>
<span data-ttu-id="4c4e5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c4e5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c4e5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c4e5-129">Response</span></span>
<span data-ttu-id="4c4e5-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4c4e5-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c4e5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4c4e5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c4e5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c4e5-132">Request</span></span>
<span data-ttu-id="4c4e5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c4e5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="4c4e5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c4e5-134">Response</span></span>
<span data-ttu-id="4c4e5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c4e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2807

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
      "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
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
      "applyOnlyToWindowsPhone81": true,
      "appsBlockCopyPaste": true,
      "bluetoothBlocked": true,
      "cameraBlocked": true,
      "cellularBlockWifiTethering": true,
      "compliantAppsList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "compliantAppListType": "appsInListCompliant",
      "diagnosticDataBlockSubmission": true,
      "emailBlockAddingAccounts": true,
      "locationServicesBlocked": true,
      "microsoftAccountBlocked": true,
      "nfcBlocked": true,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordMinimumCharacterSetCount": 0,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordRequiredType": "alphanumeric",
      "passwordRequired": true,
      "screenCaptureBlocked": true,
      "storageBlockRemovableStorage": true,
      "storageRequireEncryption": true,
      "webBrowserBlocked": true,
      "wifiBlocked": true,
      "wifiBlockAutomaticConnectHotspots": true,
      "wifiBlockHotspotReporting": true,
      "windowsStoreBlocked": true
    }
  ]
}
```




