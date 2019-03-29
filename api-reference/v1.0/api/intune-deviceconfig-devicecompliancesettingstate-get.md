---
title: Get deviceComplianceSettingState
description: Чтение свойств и связей объекта deviceComplianceSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c804f03218ad7a0cb5385bb4ca73dc12d83460f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980364"
---
# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="102c1-103">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="102c1-103">Get deviceComplianceSettingState</span></span>

> <span data-ttu-id="102c1-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="102c1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="102c1-105">Чтение свойств и связей объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="102c1-105">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="102c1-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="102c1-106">Prerequisites</span></span>
<span data-ttu-id="102c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="102c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="102c1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="102c1-109">Permission type</span></span>|<span data-ttu-id="102c1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="102c1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="102c1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="102c1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="102c1-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="102c1-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="102c1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="102c1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="102c1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="102c1-114">Not supported.</span></span>|
|<span data-ttu-id="102c1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="102c1-115">Application</span></span>|<span data-ttu-id="102c1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="102c1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="102c1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="102c1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="102c1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="102c1-118">Optional query parameters</span></span>
<span data-ttu-id="102c1-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="102c1-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="102c1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="102c1-120">Request headers</span></span>
|<span data-ttu-id="102c1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="102c1-121">Header</span></span>|<span data-ttu-id="102c1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="102c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="102c1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="102c1-123">Authorization</span></span>|<span data-ttu-id="102c1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="102c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="102c1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="102c1-125">Accept</span></span>|<span data-ttu-id="102c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="102c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="102c1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="102c1-127">Request body</span></span>
<span data-ttu-id="102c1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="102c1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="102c1-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="102c1-129">Response</span></span>
<span data-ttu-id="102c1-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="102c1-130">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="102c1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="102c1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="102c1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="102c1-132">Request</span></span>
<span data-ttu-id="102c1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="102c1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="102c1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="102c1-134">Response</span></span>
<span data-ttu-id="102c1-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="102c1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 611

{
  "value": {
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
}
```



