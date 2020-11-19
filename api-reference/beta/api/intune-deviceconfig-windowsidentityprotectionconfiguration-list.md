---
title: Список Виндовсидентитипротектионконфигуратионс
description: Список свойств и связей объектов Виндовсидентитипротектионконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ce63bd18b8cf61170e4f6450bda5e78929608c9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49203881"
---
# <a name="list-windowsidentityprotectionconfigurations"></a><span data-ttu-id="1697b-103">Список Виндовсидентитипротектионконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="1697b-103">List windowsIdentityProtectionConfigurations</span></span>

<span data-ttu-id="1697b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1697b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1697b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1697b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1697b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1697b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1697b-107">Список свойств и связей объектов [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1697b-107">List properties and relationships of the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1697b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1697b-108">Prerequisites</span></span>
<span data-ttu-id="1697b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1697b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1697b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1697b-111">Permission type</span></span>|<span data-ttu-id="1697b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1697b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1697b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1697b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1697b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1697b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1697b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1697b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1697b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1697b-116">Not supported.</span></span>|
|<span data-ttu-id="1697b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1697b-117">Application</span></span>|<span data-ttu-id="1697b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1697b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1697b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1697b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1697b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1697b-120">Request headers</span></span>
|<span data-ttu-id="1697b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1697b-121">Header</span></span>|<span data-ttu-id="1697b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1697b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1697b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1697b-123">Authorization</span></span>|<span data-ttu-id="1697b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1697b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1697b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1697b-125">Accept</span></span>|<span data-ttu-id="1697b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1697b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1697b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1697b-127">Request body</span></span>
<span data-ttu-id="1697b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1697b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1697b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1697b-129">Response</span></span>
<span data-ttu-id="1697b-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1697b-130">If successful, this method returns a `200 OK` response code and a collection of [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1697b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1697b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1697b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1697b-132">Request</span></span>
<span data-ttu-id="1697b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1697b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="1697b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1697b-134">Response</span></span>
<span data-ttu-id="1697b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1697b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1972

{
  "value": [
    {
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
  ]
}
```




