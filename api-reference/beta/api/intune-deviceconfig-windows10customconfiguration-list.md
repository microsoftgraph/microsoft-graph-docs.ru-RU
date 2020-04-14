---
title: Перечисление объектов windows10CustomConfiguration
description: Список свойств и связей объектов windows10CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bc14664d60a7c476b011813b3c9773e823a64c8c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43340288"
---
# <a name="list-windows10customconfigurations"></a><span data-ttu-id="c0e53-103">Перечисление объектов windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="c0e53-103">List windows10CustomConfigurations</span></span>

<span data-ttu-id="c0e53-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0e53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0e53-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0e53-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0e53-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0e53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0e53-107">Список свойств и связей объектов [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0e53-107">List properties and relationships of the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0e53-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c0e53-108">Prerequisites</span></span>
<span data-ttu-id="c0e53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0e53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0e53-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0e53-111">Permission type</span></span>|<span data-ttu-id="c0e53-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0e53-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0e53-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0e53-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0e53-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0e53-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c0e53-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0e53-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0e53-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0e53-116">Not supported.</span></span>|
|<span data-ttu-id="c0e53-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="c0e53-117">Application</span></span>|<span data-ttu-id="c0e53-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0e53-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0e53-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0e53-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c0e53-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c0e53-120">Request headers</span></span>
|<span data-ttu-id="c0e53-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0e53-121">Header</span></span>|<span data-ttu-id="c0e53-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c0e53-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0e53-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0e53-123">Authorization</span></span>|<span data-ttu-id="c0e53-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0e53-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0e53-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c0e53-125">Accept</span></span>|<span data-ttu-id="c0e53-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0e53-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0e53-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0e53-127">Request body</span></span>
<span data-ttu-id="c0e53-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0e53-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0e53-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0e53-129">Response</span></span>
<span data-ttu-id="c0e53-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0e53-130">If successful, this method returns a `200 OK` response code and a collection of [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0e53-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c0e53-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0e53-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0e53-132">Request</span></span>
<span data-ttu-id="c0e53-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0e53-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="c0e53-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0e53-134">Response</span></span>
<span data-ttu-id="c0e53-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0e53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1669

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
      "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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
      "omaSettings": [
        {
          "@odata.type": "microsoft.graph.omaSettingInteger",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value",
          "value": 5,
          "isReadOnly": true
        }
      ]
    }
  ]
}
```



