---
title: Get deviceConfiguration
description: Чтение свойств и связей объекта deviceConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2138c57836df402c712bfd7cebeb0456b90aed80
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801154"
---
# <a name="get-deviceconfiguration"></a><span data-ttu-id="eaabd-103">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="eaabd-103">Get deviceConfiguration</span></span>

> <span data-ttu-id="eaabd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaabd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eaabd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eaabd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eaabd-106">Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eaabd-106">Read properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eaabd-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="eaabd-107">Prerequisites</span></span>
<span data-ttu-id="eaabd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaabd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaabd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eaabd-110">Permission type</span></span>|<span data-ttu-id="eaabd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eaabd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eaabd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eaabd-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="eaabd-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="eaabd-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="eaabd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eaabd-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="eaabd-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="eaabd-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="eaabd-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eaabd-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eaabd-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eaabd-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eaabd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaabd-118">Not supported.</span></span>|
|<span data-ttu-id="eaabd-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="eaabd-119">Application</span></span>||
| <span data-ttu-id="eaabd-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="eaabd-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="eaabd-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eaabd-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="eaabd-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="eaabd-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="eaabd-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eaabd-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaabd-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eaabd-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eaabd-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eaabd-125">Optional query parameters</span></span>
<span data-ttu-id="eaabd-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eaabd-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eaabd-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eaabd-127">Request headers</span></span>
|<span data-ttu-id="eaabd-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eaabd-128">Header</span></span>|<span data-ttu-id="eaabd-129">Значение</span><span class="sxs-lookup"><span data-stu-id="eaabd-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eaabd-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="eaabd-130">Authorization</span></span>|<span data-ttu-id="eaabd-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eaabd-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eaabd-132">Accept</span><span class="sxs-lookup"><span data-stu-id="eaabd-132">Accept</span></span>|<span data-ttu-id="eaabd-133">application/json</span><span class="sxs-lookup"><span data-stu-id="eaabd-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaabd-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eaabd-134">Request body</span></span>
<span data-ttu-id="eaabd-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eaabd-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eaabd-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="eaabd-136">Response</span></span>
<span data-ttu-id="eaabd-137">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="eaabd-137">If successful, this method returns a `200 OK` response code and [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaabd-138">Пример</span><span class="sxs-lookup"><span data-stu-id="eaabd-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="eaabd-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="eaabd-139">Request</span></span>
<span data-ttu-id="eaabd-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eaabd-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="eaabd-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaabd-141">Response</span></span>
<span data-ttu-id="eaabd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eaabd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1277

{
  "value": {
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
}
```







