---
title: Get deviceConfiguration
description: Чтение свойств и связей объекта deviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5172e39611ac2556cfed544f587d4b6c445736e6
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201072"
---
# <a name="get-deviceconfiguration"></a><span data-ttu-id="e7c23-103">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e7c23-103">Get deviceConfiguration</span></span>

> <span data-ttu-id="e7c23-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7c23-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7c23-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7c23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7c23-106">Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7c23-106">Read properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7c23-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e7c23-107">Prerequisites</span></span>
<span data-ttu-id="e7c23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7c23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7c23-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7c23-110">Permission type</span></span>|<span data-ttu-id="e7c23-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7c23-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7c23-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7c23-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e7c23-113">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="e7c23-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e7c23-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7c23-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="e7c23-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="e7c23-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e7c23-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7c23-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e7c23-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7c23-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7c23-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7c23-118">Not supported.</span></span>|
|<span data-ttu-id="e7c23-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7c23-119">Application</span></span>||
| <span data-ttu-id="e7c23-120">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="e7c23-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e7c23-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7c23-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="e7c23-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="e7c23-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e7c23-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7c23-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7c23-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7c23-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7c23-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e7c23-125">Optional query parameters</span></span>
<span data-ttu-id="e7c23-126">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e7c23-126">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7c23-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7c23-127">Request headers</span></span>
|<span data-ttu-id="e7c23-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7c23-128">Header</span></span>|<span data-ttu-id="e7c23-129">Значение</span><span class="sxs-lookup"><span data-stu-id="e7c23-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7c23-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7c23-130">Authorization</span></span>|<span data-ttu-id="e7c23-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7c23-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7c23-132">Accept</span><span class="sxs-lookup"><span data-stu-id="e7c23-132">Accept</span></span>|<span data-ttu-id="e7c23-133">application/json</span><span class="sxs-lookup"><span data-stu-id="e7c23-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7c23-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e7c23-134">Request body</span></span>
<span data-ttu-id="e7c23-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e7c23-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7c23-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7c23-136">Response</span></span>
<span data-ttu-id="e7c23-137">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e7c23-137">If successful, this method returns a `200 OK` response code and [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7c23-138">Пример</span><span class="sxs-lookup"><span data-stu-id="e7c23-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7c23-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7c23-139">Request</span></span>
<span data-ttu-id="e7c23-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7c23-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e7c23-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7c23-141">Response</span></span>
<span data-ttu-id="e7c23-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e7c23-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




