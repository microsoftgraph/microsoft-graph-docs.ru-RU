---
title: Get windows10EndpointProtectionConfiguration
description: Чтение свойств и связей объекта windows10EndpointProtectionConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 02154edb6b16e76e9908d8a31ffe94fc96fd581d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412704"
---
# <a name="get-windows10endpointprotectionconfiguration"></a><span data-ttu-id="56420-103">Get windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="56420-103">Get windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="56420-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="56420-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="56420-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56420-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56420-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="56420-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56420-107">Чтение свойств и связей объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="56420-107">Read properties and relationships of the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56420-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="56420-108">Prerequisites</span></span>
<span data-ttu-id="56420-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="56420-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="56420-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56420-111">Permission type</span></span>|<span data-ttu-id="56420-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="56420-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56420-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56420-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56420-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="56420-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="56420-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56420-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56420-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56420-116">Not supported.</span></span>|
|<span data-ttu-id="56420-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56420-117">Application</span></span>|<span data-ttu-id="56420-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56420-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56420-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56420-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56420-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="56420-120">Optional query parameters</span></span>
<span data-ttu-id="56420-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="56420-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56420-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56420-122">Request headers</span></span>
|<span data-ttu-id="56420-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="56420-123">Header</span></span>|<span data-ttu-id="56420-124">Значение</span><span class="sxs-lookup"><span data-stu-id="56420-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56420-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="56420-125">Authorization</span></span>|<span data-ttu-id="56420-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="56420-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56420-127">Accept</span><span class="sxs-lookup"><span data-stu-id="56420-127">Accept</span></span>|<span data-ttu-id="56420-128">application/json</span><span class="sxs-lookup"><span data-stu-id="56420-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56420-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56420-129">Request body</span></span>
<span data-ttu-id="56420-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56420-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56420-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="56420-131">Response</span></span>
<span data-ttu-id="56420-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="56420-132">If successful, this method returns a `200 OK` response code and [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56420-133">Пример</span><span class="sxs-lookup"><span data-stu-id="56420-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="56420-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="56420-134">Request</span></span>
<span data-ttu-id="56420-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56420-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="56420-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="56420-136">Response</span></span>
<span data-ttu-id="56420-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="56420-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 27910

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
    "id": "09709403-9403-0970-0394-700903947009",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "dmaGuardDeviceEnumerationPolicy": "blockAll",
    "userRightsAccessCredentialManagerAsTrustedCaller": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsAllowAccessFromNetwork": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsBlockAccessFromNetwork": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsActAsPartOfTheOperatingSystem": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsLocalLogOn": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsBackupData": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsChangeSystemTime": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsCreateGlobalObjects": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsCreatePageFile": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsCreatePermanentSharedObjects": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsCreateSymbolicLinks": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsCreateToken": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsDebugPrograms": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsRemoteDesktopServicesLogOn": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsDelegation": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsGenerateSecurityAudits": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsImpersonateClient": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsIncreaseSchedulingPriority": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsLoadUnloadDrivers": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsLockMemory": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsManageAuditingAndSecurityLogs": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsManageVolumes": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsModifyFirmwareEnvironment": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsModifyObjectLabels": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsProfileSingleProcess": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsRemoteShutdown": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsRestoreData": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsTakeOwnership": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "userRightsRegisterProcessAsService": {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
      "state": "blocked",
      "localUsersOrGroups": [
        {
          "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
          "name": "Name value",
          "description": "Description value",
          "securityIdentifier": "Security Identifier value"
        }
      ]
    },
    "xboxServicesEnableXboxGameSaveTask": true,
    "xboxServicesAccessoryManagementServiceStartupMode": "automatic",
    "xboxServicesLiveAuthManagerServiceStartupMode": "automatic",
    "xboxServicesLiveGameSaveServiceStartupMode": "automatic",
    "xboxServicesLiveNetworkingServiceStartupMode": "automatic",
    "localSecurityOptionsBlockMicrosoftAccounts": true,
    "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
    "localSecurityOptionsDisableAdministratorAccount": true,
    "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
    "localSecurityOptionsDisableGuestAccount": true,
    "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
    "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
    "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
    "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
    "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "administrators",
    "localSecurityOptionsMachineInactivityLimit": 10,
    "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
    "localSecurityOptionsDoNotRequireCtrlAltDel": true,
    "localSecurityOptionsHideLastSignedInUser": true,
    "localSecurityOptionsHideUsernameAtSignIn": true,
    "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
    "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
    "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
    "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
    "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
    "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "requireNtmlV2SessionSecurity",
    "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "requireNtmlV2SessionSecurity",
    "lanManagerAuthenticationLevel": "lmNtlmAndNtlmV2",
    "lanManagerWorkstationDisableInsecureGuestLogons": true,
    "localSecurityOptionsClearVirtualMemoryPageFile": true,
    "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
    "localSecurityOptionsAllowUIAccessApplicationElevation": true,
    "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
    "localSecurityOptionsOnlyElevateSignedExecutables": true,
    "localSecurityOptionsAdministratorElevationPromptBehavior": "elevateWithoutPrompting",
    "localSecurityOptionsStandardUserElevationPromptBehavior": "automaticallyDenyElevationRequests",
    "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
    "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
    "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
    "localSecurityOptionsUseAdminApprovalMode": true,
    "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
    "localSecurityOptionsInformationShownOnLockScreen": "userDisplayNameDomainUser",
    "localSecurityOptionsInformationDisplayedOnLockScreen": "administrators",
    "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
    "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
    "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
    "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
    "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
    "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
    "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
    "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
    "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
    "localSecurityOptionsSmartCardRemovalBehavior": "noAction",
    "defenderSecurityCenterDisableAppBrowserUI": true,
    "defenderSecurityCenterDisableFamilyUI": true,
    "defenderSecurityCenterDisableHealthUI": true,
    "defenderSecurityCenterDisableNetworkUI": true,
    "defenderSecurityCenterDisableVirusUI": true,
    "defenderSecurityCenterDisableAccountUI": true,
    "defenderSecurityCenterDisableHardwareUI": true,
    "defenderSecurityCenterDisableRansomwareUI": true,
    "defenderSecurityCenterDisableSecureBootUI": true,
    "defenderSecurityCenterDisableTroubleshootingUI": true,
    "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
    "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
    "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
    "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
    "defenderSecurityCenterNotificationsFromApp": "blockNoncriticalNotifications",
    "defenderSecurityCenterITContactDisplay": "displayInAppAndInNotifications",
    "firewallBlockStatefulFTP": true,
    "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
    "firewallPreSharedKeyEncodingMethod": "none",
    "firewallIPSecExemptionsAllowNeighborDiscovery": true,
    "firewallIPSecExemptionsAllowICMP": true,
    "firewallIPSecExemptionsAllowRouterDiscovery": true,
    "firewallIPSecExemptionsAllowDHCP": true,
    "firewallCertificateRevocationListCheckMethod": "none",
    "firewallMergeKeyingModuleSettings": true,
    "firewallPacketQueueingMethod": "disabled",
    "firewallProfileDomain": {
      "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
      "firewallEnabled": "blocked",
      "stealthModeRequired": true,
      "stealthModeBlocked": true,
      "incomingTrafficRequired": true,
      "incomingTrafficBlocked": true,
      "unicastResponsesToMulticastBroadcastsRequired": true,
      "unicastResponsesToMulticastBroadcastsBlocked": true,
      "inboundNotificationsRequired": true,
      "inboundNotificationsBlocked": true,
      "authorizedApplicationRulesFromGroupPolicyMerged": true,
      "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
      "globalPortRulesFromGroupPolicyMerged": true,
      "globalPortRulesFromGroupPolicyNotMerged": true,
      "connectionSecurityRulesFromGroupPolicyMerged": true,
      "connectionSecurityRulesFromGroupPolicyNotMerged": true,
      "outboundConnectionsRequired": true,
      "outboundConnectionsBlocked": true,
      "inboundConnectionsRequired": true,
      "inboundConnectionsBlocked": true,
      "securedPacketExemptionAllowed": true,
      "securedPacketExemptionBlocked": true,
      "policyRulesFromGroupPolicyMerged": true,
      "policyRulesFromGroupPolicyNotMerged": true
    },
    "firewallProfilePublic": {
      "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
      "firewallEnabled": "blocked",
      "stealthModeRequired": true,
      "stealthModeBlocked": true,
      "incomingTrafficRequired": true,
      "incomingTrafficBlocked": true,
      "unicastResponsesToMulticastBroadcastsRequired": true,
      "unicastResponsesToMulticastBroadcastsBlocked": true,
      "inboundNotificationsRequired": true,
      "inboundNotificationsBlocked": true,
      "authorizedApplicationRulesFromGroupPolicyMerged": true,
      "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
      "globalPortRulesFromGroupPolicyMerged": true,
      "globalPortRulesFromGroupPolicyNotMerged": true,
      "connectionSecurityRulesFromGroupPolicyMerged": true,
      "connectionSecurityRulesFromGroupPolicyNotMerged": true,
      "outboundConnectionsRequired": true,
      "outboundConnectionsBlocked": true,
      "inboundConnectionsRequired": true,
      "inboundConnectionsBlocked": true,
      "securedPacketExemptionAllowed": true,
      "securedPacketExemptionBlocked": true,
      "policyRulesFromGroupPolicyMerged": true,
      "policyRulesFromGroupPolicyNotMerged": true
    },
    "firewallProfilePrivate": {
      "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
      "firewallEnabled": "blocked",
      "stealthModeRequired": true,
      "stealthModeBlocked": true,
      "incomingTrafficRequired": true,
      "incomingTrafficBlocked": true,
      "unicastResponsesToMulticastBroadcastsRequired": true,
      "unicastResponsesToMulticastBroadcastsBlocked": true,
      "inboundNotificationsRequired": true,
      "inboundNotificationsBlocked": true,
      "authorizedApplicationRulesFromGroupPolicyMerged": true,
      "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
      "globalPortRulesFromGroupPolicyMerged": true,
      "globalPortRulesFromGroupPolicyNotMerged": true,
      "connectionSecurityRulesFromGroupPolicyMerged": true,
      "connectionSecurityRulesFromGroupPolicyNotMerged": true,
      "outboundConnectionsRequired": true,
      "outboundConnectionsBlocked": true,
      "inboundConnectionsRequired": true,
      "inboundConnectionsBlocked": true,
      "securedPacketExemptionAllowed": true,
      "securedPacketExemptionBlocked": true,
      "policyRulesFromGroupPolicyMerged": true,
      "policyRulesFromGroupPolicyNotMerged": true
    },
    "defenderAttackSurfaceReductionExcludedPaths": [
      "Defender Attack Surface Reduction Excluded Paths value"
    ],
    "defenderOfficeAppsOtherProcessInjectionType": "block",
    "defenderOfficeAppsOtherProcessInjection": "enable",
    "defenderOfficeAppsExecutableContentCreationOrLaunchType": "block",
    "defenderOfficeAppsExecutableContentCreationOrLaunch": "enable",
    "defenderOfficeAppsLaunchChildProcessType": "block",
    "defenderOfficeAppsLaunchChildProcess": "enable",
    "defenderOfficeMacroCodeAllowWin32ImportsType": "block",
    "defenderOfficeMacroCodeAllowWin32Imports": "enable",
    "defenderScriptObfuscatedMacroCodeType": "block",
    "defenderScriptObfuscatedMacroCode": "enable",
    "defenderScriptDownloadedPayloadExecutionType": "block",
    "defenderScriptDownloadedPayloadExecution": "enable",
    "defenderPreventCredentialStealingType": "enable",
    "defenderProcessCreationType": "block",
    "defenderProcessCreation": "enable",
    "defenderUntrustedUSBProcessType": "block",
    "defenderUntrustedUSBProcess": "enable",
    "defenderUntrustedExecutableType": "block",
    "defenderUntrustedExecutable": "enable",
    "defenderEmailContentExecutionType": "block",
    "defenderEmailContentExecution": "enable",
    "defenderAdvancedRansomewareProtectionType": "enable",
    "defenderGuardMyFoldersType": "enable",
    "defenderGuardedFoldersAllowedAppPaths": [
      "Defender Guarded Folders Allowed App Paths value"
    ],
    "defenderAdditionalGuardedFolders": [
      "Defender Additional Guarded Folders value"
    ],
    "defenderNetworkProtectionType": "enable",
    "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
    "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
    "defenderSecurityCenterBlockExploitProtectionOverride": true,
    "appLockerApplicationControl": "enforceComponentsAndStoreApps",
    "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "enableWithUEFILock",
    "deviceGuardEnableVirtualizationBasedSecurity": true,
    "deviceGuardEnableSecureBootWithDMA": true,
    "deviceGuardLaunchSystemGuard": "enabled",
    "smartScreenEnableInShell": true,
    "smartScreenBlockOverrideForFiles": true,
    "applicationGuardEnabled": true,
    "applicationGuardEnabledOptions": "enabledForEdge",
    "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
    "applicationGuardBlockNonEnterpriseContent": true,
    "applicationGuardAllowPersistence": true,
    "applicationGuardForceAuditing": true,
    "applicationGuardBlockClipboardSharing": "blockBoth",
    "applicationGuardAllowPrintToPDF": true,
    "applicationGuardAllowPrintToXPS": true,
    "applicationGuardAllowPrintToLocalPrinters": true,
    "applicationGuardAllowPrintToNetworkPrinters": true,
    "applicationGuardAllowVirtualGPU": true,
    "applicationGuardAllowFileSaveOnHost": true,
    "bitLockerAllowStandardUserEncryption": true,
    "bitLockerDisableWarningForOtherDiskEncryption": true,
    "bitLockerEnableStorageCardEncryptionOnMobile": true,
    "bitLockerEncryptDevice": true,
    "bitLockerSystemDrivePolicy": {
      "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
      "encryptionMethod": "aesCbc256",
      "startupAuthenticationRequired": true,
      "startupAuthenticationBlockWithoutTpmChip": true,
      "startupAuthenticationTpmUsage": "required",
      "startupAuthenticationTpmPinUsage": "required",
      "startupAuthenticationTpmKeyUsage": "required",
      "startupAuthenticationTpmPinAndKeyUsage": "required",
      "minimumPinLength": 0,
      "recoveryOptions": {
        "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
        "blockDataRecoveryAgent": true,
        "recoveryPasswordUsage": "required",
        "recoveryKeyUsage": "required",
        "hideRecoveryOptions": true,
        "enableRecoveryInformationSaveToStore": true,
        "recoveryInformationToStore": "passwordOnly",
        "enableBitLockerAfterRecoveryInformationToStore": true
      },
      "prebootRecoveryEnableMessageAndUrl": true,
      "prebootRecoveryMessage": "Preboot Recovery Message value",
      "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
    },
    "bitLockerFixedDrivePolicy": {
      "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
      "encryptionMethod": "aesCbc256",
      "requireEncryptionForWriteAccess": true,
      "recoveryOptions": {
        "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
        "blockDataRecoveryAgent": true,
        "recoveryPasswordUsage": "required",
        "recoveryKeyUsage": "required",
        "hideRecoveryOptions": true,
        "enableRecoveryInformationSaveToStore": true,
        "recoveryInformationToStore": "passwordOnly",
        "enableBitLockerAfterRecoveryInformationToStore": true
      }
    },
    "bitLockerRemovableDrivePolicy": {
      "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
      "encryptionMethod": "aesCbc256",
      "requireEncryptionForWriteAccess": true,
      "blockCrossOrganizationWriteAccess": true
    }
  }
}
```




