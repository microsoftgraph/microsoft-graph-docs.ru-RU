---
title: Получение Андроидфорворквификонфигуратион
description: Чтение свойств и связей объекта Андроидфорворквификонфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d0b74aa620d4cd6d07f05f1dea1b198e41c778b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963018"
---
# <a name="get-androidforworkwificonfiguration"></a><span data-ttu-id="acfef-103">Получение Андроидфорворквификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="acfef-103">Get androidForWorkWiFiConfiguration</span></span>

> <span data-ttu-id="acfef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acfef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="acfef-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="acfef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acfef-106">Чтение свойств и связей объекта [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="acfef-106">Read properties and relationships of the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="acfef-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="acfef-107">Prerequisites</span></span>
<span data-ttu-id="acfef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acfef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acfef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="acfef-110">Permission type</span></span>|<span data-ttu-id="acfef-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="acfef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acfef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="acfef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="acfef-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="acfef-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="acfef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="acfef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acfef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acfef-115">Not supported.</span></span>|
|<span data-ttu-id="acfef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="acfef-116">Application</span></span>|<span data-ttu-id="acfef-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acfef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acfef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="acfef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="acfef-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="acfef-119">Optional query parameters</span></span>
<span data-ttu-id="acfef-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="acfef-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="acfef-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="acfef-121">Request headers</span></span>
|<span data-ttu-id="acfef-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="acfef-122">Header</span></span>|<span data-ttu-id="acfef-123">Значение</span><span class="sxs-lookup"><span data-stu-id="acfef-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acfef-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="acfef-124">Authorization</span></span>|<span data-ttu-id="acfef-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="acfef-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acfef-126">Accept</span><span class="sxs-lookup"><span data-stu-id="acfef-126">Accept</span></span>|<span data-ttu-id="acfef-127">application/json</span><span class="sxs-lookup"><span data-stu-id="acfef-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acfef-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="acfef-128">Request body</span></span>
<span data-ttu-id="acfef-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="acfef-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acfef-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="acfef-130">Response</span></span>
<span data-ttu-id="acfef-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроидфорворквификонфигуратион](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="acfef-131">If successful, this method returns a `200 OK` response code and [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acfef-132">Пример</span><span class="sxs-lookup"><span data-stu-id="acfef-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="acfef-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="acfef-133">Request</span></span>
<span data-ttu-id="acfef-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="acfef-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="acfef-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="acfef-135">Response</span></span>
<span data-ttu-id="acfef-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="acfef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1480

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
    "id": "58bcfe05-fe05-58bc-05fe-bc5805febc58",
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
    "networkName": "Network Name value",
    "ssid": "Ssid value",
    "connectAutomatically": true,
    "connectWhenNetworkNameIsHidden": true,
    "wiFiSecurityType": "wpaEnterprise"
  }
}
```





