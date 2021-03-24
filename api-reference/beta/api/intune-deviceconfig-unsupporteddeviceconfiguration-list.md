---
title: Список неподдерживаемойDeviceConfigurations
description: Список свойств и связей неподдерживаемогоDeviceConfiguration объектов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d7aaab8d728ba811639f0a28037e0e78bbe767fc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129589"
---
# <a name="list-unsupporteddeviceconfigurations"></a><span data-ttu-id="60e98-103">Список неподдерживаемойDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="60e98-103">List unsupportedDeviceConfigurations</span></span>

<span data-ttu-id="60e98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60e98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60e98-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60e98-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60e98-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60e98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60e98-107">Список свойств и связей [неподдерживаемогоDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) объектов.</span><span class="sxs-lookup"><span data-stu-id="60e98-107">List properties and relationships of the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60e98-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="60e98-108">Prerequisites</span></span>
<span data-ttu-id="60e98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60e98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60e98-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60e98-111">Permission type</span></span>|<span data-ttu-id="60e98-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60e98-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60e98-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60e98-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60e98-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60e98-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="60e98-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60e98-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60e98-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60e98-116">Not supported.</span></span>|
|<span data-ttu-id="60e98-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="60e98-117">Application</span></span>|<span data-ttu-id="60e98-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60e98-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="60e98-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60e98-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="60e98-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="60e98-120">Request headers</span></span>
|<span data-ttu-id="60e98-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="60e98-121">Header</span></span>|<span data-ttu-id="60e98-122">Значение</span><span class="sxs-lookup"><span data-stu-id="60e98-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60e98-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="60e98-123">Authorization</span></span>|<span data-ttu-id="60e98-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60e98-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60e98-125">Accept</span><span class="sxs-lookup"><span data-stu-id="60e98-125">Accept</span></span>|<span data-ttu-id="60e98-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60e98-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60e98-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60e98-127">Request body</span></span>
<span data-ttu-id="60e98-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60e98-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60e98-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="60e98-129">Response</span></span>
<span data-ttu-id="60e98-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="60e98-130">If successful, this method returns a `200 OK` response code and a collection of [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60e98-131">Пример</span><span class="sxs-lookup"><span data-stu-id="60e98-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="60e98-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="60e98-132">Request</span></span>
<span data-ttu-id="60e98-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60e98-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="60e98-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="60e98-134">Response</span></span>
<span data-ttu-id="60e98-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="60e98-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1656

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
      "id": "f80d6fc8-6fc8-f80d-c86f-0df8c86f0df8",
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
      "originalEntityTypeName": "Original Entity Type Name value",
      "details": [
        {
          "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
          "message": "Message value",
          "propertyName": "Property Name value"
        }
      ]
    }
  ]
}
```




