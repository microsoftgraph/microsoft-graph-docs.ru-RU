---
title: Получение Андроиддевицеовнервпнконфигуратион
description: Чтение свойств и связей объекта Андроиддевицеовнервпнконфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dd607bc44aeac4c68118f237767bb3c054ccc42b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759670"
---
# <a name="get-androiddeviceownervpnconfiguration"></a><span data-ttu-id="f936c-103">Получение Андроиддевицеовнервпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="f936c-103">Get androidDeviceOwnerVpnConfiguration</span></span>

> <span data-ttu-id="f936c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f936c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f936c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f936c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f936c-106">Чтение свойств и связей объекта [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f936c-106">Read properties and relationships of the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f936c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f936c-107">Prerequisites</span></span>
<span data-ttu-id="f936c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f936c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f936c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f936c-110">Permission type</span></span>|<span data-ttu-id="f936c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f936c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f936c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f936c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f936c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f936c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f936c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f936c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f936c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f936c-115">Not supported.</span></span>|
|<span data-ttu-id="f936c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f936c-116">Application</span></span>|<span data-ttu-id="f936c-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f936c-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f936c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f936c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f936c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f936c-119">Optional query parameters</span></span>
<span data-ttu-id="f936c-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f936c-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f936c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f936c-121">Request headers</span></span>
|<span data-ttu-id="f936c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f936c-122">Header</span></span>|<span data-ttu-id="f936c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f936c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f936c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f936c-124">Authorization</span></span>|<span data-ttu-id="f936c-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f936c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f936c-126">Accept</span><span class="sxs-lookup"><span data-stu-id="f936c-126">Accept</span></span>|<span data-ttu-id="f936c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f936c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f936c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f936c-128">Request body</span></span>
<span data-ttu-id="f936c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f936c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f936c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f936c-130">Response</span></span>
<span data-ttu-id="f936c-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f936c-131">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f936c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f936c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f936c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f936c-133">Request</span></span>
<span data-ttu-id="f936c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f936c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f936c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f936c-135">Response</span></span>
<span data-ttu-id="f936c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f936c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1698

{
  "value": {
    "@odata.type": "#microsoft.graph.androidDeviceOwnerVpnConfiguration",
    "id": "972962e3-62e3-9729-e362-2997e3622997",
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
    "authenticationMethod": "usernameAndPassword",
    "connectionName": "Connection Name value",
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
    "connectionType": "pulseSecure"
  }
}
```




