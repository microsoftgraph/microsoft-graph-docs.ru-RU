---
title: Перечисление объектов windows10TeamGeneralConfiguration
description: Перечисление свойств и связей объектов windows10TeamGeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8cc7992b95d44a01795d49b4153e4cc2f9524b96
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760428"
---
# <a name="list-windows10teamgeneralconfigurations"></a><span data-ttu-id="023a0-103">Перечисление объектов windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="023a0-103">List windows10TeamGeneralConfigurations</span></span>

<span data-ttu-id="023a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="023a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="023a0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="023a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="023a0-106">Перечисление свойств и связей объектов [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="023a0-106">List properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="023a0-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="023a0-107">Prerequisites</span></span>
<span data-ttu-id="023a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="023a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="023a0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="023a0-110">Permission type</span></span>|<span data-ttu-id="023a0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="023a0-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="023a0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="023a0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="023a0-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="023a0-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="023a0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="023a0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="023a0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="023a0-115">Not supported.</span></span>|
|<span data-ttu-id="023a0-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="023a0-116">Application</span></span>|<span data-ttu-id="023a0-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="023a0-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="023a0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="023a0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="023a0-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="023a0-119">Request headers</span></span>
|<span data-ttu-id="023a0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="023a0-120">Header</span></span>|<span data-ttu-id="023a0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="023a0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="023a0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="023a0-122">Authorization</span></span>|<span data-ttu-id="023a0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="023a0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="023a0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="023a0-124">Accept</span></span>|<span data-ttu-id="023a0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="023a0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="023a0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="023a0-126">Request body</span></span>
<span data-ttu-id="023a0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="023a0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="023a0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="023a0-128">Response</span></span>
<span data-ttu-id="023a0-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="023a0-129">If successful, this method returns a `200 OK` response code and a collection of [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="023a0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="023a0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="023a0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="023a0-131">Request</span></span>
<span data-ttu-id="023a0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="023a0-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="023a0-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="023a0-133">Response</span></span>
<span data-ttu-id="023a0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="023a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




