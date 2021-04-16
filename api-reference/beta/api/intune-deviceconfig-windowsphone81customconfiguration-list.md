---
title: Перечисление объектов windowsPhone81CustomConfiguration
description: Перечисление свойств и связей объектов windowsPhone81CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2015a59af02199158972698c3076980910cfdc96
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867170"
---
# <a name="list-windowsphone81customconfigurations"></a><span data-ttu-id="2b425-103">Перечисление объектов windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b425-103">List windowsPhone81CustomConfigurations</span></span>

<span data-ttu-id="2b425-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b425-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b425-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b425-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b425-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b425-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b425-107">Перечисление свойств и связей объектов [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b425-107">List properties and relationships of the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b425-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2b425-108">Prerequisites</span></span>
<span data-ttu-id="2b425-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b425-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b425-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b425-111">Permission type</span></span>|<span data-ttu-id="2b425-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b425-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b425-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b425-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b425-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b425-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2b425-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b425-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b425-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b425-116">Not supported.</span></span>|
|<span data-ttu-id="2b425-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="2b425-117">Application</span></span>|<span data-ttu-id="2b425-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b425-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b425-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b425-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2b425-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2b425-120">Request headers</span></span>
|<span data-ttu-id="2b425-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b425-121">Header</span></span>|<span data-ttu-id="2b425-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2b425-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b425-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b425-123">Authorization</span></span>|<span data-ttu-id="2b425-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b425-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b425-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b425-125">Accept</span></span>|<span data-ttu-id="2b425-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b425-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b425-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b425-127">Request body</span></span>
<span data-ttu-id="2b425-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b425-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b425-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b425-129">Response</span></span>
<span data-ttu-id="2b425-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b425-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b425-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2b425-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b425-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b425-132">Request</span></span>
<span data-ttu-id="2b425-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b425-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="2b425-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b425-134">Response</span></span>
<span data-ttu-id="2b425-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b425-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1717

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
      "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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
          "@odata.type": "microsoft.graph.omaSetting",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value",
          "secretReferenceValueId": "Secret Reference Value Id value",
          "isEncrypted": true
        }
      ]
    }
  ]
}
```




