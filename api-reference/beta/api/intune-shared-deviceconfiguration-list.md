---
title: Перечисление объектов deviceConfiguration
description: Список свойств и связей объектов deviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ef87a8f188d1ca3130a969729a48fbee4b10d29f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027771"
---
# <a name="list-deviceconfigurations"></a><span data-ttu-id="4f0c2-103">Перечисление объектов deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4f0c2-103">List deviceConfigurations</span></span>

<span data-ttu-id="4f0c2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f0c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f0c2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f0c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f0c2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f0c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f0c2-107">Список свойств и связей объектов [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f0c2-107">List properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f0c2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4f0c2-108">Prerequisites</span></span>
<span data-ttu-id="4f0c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f0c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f0c2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f0c2-111">Permission type</span></span>|<span data-ttu-id="4f0c2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f0c2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f0c2-113">Делегированная (Рабочая или учебная учетная запись</span><span class="sxs-lookup"><span data-stu-id="4f0c2-113">Delegated (work or school account</span></span>||
| <span data-ttu-id="4f0c2-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="4f0c2-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4f0c2-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f0c2-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="4f0c2-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="4f0c2-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="4f0c2-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f0c2-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4f0c2-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f0c2-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f0c2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f0c2-119">Not supported.</span></span>|
|<span data-ttu-id="4f0c2-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f0c2-120">Application</span></span>||
| <span data-ttu-id="4f0c2-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="4f0c2-121">&nbsp; &nbsp; **Device configuration**</span></span> |<span data-ttu-id="4f0c2-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f0c2-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="4f0c2-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="4f0c2-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="4f0c2-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f0c2-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f0c2-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f0c2-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4f0c2-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4f0c2-126">Request headers</span></span>
|<span data-ttu-id="4f0c2-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f0c2-127">Header</span></span>|<span data-ttu-id="4f0c2-128">Значение</span><span class="sxs-lookup"><span data-stu-id="4f0c2-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f0c2-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f0c2-129">Authorization</span></span>|<span data-ttu-id="4f0c2-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f0c2-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f0c2-131">Accept</span><span class="sxs-lookup"><span data-stu-id="4f0c2-131">Accept</span></span>|<span data-ttu-id="4f0c2-132">application/json</span><span class="sxs-lookup"><span data-stu-id="4f0c2-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f0c2-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f0c2-133">Request body</span></span>
<span data-ttu-id="4f0c2-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f0c2-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f0c2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f0c2-135">Response</span></span>
<span data-ttu-id="4f0c2-136">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4f0c2-136">If successful, this method returns a `200 OK` response code and a collection of [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f0c2-137">Пример</span><span class="sxs-lookup"><span data-stu-id="4f0c2-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f0c2-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f0c2-138">Request</span></span>
<span data-ttu-id="4f0c2-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f0c2-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="4f0c2-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f0c2-140">Response</span></span>
<span data-ttu-id="4f0c2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f0c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1355

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfiguration",
      "id": "34977265-7265-3497-6572-973465729734",
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
      "version": 7
    }
  ]
}
```









