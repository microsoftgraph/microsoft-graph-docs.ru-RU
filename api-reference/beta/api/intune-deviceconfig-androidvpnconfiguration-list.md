---
title: Список Андроидвпнконфигуратионс
description: Список свойств и связей объектов Андроидвпнконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c08b486836794ed1f9d9bd987be9c52e06ae807d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36340942"
---
# <a name="list-androidvpnconfigurations"></a><span data-ttu-id="18563-103">Список Андроидвпнконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="18563-103">List androidVpnConfigurations</span></span>

> <span data-ttu-id="18563-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18563-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18563-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18563-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18563-106">Список свойств и связей объектов [андроидвпнконфигуратион](../resources/intune-deviceconfig-androidvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="18563-106">List properties and relationships of the [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18563-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="18563-107">Prerequisites</span></span>
<span data-ttu-id="18563-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18563-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18563-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18563-110">Permission type</span></span>|<span data-ttu-id="18563-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18563-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18563-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18563-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18563-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="18563-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="18563-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18563-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18563-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18563-115">Not supported.</span></span>|
|<span data-ttu-id="18563-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18563-116">Application</span></span>|<span data-ttu-id="18563-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="18563-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18563-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18563-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="18563-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18563-119">Request headers</span></span>
|<span data-ttu-id="18563-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18563-120">Header</span></span>|<span data-ttu-id="18563-121">Значение</span><span class="sxs-lookup"><span data-stu-id="18563-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18563-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18563-122">Authorization</span></span>|<span data-ttu-id="18563-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18563-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18563-124">Accept</span><span class="sxs-lookup"><span data-stu-id="18563-124">Accept</span></span>|<span data-ttu-id="18563-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18563-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18563-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="18563-126">Request body</span></span>
<span data-ttu-id="18563-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18563-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18563-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="18563-128">Response</span></span>
<span data-ttu-id="18563-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроидвпнконфигуратион](../resources/intune-deviceconfig-androidvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18563-129">If successful, this method returns a `200 OK` response code and a collection of [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18563-130">Пример</span><span class="sxs-lookup"><span data-stu-id="18563-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="18563-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="18563-131">Request</span></span>
<span data-ttu-id="18563-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18563-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="18563-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="18563-133">Response</span></span>
<span data-ttu-id="18563-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18563-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2196

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidVpnConfiguration",
      "id": "d4c48852-8852-d4c4-5288-c4d45288c4d4",
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






