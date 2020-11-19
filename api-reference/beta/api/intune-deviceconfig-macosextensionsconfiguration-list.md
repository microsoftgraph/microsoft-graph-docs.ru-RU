---
title: Список Макосекстенсионсконфигуратионс
description: Список свойств и связей объектов Макосекстенсионсконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bf8699b99c8522c8afdfdd0220d41fe83464b1ea
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49306655"
---
# <a name="list-macosextensionsconfigurations"></a><span data-ttu-id="72939-103">Список Макосекстенсионсконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="72939-103">List macOSExtensionsConfigurations</span></span>

<span data-ttu-id="72939-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72939-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72939-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72939-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72939-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72939-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72939-107">Список свойств и связей объектов [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="72939-107">List properties and relationships of the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72939-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="72939-108">Prerequisites</span></span>
<span data-ttu-id="72939-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72939-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72939-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72939-111">Permission type</span></span>|<span data-ttu-id="72939-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="72939-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72939-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72939-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72939-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="72939-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="72939-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72939-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72939-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72939-116">Not supported.</span></span>|
|<span data-ttu-id="72939-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72939-117">Application</span></span>|<span data-ttu-id="72939-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="72939-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72939-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72939-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="72939-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="72939-120">Request headers</span></span>
|<span data-ttu-id="72939-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72939-121">Header</span></span>|<span data-ttu-id="72939-122">Значение</span><span class="sxs-lookup"><span data-stu-id="72939-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72939-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72939-123">Authorization</span></span>|<span data-ttu-id="72939-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72939-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72939-125">Accept</span><span class="sxs-lookup"><span data-stu-id="72939-125">Accept</span></span>|<span data-ttu-id="72939-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72939-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72939-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72939-127">Request body</span></span>
<span data-ttu-id="72939-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72939-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72939-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="72939-129">Response</span></span>
<span data-ttu-id="72939-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [макосекстенсионсконфигуратион](../resources/intune-deviceconfig-macosextensionsconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72939-130">If successful, this method returns a `200 OK` response code and a collection of [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72939-131">Пример</span><span class="sxs-lookup"><span data-stu-id="72939-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="72939-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="72939-132">Request</span></span>
<span data-ttu-id="72939-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72939-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="72939-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="72939-134">Response</span></span>
<span data-ttu-id="72939-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72939-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2414

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
      "id": "c273f4f6-f4f6-c273-f6f4-73c2f6f473c2",
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
      "kernelExtensionOverridesAllowed": true,
      "kernelExtensionAllowedTeamIdentifiers": [
        "Kernel Extension Allowed Team Identifiers value"
      ],
      "kernelExtensionsAllowed": [
        {
          "@odata.type": "microsoft.graph.macOSKernelExtension",
          "teamIdentifier": "Team Identifier value",
          "bundleId": "Bundle Id value"
        }
      ],
      "systemExtensionsBlockOverride": true,
      "systemExtensionsAllowedTeamIdentifiers": [
        "System Extensions Allowed Team Identifiers value"
      ],
      "systemExtensionsAllowed": [
        {
          "@odata.type": "microsoft.graph.macOSSystemExtension",
          "teamIdentifier": "Team Identifier value",
          "bundleId": "Bundle Id value"
        }
      ],
      "systemExtensionsAllowedTypes": [
        {
          "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping",
          "teamIdentifier": "Team Identifier value",
          "allowedTypes": "networkExtensionsAllowed"
        }
      ]
    }
  ]
}
```




