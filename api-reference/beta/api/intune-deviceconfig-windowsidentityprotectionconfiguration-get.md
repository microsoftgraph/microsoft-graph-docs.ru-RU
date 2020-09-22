---
title: Получение Виндовсидентитипротектионконфигуратион
description: Чтение свойств и связей объекта Виндовсидентитипротектионконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b6570a8f883203c6216f3f73b987120f5076c619
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017761"
---
# <a name="get-windowsidentityprotectionconfiguration"></a><span data-ttu-id="ad9de-103">Получение Виндовсидентитипротектионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ad9de-103">Get windowsIdentityProtectionConfiguration</span></span>

<span data-ttu-id="ad9de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad9de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad9de-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad9de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad9de-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad9de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad9de-107">Чтение свойств и связей объекта [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ad9de-107">Read properties and relationships of the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad9de-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ad9de-108">Prerequisites</span></span>
<span data-ttu-id="ad9de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad9de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad9de-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad9de-111">Permission type</span></span>|<span data-ttu-id="ad9de-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad9de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad9de-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad9de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad9de-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad9de-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ad9de-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad9de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad9de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad9de-116">Not supported.</span></span>|
|<span data-ttu-id="ad9de-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad9de-117">Application</span></span>|<span data-ttu-id="ad9de-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad9de-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad9de-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad9de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad9de-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ad9de-120">Optional query parameters</span></span>
<span data-ttu-id="ad9de-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ad9de-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad9de-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad9de-122">Request headers</span></span>
|<span data-ttu-id="ad9de-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad9de-123">Header</span></span>|<span data-ttu-id="ad9de-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ad9de-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad9de-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad9de-125">Authorization</span></span>|<span data-ttu-id="ad9de-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad9de-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad9de-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ad9de-127">Accept</span></span>|<span data-ttu-id="ad9de-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ad9de-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad9de-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad9de-129">Request body</span></span>
<span data-ttu-id="ad9de-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad9de-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad9de-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad9de-131">Response</span></span>
<span data-ttu-id="ad9de-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad9de-132">If successful, this method returns a `200 OK` response code and [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad9de-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ad9de-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad9de-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad9de-134">Request</span></span>
<span data-ttu-id="ad9de-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad9de-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ad9de-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad9de-136">Response</span></span>
<span data-ttu-id="ad9de-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad9de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1866

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
    "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
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
    "useSecurityKeyForSignin": true,
    "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
    "pinMinimumLength": 0,
    "pinMaximumLength": 0,
    "pinUppercaseCharactersUsage": "required",
    "pinLowercaseCharactersUsage": "required",
    "pinSpecialCharactersUsage": "required",
    "pinExpirationInDays": 3,
    "pinPreviousBlockCount": 5,
    "pinRecoveryEnabled": true,
    "securityDeviceRequired": true,
    "unlockWithBiometricsEnabled": true,
    "useCertificatesForOnPremisesAuthEnabled": true,
    "windowsHelloForBusinessBlocked": true
  }
}
```






