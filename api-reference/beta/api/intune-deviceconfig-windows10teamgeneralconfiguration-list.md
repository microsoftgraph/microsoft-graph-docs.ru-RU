---
title: Перечисление объектов windows10TeamGeneralConfiguration
description: Перечисление свойств и связей объектов windows10TeamGeneralConfiguration.
ms.openlocfilehash: 350f67c881d1c154df3bb9066c9cb23321817104
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078866"
---
# <a name="list-windows10teamgeneralconfigurations"></a><span data-ttu-id="181ea-103">Перечисление объектов windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="181ea-103">List windows10TeamGeneralConfigurations</span></span>

> <span data-ttu-id="181ea-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="181ea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="181ea-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="181ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="181ea-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="181ea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="181ea-107">Перечисление свойств и связей объектов [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="181ea-107">List properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="181ea-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="181ea-108">Prerequisites</span></span>
<span data-ttu-id="181ea-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="181ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="181ea-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="181ea-111">Permission type</span></span>|<span data-ttu-id="181ea-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="181ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="181ea-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="181ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="181ea-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="181ea-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="181ea-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="181ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="181ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="181ea-116">Not supported.</span></span>|
|<span data-ttu-id="181ea-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="181ea-117">Application</span></span>|<span data-ttu-id="181ea-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="181ea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="181ea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="181ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="181ea-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="181ea-120">Request headers</span></span>
|<span data-ttu-id="181ea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="181ea-121">Header</span></span>|<span data-ttu-id="181ea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="181ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="181ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="181ea-123">Authorization</span></span>|<span data-ttu-id="181ea-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="181ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="181ea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="181ea-125">Accept</span></span>|<span data-ttu-id="181ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="181ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="181ea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="181ea-127">Request body</span></span>
<span data-ttu-id="181ea-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="181ea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="181ea-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="181ea-129">Response</span></span>
<span data-ttu-id="181ea-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="181ea-130">If successful, this method returns a `200 OK` response code and a collection of [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="181ea-131">Пример</span><span class="sxs-lookup"><span data-stu-id="181ea-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="181ea-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="181ea-132">Request</span></span>
<span data-ttu-id="181ea-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="181ea-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="181ea-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="181ea-134">Response</span></span>
<span data-ttu-id="181ea-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="181ea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1571

{
  "value": [
    {
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
  ]
}
```





