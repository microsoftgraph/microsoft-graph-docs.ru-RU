---
title: Перечисление объектов windows10TeamGeneralConfiguration
description: Перечисление свойств и связей объектов windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 89421a0a605285644af3627ebb804751f4411f7b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951007"
---
# <a name="list-windows10teamgeneralconfigurations"></a><span data-ttu-id="74ee2-103">Перечисление объектов windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="74ee2-103">List windows10TeamGeneralConfigurations</span></span>

> <span data-ttu-id="74ee2-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="74ee2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74ee2-105">Перечисление свойств и связей объектов [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="74ee2-105">List properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="74ee2-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="74ee2-106">Prerequisites</span></span>
<span data-ttu-id="74ee2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74ee2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74ee2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74ee2-109">Permission type</span></span>|<span data-ttu-id="74ee2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="74ee2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74ee2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74ee2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="74ee2-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="74ee2-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="74ee2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74ee2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74ee2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74ee2-114">Not supported.</span></span>|
|<span data-ttu-id="74ee2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74ee2-115">Application</span></span>|<span data-ttu-id="74ee2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74ee2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74ee2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74ee2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="74ee2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74ee2-118">Request headers</span></span>
|<span data-ttu-id="74ee2-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74ee2-119">Header</span></span>|<span data-ttu-id="74ee2-120">Значение</span><span class="sxs-lookup"><span data-stu-id="74ee2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74ee2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="74ee2-121">Authorization</span></span>|<span data-ttu-id="74ee2-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="74ee2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74ee2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="74ee2-123">Accept</span></span>|<span data-ttu-id="74ee2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="74ee2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74ee2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="74ee2-125">Request body</span></span>
<span data-ttu-id="74ee2-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="74ee2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74ee2-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="74ee2-127">Response</span></span>
<span data-ttu-id="74ee2-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="74ee2-128">If successful, this method returns a `200 OK` response code and a collection of [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74ee2-129">Пример</span><span class="sxs-lookup"><span data-stu-id="74ee2-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="74ee2-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="74ee2-130">Request</span></span>
<span data-ttu-id="74ee2-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74ee2-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="74ee2-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="74ee2-132">Response</span></span>
<span data-ttu-id="74ee2-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="74ee2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



