---
title: Перечисление объектов deviceCompliancePolicySettingStateSummary
description: Список свойств и связей объектов deviceCompliancePolicySettingStateSummary.
ms.openlocfilehash: 50326e17db43d4f6249c06c7a8e4552a7a826821
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025889"
---
# <a name="list-devicecompliancepolicysettingstatesummaries"></a><span data-ttu-id="214a3-103">Перечисление объектов deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="214a3-103">List deviceCompliancePolicySettingStateSummaries</span></span>

> <span data-ttu-id="214a3-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="214a3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="214a3-105">Список свойств и связей объектов [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="214a3-105">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="214a3-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="214a3-106">Prerequisites</span></span>
<span data-ttu-id="214a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="214a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="214a3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="214a3-109">Permission type</span></span>|<span data-ttu-id="214a3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="214a3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="214a3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="214a3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="214a3-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="214a3-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="214a3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="214a3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="214a3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="214a3-114">Not supported.</span></span>|
|<span data-ttu-id="214a3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="214a3-115">Application</span></span>|<span data-ttu-id="214a3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="214a3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="214a3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="214a3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="214a3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="214a3-118">Request headers</span></span>
|<span data-ttu-id="214a3-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="214a3-119">Header</span></span>|<span data-ttu-id="214a3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="214a3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="214a3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="214a3-121">Authorization</span></span>|<span data-ttu-id="214a3-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="214a3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="214a3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="214a3-123">Accept</span></span>|<span data-ttu-id="214a3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="214a3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="214a3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="214a3-125">Request body</span></span>
<span data-ttu-id="214a3-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="214a3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="214a3-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="214a3-127">Response</span></span>
<span data-ttu-id="214a3-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="214a3-128">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="214a3-129">Пример</span><span class="sxs-lookup"><span data-stu-id="214a3-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="214a3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="214a3-130">Request</span></span>
<span data-ttu-id="214a3-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="214a3-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="214a3-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="214a3-132">Response</span></span>
<span data-ttu-id="214a3-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="214a3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 521

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
      "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "platformType": "iOS",
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



