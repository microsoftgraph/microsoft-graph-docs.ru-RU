---
title: Перечисление объектов macOSCustomConfiguration
description: Список свойств и связей объектов macOSCustomConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 241bd8a436c26822725a91491f64fd3b3fdab351
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948440"
---
# <a name="list-macoscustomconfigurations"></a><span data-ttu-id="fd30e-103">Перечисление объектов macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd30e-103">List macOSCustomConfigurations</span></span>

> <span data-ttu-id="fd30e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd30e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd30e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd30e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd30e-106">Список свойств и связей объектов [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fd30e-106">List properties and relationships of the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd30e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fd30e-107">Prerequisites</span></span>
<span data-ttu-id="fd30e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd30e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd30e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd30e-110">Permission type</span></span>|<span data-ttu-id="fd30e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd30e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd30e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd30e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd30e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd30e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fd30e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd30e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd30e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd30e-115">Not supported.</span></span>|
|<span data-ttu-id="fd30e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd30e-116">Application</span></span>|<span data-ttu-id="fd30e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd30e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd30e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd30e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fd30e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fd30e-119">Request headers</span></span>
|<span data-ttu-id="fd30e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd30e-120">Header</span></span>|<span data-ttu-id="fd30e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fd30e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd30e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd30e-122">Authorization</span></span>|<span data-ttu-id="fd30e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd30e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd30e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fd30e-124">Accept</span></span>|<span data-ttu-id="fd30e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fd30e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd30e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fd30e-126">Request body</span></span>
<span data-ttu-id="fd30e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd30e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd30e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd30e-128">Response</span></span>
<span data-ttu-id="fd30e-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fd30e-129">If successful, this method returns a `200 OK` response code and a collection of [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd30e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fd30e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd30e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd30e-131">Request</span></span>
<span data-ttu-id="fd30e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd30e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="fd30e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd30e-133">Response</span></span>
<span data-ttu-id="fd30e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd30e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1491

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
      "id": "a253835d-835d-a253-5d83-53a25d8353a2",
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





