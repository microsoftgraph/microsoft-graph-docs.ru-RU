---
title: Перечисление объектов windows10TeamGeneralConfiguration
description: Перечисление свойств и связей объектов windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b1635459cc104a2ad89e949ce33e224184f51d5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259768"
---
# <a name="list-windows10teamgeneralconfigurations"></a><span data-ttu-id="d8067-103">Перечисление объектов windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8067-103">List windows10TeamGeneralConfigurations</span></span>

> <span data-ttu-id="d8067-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8067-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8067-105">Перечисление свойств и связей объектов [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8067-105">List properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8067-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d8067-106">Prerequisites</span></span>
<span data-ttu-id="d8067-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d8067-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d8067-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8067-109">Permission type</span></span>|<span data-ttu-id="d8067-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8067-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8067-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8067-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d8067-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8067-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d8067-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8067-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8067-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8067-114">Not supported.</span></span>|
|<span data-ttu-id="d8067-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8067-115">Application</span></span>|<span data-ttu-id="d8067-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8067-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8067-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8067-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d8067-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8067-118">Request headers</span></span>
|<span data-ttu-id="d8067-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8067-119">Header</span></span>|<span data-ttu-id="d8067-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d8067-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8067-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8067-121">Authorization</span></span>|<span data-ttu-id="d8067-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d8067-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8067-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d8067-123">Accept</span></span>|<span data-ttu-id="d8067-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d8067-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8067-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8067-125">Request body</span></span>
<span data-ttu-id="d8067-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8067-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8067-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8067-127">Response</span></span>
<span data-ttu-id="d8067-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d8067-128">If successful, this method returns a `200 OK` response code and a collection of [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8067-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d8067-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8067-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8067-130">Request</span></span>
<span data-ttu-id="d8067-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8067-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="d8067-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8067-132">Response</span></span>
<span data-ttu-id="d8067-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d8067-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1463

{
  "value": [
    {
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
  ]
}
```



