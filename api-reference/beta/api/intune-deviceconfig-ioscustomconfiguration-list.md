---
title: Перечисление объектов iosCustomConfiguration
description: Список свойств и связей объектов iosCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 95aab8ca8c825653a99abc4a4d160f5a49c2f85d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082639"
---
# <a name="list-ioscustomconfigurations"></a><span data-ttu-id="24c7b-103">Перечисление объектов iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="24c7b-103">List iosCustomConfigurations</span></span>

<span data-ttu-id="24c7b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24c7b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24c7b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24c7b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24c7b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24c7b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24c7b-107">Список свойств и связей объектов [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="24c7b-107">List properties and relationships of the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24c7b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="24c7b-108">Prerequisites</span></span>
<span data-ttu-id="24c7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24c7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24c7b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24c7b-111">Permission type</span></span>|<span data-ttu-id="24c7b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24c7b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24c7b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24c7b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24c7b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="24c7b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="24c7b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24c7b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24c7b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24c7b-116">Not supported.</span></span>|
|<span data-ttu-id="24c7b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24c7b-117">Application</span></span>|<span data-ttu-id="24c7b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="24c7b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24c7b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24c7b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="24c7b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="24c7b-120">Request headers</span></span>
|<span data-ttu-id="24c7b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24c7b-121">Header</span></span>|<span data-ttu-id="24c7b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="24c7b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24c7b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24c7b-123">Authorization</span></span>|<span data-ttu-id="24c7b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24c7b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24c7b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="24c7b-125">Accept</span></span>|<span data-ttu-id="24c7b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24c7b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24c7b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24c7b-127">Request body</span></span>
<span data-ttu-id="24c7b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="24c7b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24c7b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="24c7b-129">Response</span></span>
<span data-ttu-id="24c7b-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24c7b-130">If successful, this method returns a `200 OK` response code and a collection of [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24c7b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="24c7b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="24c7b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="24c7b-132">Request</span></span>
<span data-ttu-id="24c7b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24c7b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="24c7b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="24c7b-134">Response</span></span>
<span data-ttu-id="24c7b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24c7b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1489

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCustomConfiguration",
      "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
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
      "payloadName": "Payload Name value",
      "payloadFileName": "Payload File Name value",
      "payload": "cGF5bG9hZA=="
    }
  ]
}
```






