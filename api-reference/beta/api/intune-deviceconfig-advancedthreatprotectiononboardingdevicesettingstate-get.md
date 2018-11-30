---
title: Получение advancedThreatProtectionOnboardingDeviceSettingState
description: Чтение свойства и связи объекта advancedThreatProtectionOnboardingDeviceSettingState.
ms.openlocfilehash: 431a8a6fa945b71cedaefe5613f301b721e749ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078560"
---
# <a name="get-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="7623b-103">Получение advancedThreatProtectionOnboardingDeviceSettingState</span><span class="sxs-lookup"><span data-stu-id="7623b-103">Get advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="7623b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7623b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7623b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7623b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7623b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7623b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7623b-107">Чтение свойства и связи объекта [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="7623b-107">Read properties and relationships of the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7623b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7623b-108">Prerequisites</span></span>
<span data-ttu-id="7623b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7623b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7623b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7623b-111">Permission type</span></span>|<span data-ttu-id="7623b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7623b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7623b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7623b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7623b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7623b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7623b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7623b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7623b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7623b-116">Not supported.</span></span>|
|<span data-ttu-id="7623b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7623b-117">Application</span></span>|<span data-ttu-id="7623b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7623b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7623b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7623b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7623b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7623b-120">Optional query parameters</span></span>
<span data-ttu-id="7623b-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7623b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7623b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7623b-122">Request headers</span></span>
|<span data-ttu-id="7623b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7623b-123">Header</span></span>|<span data-ttu-id="7623b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7623b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7623b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7623b-125">Authorization</span></span>|<span data-ttu-id="7623b-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7623b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7623b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7623b-127">Accept</span></span>|<span data-ttu-id="7623b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7623b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7623b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7623b-129">Request body</span></span>
<span data-ttu-id="7623b-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7623b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7623b-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7623b-131">Response</span></span>
<span data-ttu-id="7623b-132">Успешно завершена, этот метод возвращает `200 OK` объект [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7623b-132">If successful, this method returns a `200 OK` response code and [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7623b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7623b-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="7623b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7623b-134">Request</span></span>
<span data-ttu-id="7623b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7623b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="7623b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7623b-136">Response</span></span>
<span data-ttu-id="7623b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7623b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 669

{
  "value": {
    "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
    "id": "63593fc6-3fc6-6359-c63f-5963c63f5963",
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





