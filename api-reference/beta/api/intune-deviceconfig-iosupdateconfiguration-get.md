---
title: Get iosUpdateConfiguration
description: Чтение свойств и связей объекта iosUpdateConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4af4965472453934c7f6f3d6d0325e733389b1c8
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41635883"
---
# <a name="get-iosupdateconfiguration"></a><span data-ttu-id="06801-103">Get iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="06801-103">Get iosUpdateConfiguration</span></span>

> <span data-ttu-id="06801-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06801-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06801-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06801-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06801-106">Чтение свойств и связей объекта [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06801-106">Read properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06801-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="06801-107">Prerequisites</span></span>
<span data-ttu-id="06801-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06801-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06801-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06801-110">Permission type</span></span>|<span data-ttu-id="06801-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06801-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06801-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06801-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06801-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="06801-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="06801-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06801-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06801-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06801-115">Not supported.</span></span>|
|<span data-ttu-id="06801-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06801-116">Application</span></span>|<span data-ttu-id="06801-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="06801-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06801-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06801-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06801-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="06801-119">Optional query parameters</span></span>
<span data-ttu-id="06801-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="06801-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06801-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06801-121">Request headers</span></span>
|<span data-ttu-id="06801-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06801-122">Header</span></span>|<span data-ttu-id="06801-123">Значение</span><span class="sxs-lookup"><span data-stu-id="06801-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06801-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06801-124">Authorization</span></span>|<span data-ttu-id="06801-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06801-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06801-126">Accept</span><span class="sxs-lookup"><span data-stu-id="06801-126">Accept</span></span>|<span data-ttu-id="06801-127">application/json</span><span class="sxs-lookup"><span data-stu-id="06801-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06801-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06801-128">Request body</span></span>
<span data-ttu-id="06801-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06801-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06801-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="06801-130">Response</span></span>
<span data-ttu-id="06801-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="06801-131">If successful, this method returns a `200 OK` response code and [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06801-132">Пример</span><span class="sxs-lookup"><span data-stu-id="06801-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="06801-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="06801-133">Request</span></span>
<span data-ttu-id="06801-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06801-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="06801-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="06801-135">Response</span></span>
<span data-ttu-id="06801-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06801-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1579

{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
    "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
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
    "isEnabled": true,
    "activeHoursStart": "12:00:05.5020000",
    "activeHoursEnd": "11:59:00.8990000",
    "desiredOsVersion": "Desired Os Version value",
    "scheduledInstallDays": [
      "monday"
    ],
    "utcTimeOffsetInMinutes": 6,
    "enforcedSoftwareUpdateDelayInDays": 1
  }
}
```





