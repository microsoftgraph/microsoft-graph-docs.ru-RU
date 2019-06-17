---
title: Получение объекта macOSDeviceFeaturesConfiguration
description: Чтение свойств и связей объекта macOSDeviceFeaturesConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4437be5924c9bb30b0d4b2bbf952cc867eef453
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34976857"
---
# <a name="get-macosdevicefeaturesconfiguration"></a><span data-ttu-id="a0a60-103">Получение объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0a60-103">Get macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="a0a60-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0a60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0a60-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0a60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0a60-106">Чтение свойств и связей объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0a60-106">Read properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0a60-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a0a60-107">Prerequisites</span></span>
<span data-ttu-id="a0a60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0a60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0a60-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0a60-110">Permission type</span></span>|<span data-ttu-id="a0a60-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0a60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0a60-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0a60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0a60-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0a60-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a0a60-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0a60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0a60-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0a60-115">Not supported.</span></span>|
|<span data-ttu-id="a0a60-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0a60-116">Application</span></span>|<span data-ttu-id="a0a60-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0a60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0a60-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0a60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0a60-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a0a60-119">Optional query parameters</span></span>
<span data-ttu-id="a0a60-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a0a60-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0a60-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0a60-121">Request headers</span></span>
|<span data-ttu-id="a0a60-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0a60-122">Header</span></span>|<span data-ttu-id="a0a60-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a0a60-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0a60-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0a60-124">Authorization</span></span>|<span data-ttu-id="a0a60-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0a60-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0a60-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a0a60-126">Accept</span></span>|<span data-ttu-id="a0a60-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a0a60-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0a60-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a0a60-128">Request body</span></span>
<span data-ttu-id="a0a60-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0a60-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0a60-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0a60-130">Response</span></span>
<span data-ttu-id="a0a60-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a0a60-131">If successful, this method returns a `200 OK` response code and [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0a60-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a0a60-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0a60-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0a60-133">Request</span></span>
<span data-ttu-id="a0a60-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0a60-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a0a60-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0a60-135">Response</span></span>
<span data-ttu-id="a0a60-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0a60-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2428

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
    "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
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
    "airPrintDestinations": [
      {
        "@odata.type": "microsoft.graph.airPrintDestination",
        "ipAddress": "Ip Address value",
        "resourcePath": "Resource Path value",
        "port": 4,
        "forceTls": true
      }
    ],
    "autoLaunchItems": [
      {
        "@odata.type": "microsoft.graph.macOSLaunchItem",
        "path": "Path value",
        "hide": true
      }
    ],
    "adminShowHostInfo": true,
    "loginWindowText": "Login Window Text value",
    "authorizedUsersListHidden": true,
    "authorizedUsersListHideLocalUsers": true,
    "authorizedUsersListHideMobileAccounts": true,
    "authorizedUsersListIncludeNetworkUsers": true,
    "authorizedUsersListHideAdminUsers": true,
    "authorizedUsersListShowOtherManagedUsers": true,
    "shutDownDisabled": true,
    "restartDisabled": true,
    "sleepDisabled": true,
    "consoleAccessDisabled": true,
    "shutDownDisabledWhileLoggedIn": true,
    "restartDisabledWhileLoggedIn": true,
    "powerOffDisabledWhileLoggedIn": true,
    "logOutDisabledWhileLoggedIn": true,
    "screenLockDisableImmediate": true
  }
}
```





