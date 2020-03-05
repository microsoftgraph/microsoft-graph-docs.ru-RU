---
title: Перечисление объектов iosUpdateConfiguration
description: Список свойств и связей объектов iosUpdateConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 97e58dccbdc12478716af5f3c63653b940b9da7e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442623"
---
# <a name="list-iosupdateconfigurations"></a><span data-ttu-id="12435-103">Перечисление объектов iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="12435-103">List iosUpdateConfigurations</span></span>

<span data-ttu-id="12435-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="12435-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12435-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12435-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12435-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12435-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12435-107">Список свойств и связей объектов [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12435-107">List properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12435-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="12435-108">Prerequisites</span></span>
<span data-ttu-id="12435-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12435-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12435-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12435-111">Permission type</span></span>|<span data-ttu-id="12435-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12435-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12435-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12435-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12435-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="12435-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="12435-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12435-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12435-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12435-116">Not supported.</span></span>|
|<span data-ttu-id="12435-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12435-117">Application</span></span>|<span data-ttu-id="12435-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="12435-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12435-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12435-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="12435-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="12435-120">Request headers</span></span>
|<span data-ttu-id="12435-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12435-121">Header</span></span>|<span data-ttu-id="12435-122">Значение</span><span class="sxs-lookup"><span data-stu-id="12435-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12435-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12435-123">Authorization</span></span>|<span data-ttu-id="12435-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12435-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12435-125">Accept</span><span class="sxs-lookup"><span data-stu-id="12435-125">Accept</span></span>|<span data-ttu-id="12435-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12435-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12435-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12435-127">Request body</span></span>
<span data-ttu-id="12435-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12435-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12435-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="12435-129">Response</span></span>
<span data-ttu-id="12435-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12435-130">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12435-131">Пример</span><span class="sxs-lookup"><span data-stu-id="12435-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="12435-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="12435-132">Request</span></span>
<span data-ttu-id="12435-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12435-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="12435-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="12435-134">Response</span></span>
<span data-ttu-id="12435-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12435-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2005

{
  "value": [
    {
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
      "enforcedSoftwareUpdateDelayInDays": 1,
      "updateScheduleType": "alwaysUpdate",
      "customUpdateTimeWindows": [
        {
          "@odata.type": "microsoft.graph.customUpdateTimeWindow",
          "startDay": "monday",
          "endDay": "monday",
          "startTime": "12:03:30.2730000",
          "endTime": "12:03:02.3740000"
        }
      ]
    }
  ]
}
```





