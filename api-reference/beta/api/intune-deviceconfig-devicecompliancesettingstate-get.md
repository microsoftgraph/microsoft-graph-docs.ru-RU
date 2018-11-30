---
title: Get deviceComplianceSettingState
description: Чтение свойств и связей объекта deviceComplianceSettingState.
ms.openlocfilehash: 4f524b21951e28b404bebdefeb60cbeb63a7682c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075580"
---
# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="75d2a-103">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="75d2a-103">Get deviceComplianceSettingState</span></span>

> <span data-ttu-id="75d2a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="75d2a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75d2a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75d2a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="75d2a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="75d2a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75d2a-107">Чтение свойств и связей объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="75d2a-107">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="75d2a-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="75d2a-108">Prerequisites</span></span>
<span data-ttu-id="75d2a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75d2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75d2a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75d2a-111">Permission type</span></span>|<span data-ttu-id="75d2a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75d2a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75d2a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75d2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75d2a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="75d2a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="75d2a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75d2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75d2a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75d2a-116">Not supported.</span></span>|
|<span data-ttu-id="75d2a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75d2a-117">Application</span></span>|<span data-ttu-id="75d2a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75d2a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75d2a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75d2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75d2a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="75d2a-120">Optional query parameters</span></span>
<span data-ttu-id="75d2a-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="75d2a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="75d2a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75d2a-122">Request headers</span></span>
|<span data-ttu-id="75d2a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75d2a-123">Header</span></span>|<span data-ttu-id="75d2a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="75d2a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75d2a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="75d2a-125">Authorization</span></span>|<span data-ttu-id="75d2a-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="75d2a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75d2a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="75d2a-127">Accept</span></span>|<span data-ttu-id="75d2a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="75d2a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75d2a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75d2a-129">Request body</span></span>
<span data-ttu-id="75d2a-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75d2a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75d2a-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="75d2a-131">Response</span></span>
<span data-ttu-id="75d2a-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="75d2a-132">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75d2a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="75d2a-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="75d2a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="75d2a-134">Request</span></span>
<span data-ttu-id="75d2a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75d2a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="75d2a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="75d2a-136">Response</span></span>
<span data-ttu-id="75d2a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="75d2a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 645

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
    "id": "9905f955-f955-9905-55f9-059955f90599",
    "platformType": "windowsRT",
    "setting": "Setting value",
    "settingName": "Setting Name value",
    "deviceId": "Device Id value",
    "deviceName": "Device Name value",
    "userId": "User Id value",
    "userEmail": "User Email value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value",
    "deviceModel": "Device Model value",
    "state": "notApplicable",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
  }
}
```





