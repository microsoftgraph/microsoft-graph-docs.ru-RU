---
title: Список windows10DeviceFirmwareConfigurationInterfaces
description: Список свойств и связей объектов Windows10DeviceFirmwareConfigurationInterface.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c536634d482c1a5fc88288a73ef214a26e84c119
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867177"
---
# <a name="list-windows10devicefirmwareconfigurationinterfaces"></a><span data-ttu-id="356fd-103">Список windows10DeviceFirmwareConfigurationInterfaces</span><span class="sxs-lookup"><span data-stu-id="356fd-103">List windows10DeviceFirmwareConfigurationInterfaces</span></span>

<span data-ttu-id="356fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="356fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="356fd-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="356fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="356fd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="356fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="356fd-107">Список свойств и связей [объектов Windows10DeviceFirmwareConfigurationInterface.](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)</span><span class="sxs-lookup"><span data-stu-id="356fd-107">List properties and relationships of the [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="356fd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="356fd-108">Prerequisites</span></span>
<span data-ttu-id="356fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="356fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="356fd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="356fd-111">Permission type</span></span>|<span data-ttu-id="356fd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="356fd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="356fd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="356fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="356fd-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="356fd-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="356fd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="356fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="356fd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="356fd-116">Not supported.</span></span>|
|<span data-ttu-id="356fd-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="356fd-117">Application</span></span>|<span data-ttu-id="356fd-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="356fd-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="356fd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="356fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="356fd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="356fd-120">Request headers</span></span>
|<span data-ttu-id="356fd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="356fd-121">Header</span></span>|<span data-ttu-id="356fd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="356fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="356fd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="356fd-123">Authorization</span></span>|<span data-ttu-id="356fd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="356fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="356fd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="356fd-125">Accept</span></span>|<span data-ttu-id="356fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="356fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="356fd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="356fd-127">Request body</span></span>
<span data-ttu-id="356fd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="356fd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="356fd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="356fd-129">Response</span></span>
<span data-ttu-id="356fd-130">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="356fd-130">If successful, this method returns a `200 OK` response code and a collection of [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="356fd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="356fd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="356fd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="356fd-132">Request</span></span>
<span data-ttu-id="356fd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="356fd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="356fd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="356fd-134">Response</span></span>
<span data-ttu-id="356fd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="356fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1766

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
      "id": "96474363-4363-9647-6343-479663434796",
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
      "changeUefiSettingsPermission": "none",
      "virtualizationOfCpuAndIO": "enabled",
      "cameras": "enabled",
      "microphonesAndSpeakers": "enabled",
      "radios": "enabled",
      "bootFromExternalMedia": "enabled",
      "bootFromBuiltInNetworkAdapters": "enabled",
      "windowsPlatformBinaryTable": "enabled",
      "simultaneousMultiThreading": "enabled"
    }
  ]
}
```




