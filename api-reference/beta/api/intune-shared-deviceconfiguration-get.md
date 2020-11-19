---
title: Get deviceConfiguration
description: Чтение свойств и связей объекта deviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fa4b965530673d4242a6c58594f0ef86f749d510
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49257466"
---
# <a name="get-deviceconfiguration"></a><span data-ttu-id="4eb95-103">Get deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4eb95-103">Get deviceConfiguration</span></span>

<span data-ttu-id="4eb95-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4eb95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4eb95-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eb95-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4eb95-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4eb95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4eb95-107">Чтение свойств и связей объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4eb95-107">Read properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4eb95-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4eb95-108">Prerequisites</span></span>
<span data-ttu-id="4eb95-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4eb95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4eb95-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4eb95-111">Permission type</span></span>|<span data-ttu-id="4eb95-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4eb95-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4eb95-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4eb95-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4eb95-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="4eb95-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4eb95-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4eb95-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="4eb95-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="4eb95-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="4eb95-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4eb95-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4eb95-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4eb95-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4eb95-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eb95-119">Not supported.</span></span>|
|<span data-ttu-id="4eb95-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="4eb95-120">Application</span></span>||
| <span data-ttu-id="4eb95-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="4eb95-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4eb95-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4eb95-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="4eb95-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="4eb95-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="4eb95-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4eb95-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4eb95-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4eb95-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4eb95-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4eb95-126">Optional query parameters</span></span>
<span data-ttu-id="4eb95-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4eb95-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4eb95-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4eb95-128">Request headers</span></span>
|<span data-ttu-id="4eb95-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4eb95-129">Header</span></span>|<span data-ttu-id="4eb95-130">Значение</span><span class="sxs-lookup"><span data-stu-id="4eb95-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4eb95-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4eb95-131">Authorization</span></span>|<span data-ttu-id="4eb95-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4eb95-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4eb95-133">Accept</span><span class="sxs-lookup"><span data-stu-id="4eb95-133">Accept</span></span>|<span data-ttu-id="4eb95-134">application/json</span><span class="sxs-lookup"><span data-stu-id="4eb95-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4eb95-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4eb95-135">Request body</span></span>
<span data-ttu-id="4eb95-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4eb95-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4eb95-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eb95-137">Response</span></span>
<span data-ttu-id="4eb95-138">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4eb95-138">If successful, this method returns a `200 OK` response code and [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eb95-139">Пример</span><span class="sxs-lookup"><span data-stu-id="4eb95-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="4eb95-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4eb95-140">Request</span></span>
<span data-ttu-id="4eb95-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4eb95-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="4eb95-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eb95-142">Response</span></span>
<span data-ttu-id="4eb95-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4eb95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







