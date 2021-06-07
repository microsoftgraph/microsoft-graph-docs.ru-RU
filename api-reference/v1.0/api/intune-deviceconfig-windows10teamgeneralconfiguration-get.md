---
title: Get windows10TeamGeneralConfiguration
description: Чтение свойств и связей объекта windows10TeamGeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af5da45ed00c02ec770d9ce534efbbb0b6503d66
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760435"
---
# <a name="get-windows10teamgeneralconfiguration"></a><span data-ttu-id="015c8-103">Get windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="015c8-103">Get windows10TeamGeneralConfiguration</span></span>

<span data-ttu-id="015c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="015c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="015c8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="015c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="015c8-106">Чтение свойств и связей объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="015c8-106">Read properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="015c8-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="015c8-107">Prerequisites</span></span>
<span data-ttu-id="015c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="015c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="015c8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="015c8-110">Permission type</span></span>|<span data-ttu-id="015c8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="015c8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="015c8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="015c8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="015c8-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="015c8-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="015c8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="015c8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="015c8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="015c8-115">Not supported.</span></span>|
|<span data-ttu-id="015c8-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="015c8-116">Application</span></span>|<span data-ttu-id="015c8-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="015c8-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="015c8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="015c8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="015c8-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="015c8-119">Optional query parameters</span></span>
<span data-ttu-id="015c8-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="015c8-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="015c8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="015c8-121">Request headers</span></span>
|<span data-ttu-id="015c8-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="015c8-122">Header</span></span>|<span data-ttu-id="015c8-123">Значение</span><span class="sxs-lookup"><span data-stu-id="015c8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="015c8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="015c8-124">Authorization</span></span>|<span data-ttu-id="015c8-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="015c8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="015c8-126">Accept</span><span class="sxs-lookup"><span data-stu-id="015c8-126">Accept</span></span>|<span data-ttu-id="015c8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="015c8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="015c8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="015c8-128">Request body</span></span>
<span data-ttu-id="015c8-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="015c8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="015c8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="015c8-130">Response</span></span>
<span data-ttu-id="015c8-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="015c8-131">If successful, this method returns a `200 OK` response code and [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="015c8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="015c8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="015c8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="015c8-133">Request</span></span>
<span data-ttu-id="015c8-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="015c8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="015c8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="015c8-135">Response</span></span>
<span data-ttu-id="015c8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="015c8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1395

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
    "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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




