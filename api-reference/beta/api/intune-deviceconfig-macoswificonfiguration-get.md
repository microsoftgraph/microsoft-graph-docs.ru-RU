---
title: Получение Макосвификонфигуратион
description: Чтение свойств и связей объекта Макосвификонфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f1cb39d8de8f1c4671629466fe0cb6c62de9bab
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36315066"
---
# <a name="get-macoswificonfiguration"></a><span data-ttu-id="7fe65-103">Получение Макосвификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="7fe65-103">Get macOSWiFiConfiguration</span></span>

> <span data-ttu-id="7fe65-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fe65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fe65-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7fe65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fe65-106">Чтение свойств и связей объекта [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7fe65-106">Read properties and relationships of the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fe65-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7fe65-107">Prerequisites</span></span>
<span data-ttu-id="7fe65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fe65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fe65-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fe65-110">Permission type</span></span>|<span data-ttu-id="7fe65-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fe65-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fe65-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fe65-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7fe65-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fe65-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7fe65-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fe65-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fe65-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fe65-115">Not supported.</span></span>|
|<span data-ttu-id="7fe65-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fe65-116">Application</span></span>|<span data-ttu-id="7fe65-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fe65-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fe65-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fe65-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7fe65-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7fe65-119">Optional query parameters</span></span>
<span data-ttu-id="7fe65-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7fe65-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7fe65-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7fe65-121">Request headers</span></span>
|<span data-ttu-id="7fe65-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7fe65-122">Header</span></span>|<span data-ttu-id="7fe65-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7fe65-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fe65-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7fe65-124">Authorization</span></span>|<span data-ttu-id="7fe65-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7fe65-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fe65-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7fe65-126">Accept</span></span>|<span data-ttu-id="7fe65-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7fe65-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fe65-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7fe65-128">Request body</span></span>
<span data-ttu-id="7fe65-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7fe65-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fe65-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7fe65-130">Response</span></span>
<span data-ttu-id="7fe65-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7fe65-131">If successful, this method returns a `200 OK` response code and [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fe65-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7fe65-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fe65-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fe65-133">Request</span></span>
<span data-ttu-id="7fe65-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fe65-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="7fe65-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fe65-135">Response</span></span>
<span data-ttu-id="7fe65-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7fe65-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1725

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
    "id": "471203fb-03fb-4712-fb03-1247fb031247",
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
    "wiFiSecurityType": "wpaPersonal",
    "proxySettings": "manual",
    "proxyManualAddress": "Proxy Manual Address value",
    "proxyManualPort": 15,
    "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
    "preSharedKey": "Pre Shared Key value"
  }
}
```






