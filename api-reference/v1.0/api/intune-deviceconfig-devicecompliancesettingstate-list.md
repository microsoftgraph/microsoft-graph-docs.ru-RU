---
title: List deviceComplianceSettingStates
description: Перечисление свойств и связей объектов deviceComplianceSettingState.
author: tfitzmac
ms.openlocfilehash: a282b306478cc1ff2ecbe7f86a063183eee0edd8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313799"
---
# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="70210-103">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="70210-103">List deviceComplianceSettingStates</span></span>

> <span data-ttu-id="70210-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="70210-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70210-105">Перечисление свойств и связей объектов [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="70210-105">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="70210-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="70210-106">Prerequisites</span></span>
<span data-ttu-id="70210-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70210-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70210-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70210-109">Permission type</span></span>|<span data-ttu-id="70210-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="70210-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70210-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70210-111">Delegated (work or school account)</span></span>|<span data-ttu-id="70210-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="70210-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="70210-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70210-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70210-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70210-114">Not supported.</span></span>|
|<span data-ttu-id="70210-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70210-115">Application</span></span>|<span data-ttu-id="70210-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70210-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70210-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70210-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="70210-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70210-118">Request headers</span></span>
|<span data-ttu-id="70210-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70210-119">Header</span></span>|<span data-ttu-id="70210-120">Значение</span><span class="sxs-lookup"><span data-stu-id="70210-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70210-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70210-121">Authorization</span></span>|<span data-ttu-id="70210-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="70210-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70210-123">Accept</span><span class="sxs-lookup"><span data-stu-id="70210-123">Accept</span></span>|<span data-ttu-id="70210-124">application/json</span><span class="sxs-lookup"><span data-stu-id="70210-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70210-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70210-125">Request body</span></span>
<span data-ttu-id="70210-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70210-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70210-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="70210-127">Response</span></span>
<span data-ttu-id="70210-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="70210-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70210-129">Пример</span><span class="sxs-lookup"><span data-stu-id="70210-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="70210-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="70210-130">Request</span></span>
<span data-ttu-id="70210-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70210-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="70210-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="70210-132">Response</span></span>
<span data-ttu-id="70210-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="70210-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
      "id": "9905f955-f955-9905-55f9-059955f90599",
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



