---
title: Get windows10TeamGeneralConfiguration
description: Чтение свойств и связей объекта windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4922352cf9824683b18fe068bfea29b8cb86310b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157437"
---
# <a name="get-windows10teamgeneralconfiguration"></a><span data-ttu-id="2190b-103">Get windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="2190b-103">Get windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="2190b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2190b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2190b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2190b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2190b-106">Чтение свойств и связей объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2190b-106">Read properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2190b-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2190b-107">Prerequisites</span></span>
<span data-ttu-id="2190b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2190b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2190b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2190b-110">Permission type</span></span>|<span data-ttu-id="2190b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2190b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2190b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2190b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2190b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2190b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2190b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2190b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2190b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2190b-115">Not supported.</span></span>|
|<span data-ttu-id="2190b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2190b-116">Application</span></span>|<span data-ttu-id="2190b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2190b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2190b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2190b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2190b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2190b-119">Optional query parameters</span></span>
<span data-ttu-id="2190b-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2190b-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2190b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2190b-121">Request headers</span></span>
|<span data-ttu-id="2190b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2190b-122">Header</span></span>|<span data-ttu-id="2190b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2190b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2190b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2190b-124">Authorization</span></span>|<span data-ttu-id="2190b-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2190b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2190b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2190b-126">Accept</span></span>|<span data-ttu-id="2190b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2190b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2190b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2190b-128">Request body</span></span>
<span data-ttu-id="2190b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2190b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2190b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="2190b-130">Response</span></span>
<span data-ttu-id="2190b-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2190b-131">If successful, this method returns a `200 OK` response code and [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2190b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2190b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2190b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2190b-133">Request</span></span>
<span data-ttu-id="2190b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2190b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2190b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2190b-135">Response</span></span>
<span data-ttu-id="2190b-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2190b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1495

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
    "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "azureOperationalInsightsBlockTelemetry": true,
    "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
    "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
    "connectAppBlockAutoLaunch": true,
    "maintenanceWindowBlocked": true,
    "maintenanceWindowDurationInHours": 0,
    "maintenanceWindowStartTime": "11:59:09.3130000",
    "miracastChannel": "one",
    "miracastBlocked": true,
    "miracastRequirePin": true,
    "settingsBlockMyMeetingsAndFiles": true,
    "settingsBlockSessionResume": true,
    "settingsBlockSigninSuggestions": true,
    "settingsDefaultVolume": 5,
    "settingsScreenTimeoutInMinutes": 14,
    "settingsSessionTimeoutInMinutes": 15,
    "settingsSleepTimeoutInMinutes": 13,
    "welcomeScreenBlockAutomaticWakeUp": true,
    "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
    "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
  }
}
```




