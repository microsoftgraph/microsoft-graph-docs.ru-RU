---
title: Получение androidWorkProfileGeneralDeviceConfiguration
description: Чтение свойств и связей объекта androidWorkProfileGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7936e34f8d226e5e1495e14f12a73badfc171522
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35950800"
---
# <a name="get-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="bf0d7-103">Получение androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="bf0d7-103">Get androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="bf0d7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf0d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf0d7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf0d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf0d7-106">Чтение свойств и связей объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bf0d7-106">Read properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf0d7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bf0d7-107">Prerequisites</span></span>
<span data-ttu-id="bf0d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf0d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf0d7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf0d7-110">Permission type</span></span>|<span data-ttu-id="bf0d7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf0d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf0d7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf0d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf0d7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf0d7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bf0d7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf0d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf0d7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf0d7-115">Not supported.</span></span>|
|<span data-ttu-id="bf0d7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf0d7-116">Application</span></span>|<span data-ttu-id="bf0d7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf0d7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf0d7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf0d7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bf0d7-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bf0d7-119">Optional query parameters</span></span>
<span data-ttu-id="bf0d7-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bf0d7-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf0d7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf0d7-121">Request headers</span></span>
|<span data-ttu-id="bf0d7-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf0d7-122">Header</span></span>|<span data-ttu-id="bf0d7-123">Значение</span><span class="sxs-lookup"><span data-stu-id="bf0d7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf0d7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf0d7-124">Authorization</span></span>|<span data-ttu-id="bf0d7-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf0d7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf0d7-126">Accept</span><span class="sxs-lookup"><span data-stu-id="bf0d7-126">Accept</span></span>|<span data-ttu-id="bf0d7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bf0d7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf0d7-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bf0d7-128">Request body</span></span>
<span data-ttu-id="bf0d7-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf0d7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf0d7-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf0d7-130">Response</span></span>
<span data-ttu-id="bf0d7-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bf0d7-131">If successful, this method returns a `200 OK` response code and [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf0d7-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bf0d7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf0d7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf0d7-133">Request</span></span>
<span data-ttu-id="bf0d7-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf0d7-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="bf0d7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf0d7-135">Response</span></span>
<span data-ttu-id="bf0d7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf0d7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3142

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
    "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
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
    "passwordBlockFingerprintUnlock": true,
    "passwordBlockTrustAgents": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "passwordRequiredType": "lowSecurityBiometric",
    "workProfileDataSharingType": "preventAny",
    "workProfileBlockNotificationsWhileDeviceLocked": true,
    "workProfileBlockAddingAccounts": true,
    "workProfileBluetoothEnableContactSharing": true,
    "workProfileBlockScreenCapture": true,
    "workProfileBlockCrossProfileCallerId": true,
    "workProfileBlockCamera": true,
    "workProfileBlockCrossProfileContactsSearch": true,
    "workProfileBlockCrossProfileCopyPaste": true,
    "workProfileDefaultAppPermissionPolicy": "prompt",
    "workProfilePasswordBlockFingerprintUnlock": true,
    "workProfilePasswordBlockTrustAgents": true,
    "workProfilePasswordExpirationDays": 1,
    "workProfilePasswordMinimumLength": 0,
    "workProfilePasswordMinNumericCharacters": 7,
    "workProfilePasswordMinNonLetterCharacters": 9,
    "workProfilePasswordMinLetterCharacters": 6,
    "workProfilePasswordMinLowerCaseCharacters": 9,
    "workProfilePasswordMinUpperCaseCharacters": 9,
    "workProfilePasswordMinSymbolCharacters": 6,
    "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
    "workProfilePasswordPreviousPasswordBlockCount": 13,
    "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
    "workProfilePasswordRequiredType": "lowSecurityBiometric",
    "workProfileRequirePassword": true,
    "securityRequireVerifyApps": true,
    "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
    "vpnEnableAlwaysOnLockdownMode": true
  }
}
```





