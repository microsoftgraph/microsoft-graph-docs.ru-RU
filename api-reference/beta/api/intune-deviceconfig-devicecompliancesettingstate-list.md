---
title: List deviceComplianceSettingStates
description: Перечисление свойств и связей объектов deviceComplianceSettingState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 550f08632a75770230068b2d8245e38e64b534df
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402050"
---
# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="d1675-103">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="d1675-103">List deviceComplianceSettingStates</span></span>

> <span data-ttu-id="d1675-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d1675-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d1675-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1675-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1675-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1675-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1675-107">Перечисление свойств и связей объектов [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="d1675-107">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1675-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d1675-108">Prerequisites</span></span>
<span data-ttu-id="d1675-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d1675-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d1675-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1675-111">Permission type</span></span>|<span data-ttu-id="d1675-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1675-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1675-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1675-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1675-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1675-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d1675-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1675-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1675-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1675-116">Not supported.</span></span>|
|<span data-ttu-id="d1675-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1675-117">Application</span></span>|<span data-ttu-id="d1675-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1675-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1675-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1675-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="d1675-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1675-120">Request headers</span></span>
|<span data-ttu-id="d1675-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1675-121">Header</span></span>|<span data-ttu-id="d1675-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d1675-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1675-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1675-123">Authorization</span></span>|<span data-ttu-id="d1675-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d1675-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1675-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d1675-125">Accept</span></span>|<span data-ttu-id="d1675-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1675-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1675-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1675-127">Request body</span></span>
<span data-ttu-id="d1675-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1675-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1675-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1675-129">Response</span></span>
<span data-ttu-id="d1675-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d1675-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1675-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d1675-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1675-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1675-132">Request</span></span>
<span data-ttu-id="d1675-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1675-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="d1675-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1675-134">Response</span></span>
<span data-ttu-id="d1675-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d1675-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 687

{
  "value": [
    {
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
  ]
}
```




