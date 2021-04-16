---
title: Список androidWorkProfileCustomConfigurations
description: Список свойств и связей объектов AndroidWorkProfileCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b42f899931bb6c1a540e438486070e09c9449d73
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864482"
---
# <a name="list-androidworkprofilecustomconfigurations"></a><span data-ttu-id="d07bc-103">Список androidWorkProfileCustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="d07bc-103">List androidWorkProfileCustomConfigurations</span></span>

<span data-ttu-id="d07bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d07bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d07bc-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d07bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d07bc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d07bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d07bc-107">Список свойств и связей [объектов AndroidWorkProfileCustomConfiguration.](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d07bc-107">List properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d07bc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d07bc-108">Prerequisites</span></span>
<span data-ttu-id="d07bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d07bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d07bc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d07bc-111">Permission type</span></span>|<span data-ttu-id="d07bc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d07bc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d07bc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d07bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d07bc-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d07bc-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d07bc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d07bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d07bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d07bc-116">Not supported.</span></span>|
|<span data-ttu-id="d07bc-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d07bc-117">Application</span></span>|<span data-ttu-id="d07bc-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d07bc-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d07bc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d07bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d07bc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d07bc-120">Request headers</span></span>
|<span data-ttu-id="d07bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d07bc-121">Header</span></span>|<span data-ttu-id="d07bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d07bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d07bc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d07bc-123">Authorization</span></span>|<span data-ttu-id="d07bc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d07bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d07bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d07bc-125">Accept</span></span>|<span data-ttu-id="d07bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d07bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d07bc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d07bc-127">Request body</span></span>
<span data-ttu-id="d07bc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d07bc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d07bc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d07bc-129">Response</span></span>
<span data-ttu-id="d07bc-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d07bc-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d07bc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d07bc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d07bc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d07bc-132">Request</span></span>
<span data-ttu-id="d07bc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d07bc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="d07bc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d07bc-134">Response</span></span>
<span data-ttu-id="d07bc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d07bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1721

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
      "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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




