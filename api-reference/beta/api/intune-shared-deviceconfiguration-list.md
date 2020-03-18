---
title: Перечисление объектов deviceConfiguration
description: Список свойств и связей объектов deviceConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 33cb2258b3635bfd523cf41a5cd6801b7a4c3fd6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801133"
---
# <a name="list-deviceconfigurations"></a><span data-ttu-id="a7be5-103">Перечисление объектов deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7be5-103">List deviceConfigurations</span></span>

> <span data-ttu-id="a7be5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7be5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7be5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7be5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7be5-106">Список свойств и связей объектов [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7be5-106">List properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7be5-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a7be5-107">Prerequisites</span></span>
<span data-ttu-id="a7be5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7be5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7be5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7be5-110">Permission type</span></span>|<span data-ttu-id="a7be5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7be5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7be5-112">Делегированная (Рабочая или учебная учетная запись</span><span class="sxs-lookup"><span data-stu-id="a7be5-112">Delegated (work or school account</span></span>||
| <span data-ttu-id="a7be5-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="a7be5-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="a7be5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7be5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="a7be5-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="a7be5-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a7be5-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7be5-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a7be5-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7be5-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7be5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7be5-118">Not supported.</span></span>|
|<span data-ttu-id="a7be5-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="a7be5-119">Application</span></span>||
| <span data-ttu-id="a7be5-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="a7be5-120">&nbsp; &nbsp; **Device configuration**</span></span> |<span data-ttu-id="a7be5-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7be5-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="a7be5-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="a7be5-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a7be5-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7be5-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7be5-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7be5-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a7be5-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a7be5-125">Request headers</span></span>
|<span data-ttu-id="a7be5-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7be5-126">Header</span></span>|<span data-ttu-id="a7be5-127">Значение</span><span class="sxs-lookup"><span data-stu-id="a7be5-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7be5-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7be5-128">Authorization</span></span>|<span data-ttu-id="a7be5-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7be5-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7be5-130">Accept</span><span class="sxs-lookup"><span data-stu-id="a7be5-130">Accept</span></span>|<span data-ttu-id="a7be5-131">application/json</span><span class="sxs-lookup"><span data-stu-id="a7be5-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7be5-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7be5-132">Request body</span></span>
<span data-ttu-id="a7be5-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7be5-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7be5-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7be5-134">Response</span></span>
<span data-ttu-id="a7be5-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a7be5-135">If successful, this method returns a `200 OK` response code and a collection of [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7be5-136">Пример</span><span class="sxs-lookup"><span data-stu-id="a7be5-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7be5-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7be5-137">Request</span></span>
<span data-ttu-id="a7be5-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7be5-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a7be5-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7be5-139">Response</span></span>
<span data-ttu-id="a7be5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7be5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







