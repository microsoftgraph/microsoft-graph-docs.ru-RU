---
title: Get windows10TeamGeneralConfiguration
description: Чтение свойств и связей объекта windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 340dc198543d67c8829b06d149bb77a9f11955bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889084"
---
# <a name="get-windows10teamgeneralconfiguration"></a><span data-ttu-id="ef584-103">Get windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="ef584-103">Get windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="ef584-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ef584-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef584-105">Чтение свойств и связей объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef584-105">Read properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef584-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ef584-106">Prerequisites</span></span>
<span data-ttu-id="ef584-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef584-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef584-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef584-109">Permission type</span></span>|<span data-ttu-id="ef584-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef584-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef584-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef584-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ef584-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef584-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ef584-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef584-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef584-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef584-114">Not supported.</span></span>|
|<span data-ttu-id="ef584-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef584-115">Application</span></span>|<span data-ttu-id="ef584-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef584-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef584-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef584-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ef584-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ef584-118">Optional query parameters</span></span>
<span data-ttu-id="ef584-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ef584-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ef584-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef584-120">Request headers</span></span>
|<span data-ttu-id="ef584-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef584-121">Header</span></span>|<span data-ttu-id="ef584-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ef584-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef584-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef584-123">Authorization</span></span>|<span data-ttu-id="ef584-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ef584-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef584-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef584-125">Accept</span></span>|<span data-ttu-id="ef584-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef584-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef584-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef584-127">Request body</span></span>
<span data-ttu-id="ef584-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef584-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef584-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef584-129">Response</span></span>
<span data-ttu-id="ef584-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ef584-130">If successful, this method returns a `200 OK` response code and [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef584-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ef584-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef584-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef584-132">Request</span></span>
<span data-ttu-id="ef584-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef584-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ef584-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef584-134">Response</span></span>
<span data-ttu-id="ef584-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ef584-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



