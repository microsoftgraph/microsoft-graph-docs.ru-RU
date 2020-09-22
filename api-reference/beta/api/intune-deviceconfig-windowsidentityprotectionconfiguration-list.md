---
title: Список Виндовсидентитипротектионконфигуратионс
description: Список свойств и связей объектов Виндовсидентитипротектионконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 97eca31bf22fd70059c4053a6150ec6c2bb0bd07
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056305"
---
# <a name="list-windowsidentityprotectionconfigurations"></a><span data-ttu-id="b6b56-103">Список Виндовсидентитипротектионконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="b6b56-103">List windowsIdentityProtectionConfigurations</span></span>

<span data-ttu-id="b6b56-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6b56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6b56-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6b56-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6b56-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6b56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6b56-107">Список свойств и связей объектов [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b6b56-107">List properties and relationships of the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6b56-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b6b56-108">Prerequisites</span></span>
<span data-ttu-id="b6b56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6b56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6b56-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6b56-111">Permission type</span></span>|<span data-ttu-id="b6b56-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6b56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6b56-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6b56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6b56-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6b56-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b6b56-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6b56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6b56-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6b56-116">Not supported.</span></span>|
|<span data-ttu-id="b6b56-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6b56-117">Application</span></span>|<span data-ttu-id="b6b56-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6b56-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6b56-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6b56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b6b56-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b6b56-120">Request headers</span></span>
|<span data-ttu-id="b6b56-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6b56-121">Header</span></span>|<span data-ttu-id="b6b56-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b6b56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6b56-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6b56-123">Authorization</span></span>|<span data-ttu-id="b6b56-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6b56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6b56-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6b56-125">Accept</span></span>|<span data-ttu-id="b6b56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6b56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6b56-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6b56-127">Request body</span></span>
<span data-ttu-id="b6b56-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6b56-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6b56-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6b56-129">Response</span></span>
<span data-ttu-id="b6b56-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b6b56-130">If successful, this method returns a `200 OK` response code and a collection of [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6b56-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b6b56-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6b56-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6b56-132">Request</span></span>
<span data-ttu-id="b6b56-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6b56-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b6b56-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6b56-134">Response</span></span>
<span data-ttu-id="b6b56-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6b56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






