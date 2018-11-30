---
title: Перечисление объектов settingStateDeviceSummary
description: Список свойств и связей объектов settingStateDeviceSummary.
ms.openlocfilehash: 390af97482f0499923cad7850801eb2181de47ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028274"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="1b001-103">Перечисление объектов settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="1b001-103">List settingStateDeviceSummaries</span></span>

> <span data-ttu-id="1b001-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1b001-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b001-105">Список свойств и связей объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="1b001-105">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1b001-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1b001-106">Prerequisites</span></span>
<span data-ttu-id="1b001-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b001-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b001-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b001-109">Permission type</span></span>|<span data-ttu-id="1b001-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b001-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b001-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b001-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1b001-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b001-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1b001-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b001-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b001-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b001-114">Not supported.</span></span>|
|<span data-ttu-id="1b001-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b001-115">Application</span></span>|<span data-ttu-id="1b001-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b001-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b001-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b001-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="1b001-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b001-118">Request headers</span></span>
|<span data-ttu-id="1b001-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b001-119">Header</span></span>|<span data-ttu-id="1b001-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1b001-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b001-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b001-121">Authorization</span></span>|<span data-ttu-id="1b001-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1b001-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b001-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1b001-123">Accept</span></span>|<span data-ttu-id="1b001-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1b001-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b001-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b001-125">Request body</span></span>
<span data-ttu-id="1b001-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1b001-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b001-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b001-127">Response</span></span>
<span data-ttu-id="1b001-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b001-128">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b001-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1b001-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="1b001-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b001-130">Request</span></span>
<span data-ttu-id="1b001-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b001-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="1b001-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b001-132">Response</span></span>
<span data-ttu-id="1b001-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1b001-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



