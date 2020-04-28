---
title: Список Андроидфорворквпнконфигуратионс
description: Список свойств и связей объектов androidForWorkVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0e58dfd3cc62a083f9cc0e32dba1401e0039a96d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43345113"
---
# <a name="list-androidforworkvpnconfigurations"></a><span data-ttu-id="93f74-103">Список Андроидфорворквпнконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="93f74-103">List androidForWorkVpnConfigurations</span></span>

<span data-ttu-id="93f74-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93f74-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93f74-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93f74-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93f74-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93f74-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93f74-107">Список свойств и связей объектов [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="93f74-107">List properties and relationships of the [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93f74-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="93f74-108">Prerequisites</span></span>
<span data-ttu-id="93f74-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93f74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93f74-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93f74-111">Permission type</span></span>|<span data-ttu-id="93f74-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="93f74-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93f74-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93f74-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93f74-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="93f74-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="93f74-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93f74-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93f74-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93f74-116">Not supported.</span></span>|
|<span data-ttu-id="93f74-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93f74-117">Application</span></span>|<span data-ttu-id="93f74-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="93f74-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93f74-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93f74-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="93f74-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="93f74-120">Request headers</span></span>
|<span data-ttu-id="93f74-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93f74-121">Header</span></span>|<span data-ttu-id="93f74-122">Значение</span><span class="sxs-lookup"><span data-stu-id="93f74-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93f74-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93f74-123">Authorization</span></span>|<span data-ttu-id="93f74-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93f74-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93f74-125">Accept</span><span class="sxs-lookup"><span data-stu-id="93f74-125">Accept</span></span>|<span data-ttu-id="93f74-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93f74-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93f74-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="93f74-127">Request body</span></span>
<span data-ttu-id="93f74-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="93f74-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93f74-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="93f74-129">Response</span></span>
<span data-ttu-id="93f74-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93f74-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93f74-131">Пример</span><span class="sxs-lookup"><span data-stu-id="93f74-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="93f74-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="93f74-132">Request</span></span>
<span data-ttu-id="93f74-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93f74-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="93f74-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="93f74-134">Response</span></span>
<span data-ttu-id="93f74-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93f74-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2203

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
      "id": "2cf4c52c-c52c-2cf4-2cc5-f42c2cc5f42c",
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
      "connectionName": "Connection Name value",
      "connectionType": "pulseSecure",
      "role": "Role value",
      "realm": "Realm value",
      "servers": [
        {
          "@odata.type": "microsoft.graph.vpnServer",
          "description": "Description value",
          "address": "Address value",
          "isDefaultServer": true
        }
      ],
      "fingerprint": "Fingerprint value",
      "customData": [
        {
          "@odata.type": "microsoft.graph.keyValue",
          "key": "Key value",
          "value": "Value value"
        }
      ],
      "customKeyValueData": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "authenticationMethod": "usernameAndPassword"
    }
  ]
}
```



