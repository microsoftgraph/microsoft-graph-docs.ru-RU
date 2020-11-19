---
title: Перечисление объектов macOSCustomConfiguration
description: Список свойств и связей объектов macOSCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 19a078a1b5359d55ad2982842c15fd0e4b63f6c6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49278865"
---
# <a name="list-macoscustomconfigurations"></a><span data-ttu-id="a9895-103">Перечисление объектов macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9895-103">List macOSCustomConfigurations</span></span>

<span data-ttu-id="a9895-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9895-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9895-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9895-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9895-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9895-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9895-107">Список свойств и связей объектов [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9895-107">List properties and relationships of the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9895-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a9895-108">Prerequisites</span></span>
<span data-ttu-id="a9895-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9895-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9895-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9895-111">Permission type</span></span>|<span data-ttu-id="a9895-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9895-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9895-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9895-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9895-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9895-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a9895-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9895-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9895-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9895-116">Not supported.</span></span>|
|<span data-ttu-id="a9895-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9895-117">Application</span></span>|<span data-ttu-id="a9895-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9895-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9895-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9895-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a9895-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a9895-120">Request headers</span></span>
|<span data-ttu-id="a9895-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9895-121">Header</span></span>|<span data-ttu-id="a9895-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a9895-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9895-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9895-123">Authorization</span></span>|<span data-ttu-id="a9895-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9895-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9895-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a9895-125">Accept</span></span>|<span data-ttu-id="a9895-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9895-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9895-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9895-127">Request body</span></span>
<span data-ttu-id="a9895-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a9895-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9895-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9895-129">Response</span></span>
<span data-ttu-id="a9895-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a9895-130">If successful, this method returns a `200 OK` response code and a collection of [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9895-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a9895-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9895-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9895-132">Request</span></span>
<span data-ttu-id="a9895-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9895-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a9895-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9895-134">Response</span></span>
<span data-ttu-id="a9895-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9895-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




