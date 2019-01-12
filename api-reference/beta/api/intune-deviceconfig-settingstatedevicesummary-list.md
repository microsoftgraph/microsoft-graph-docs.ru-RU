---
title: Перечисление объектов settingStateDeviceSummary
description: Список свойств и связей объектов settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 40fd4d5b37834dd323f109a09e6fc2b197704e7a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914964"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="e0930-103">Перечисление объектов settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e0930-103">List settingStateDeviceSummaries</span></span>

> <span data-ttu-id="e0930-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e0930-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0930-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0930-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0930-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e0930-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0930-107">Список свойств и связей объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e0930-107">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0930-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e0930-108">Prerequisites</span></span>
<span data-ttu-id="e0930-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0930-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0930-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0930-111">Permission type</span></span>|<span data-ttu-id="e0930-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0930-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0930-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0930-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0930-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0930-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e0930-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0930-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0930-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0930-116">Not supported.</span></span>|
|<span data-ttu-id="e0930-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0930-117">Application</span></span>|<span data-ttu-id="e0930-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0930-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0930-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0930-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceSettingStateSummaries
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="e0930-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0930-120">Request headers</span></span>
|<span data-ttu-id="e0930-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0930-121">Header</span></span>|<span data-ttu-id="e0930-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e0930-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0930-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0930-123">Authorization</span></span>|<span data-ttu-id="e0930-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e0930-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0930-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e0930-125">Accept</span></span>|<span data-ttu-id="e0930-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0930-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0930-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e0930-127">Request body</span></span>
<span data-ttu-id="e0930-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e0930-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0930-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0930-129">Response</span></span>
<span data-ttu-id="e0930-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e0930-130">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0930-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e0930-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0930-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0930-132">Request</span></span>
<span data-ttu-id="e0930-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0930-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="e0930-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0930-134">Response</span></span>
<span data-ttu-id="e0930-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e0930-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 486

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
      "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
      "settingName": "Setting Name value",
      "instancePath": "Instance Path value",
      "unknownDeviceCount": 2,
      "notApplicableDeviceCount": 8,
      "compliantDeviceCount": 4,
      "remediatedDeviceCount": 5,
      "nonCompliantDeviceCount": 7,
      "errorDeviceCount": 0,
      "conflictDeviceCount": 3
    }
  ]
}
```





