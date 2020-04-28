---
title: Получение iosEasEmailProfileConfiguration
description: Чтение свойств и связей объекта iosEasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eae8cae1f1b0d20a7d8b4372f6d4b6357a81a172
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432698"
---
# <a name="get-ioseasemailprofileconfiguration"></a><span data-ttu-id="68009-103">Получение iosEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="68009-103">Get iosEasEmailProfileConfiguration</span></span>

<span data-ttu-id="68009-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68009-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68009-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68009-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68009-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68009-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68009-107">Чтение свойств и связей объекта [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="68009-107">Read properties and relationships of the [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68009-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="68009-108">Prerequisites</span></span>
<span data-ttu-id="68009-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68009-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68009-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68009-111">Permission type</span></span>|<span data-ttu-id="68009-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68009-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68009-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68009-113">Delegated (work or school account)</span></span>|<span data-ttu-id="68009-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="68009-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="68009-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68009-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68009-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68009-116">Not supported.</span></span>|
|<span data-ttu-id="68009-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68009-117">Application</span></span>|<span data-ttu-id="68009-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="68009-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68009-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68009-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68009-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="68009-120">Optional query parameters</span></span>
<span data-ttu-id="68009-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="68009-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68009-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68009-122">Request headers</span></span>
|<span data-ttu-id="68009-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68009-123">Header</span></span>|<span data-ttu-id="68009-124">Значение</span><span class="sxs-lookup"><span data-stu-id="68009-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68009-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68009-125">Authorization</span></span>|<span data-ttu-id="68009-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68009-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68009-127">Accept</span><span class="sxs-lookup"><span data-stu-id="68009-127">Accept</span></span>|<span data-ttu-id="68009-128">application/json</span><span class="sxs-lookup"><span data-stu-id="68009-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68009-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="68009-129">Request body</span></span>
<span data-ttu-id="68009-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68009-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68009-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="68009-131">Response</span></span>
<span data-ttu-id="68009-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68009-132">If successful, this method returns a `200 OK` response code and [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68009-133">Пример</span><span class="sxs-lookup"><span data-stu-id="68009-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="68009-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="68009-134">Request</span></span>
<span data-ttu-id="68009-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68009-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="68009-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="68009-136">Response</span></span>
<span data-ttu-id="68009-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68009-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2438

{
  "value": {
    "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
    "id": "e03086da-86da-e030-da86-30e0da8630e0",
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
    "usernameSource": "primarySmtpAddress",
    "usernameAADSource": "primarySmtpAddress",
    "userDomainNameSource": "netBiosDomainName",
    "customDomainName": "Custom Domain Name value",
    "accountName": "Account Name value",
    "authenticationMethod": "certificate",
    "blockMovingMessagesToOtherEmailAccounts": true,
    "blockSendingEmailFromThirdPartyApps": true,
    "blockSyncingRecentlyUsedEmailAddresses": true,
    "durationOfEmailToSync": "oneDay",
    "emailAddressSource": "primarySmtpAddress",
    "easServices": "calendars",
    "easServicesUserOverrideEnabled": true,
    "hostName": "Host Name value",
    "requireSmime": true,
    "smimeEnablePerMessageSwitch": true,
    "smimeEncryptByDefaultEnabled": true,
    "smimeSigningEnabled": true,
    "smimeSigningUserOverrideEnabled": true,
    "smimeEncryptByDefaultUserOverrideEnabled": true,
    "smimeSigningCertificateUserOverrideEnabled": true,
    "smimeEncryptionCertificateUserOverrideEnabled": true,
    "requireSsl": true,
    "useOAuth": true,
    "signingCertificateType": "certificate",
    "encryptionCertificateType": "certificate"
  }
}
```



