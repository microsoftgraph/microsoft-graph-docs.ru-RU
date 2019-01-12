---
title: Список advancedThreatProtectionOnboardingDeviceSettingStates
description: Свойства списка и связей объектов advancedThreatProtectionOnboardingDeviceSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 018ab29513b9a44d4068cc63b67b6432cc03656d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983536"
---
# <a name="list-advancedthreatprotectiononboardingdevicesettingstates"></a><span data-ttu-id="37e0f-103">Список advancedThreatProtectionOnboardingDeviceSettingStates</span><span class="sxs-lookup"><span data-stu-id="37e0f-103">List advancedThreatProtectionOnboardingDeviceSettingStates</span></span>

> <span data-ttu-id="37e0f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="37e0f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37e0f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37e0f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37e0f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="37e0f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37e0f-107">Свойства списка и связей объектов [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) .</span><span class="sxs-lookup"><span data-stu-id="37e0f-107">List properties and relationships of the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="37e0f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="37e0f-108">Prerequisites</span></span>
<span data-ttu-id="37e0f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37e0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37e0f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37e0f-111">Permission type</span></span>|<span data-ttu-id="37e0f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="37e0f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37e0f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37e0f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37e0f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="37e0f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="37e0f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37e0f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37e0f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37e0f-116">Not supported.</span></span>|
|<span data-ttu-id="37e0f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37e0f-117">Application</span></span>|<span data-ttu-id="37e0f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37e0f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37e0f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37e0f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="37e0f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37e0f-120">Request headers</span></span>
|<span data-ttu-id="37e0f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37e0f-121">Header</span></span>|<span data-ttu-id="37e0f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="37e0f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37e0f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37e0f-123">Authorization</span></span>|<span data-ttu-id="37e0f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="37e0f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37e0f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="37e0f-125">Accept</span></span>|<span data-ttu-id="37e0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37e0f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37e0f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="37e0f-127">Request body</span></span>
<span data-ttu-id="37e0f-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37e0f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37e0f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="37e0f-129">Response</span></span>
<span data-ttu-id="37e0f-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="37e0f-130">If successful, this method returns a `200 OK` response code and a collection of [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37e0f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="37e0f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="37e0f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="37e0f-132">Request</span></span>
<span data-ttu-id="37e0f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37e0f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

### <a name="response"></a><span data-ttu-id="37e0f-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="37e0f-134">Response</span></span>
<span data-ttu-id="37e0f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="37e0f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 711

{
  "value": [
    {
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
  ]
}
```





