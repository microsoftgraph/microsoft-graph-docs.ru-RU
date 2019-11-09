---
title: Get androidCustomConfiguration
description: Чтение свойств и связей объекта androidCustomConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: edfa4e17356fba3bd06bd8f4c195e88d61897ddf
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085024"
---
# <a name="get-androidcustomconfiguration"></a><span data-ttu-id="20d51-103">Get androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="20d51-103">Get androidCustomConfiguration</span></span>

> <span data-ttu-id="20d51-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20d51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20d51-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20d51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20d51-106">Чтение свойств и связей объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20d51-106">Read properties and relationships of the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20d51-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="20d51-107">Prerequisites</span></span>
<span data-ttu-id="20d51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20d51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20d51-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20d51-110">Permission type</span></span>|<span data-ttu-id="20d51-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20d51-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20d51-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20d51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20d51-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="20d51-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="20d51-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20d51-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20d51-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20d51-115">Not supported.</span></span>|
|<span data-ttu-id="20d51-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20d51-116">Application</span></span>|<span data-ttu-id="20d51-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="20d51-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20d51-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20d51-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20d51-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="20d51-119">Optional query parameters</span></span>
<span data-ttu-id="20d51-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="20d51-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20d51-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20d51-121">Request headers</span></span>
|<span data-ttu-id="20d51-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20d51-122">Header</span></span>|<span data-ttu-id="20d51-123">Значение</span><span class="sxs-lookup"><span data-stu-id="20d51-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20d51-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20d51-124">Authorization</span></span>|<span data-ttu-id="20d51-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20d51-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20d51-126">Accept</span><span class="sxs-lookup"><span data-stu-id="20d51-126">Accept</span></span>|<span data-ttu-id="20d51-127">application/json</span><span class="sxs-lookup"><span data-stu-id="20d51-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20d51-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20d51-128">Request body</span></span>
<span data-ttu-id="20d51-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="20d51-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20d51-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="20d51-130">Response</span></span>
<span data-ttu-id="20d51-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="20d51-131">If successful, this method returns a `200 OK` response code and [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20d51-132">Пример</span><span class="sxs-lookup"><span data-stu-id="20d51-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="20d51-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="20d51-133">Request</span></span>
<span data-ttu-id="20d51-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20d51-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="20d51-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="20d51-135">Response</span></span>
<span data-ttu-id="20d51-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20d51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1569

{
  "value": {
    "@odata.type": "#microsoft.graph.androidCustomConfiguration",
    "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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
}
```






