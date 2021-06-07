---
title: Get deviceComplianceSettingState
description: Чтение свойств и связей объекта deviceComplianceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e48211ebbba3ea9439b12abb9e9144aa75b36d37
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757124"
---
# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="c8c51-103">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="c8c51-103">Get deviceComplianceSettingState</span></span>

<span data-ttu-id="c8c51-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8c51-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8c51-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8c51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8c51-106">Чтение свойств и связей объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="c8c51-106">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8c51-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c8c51-107">Prerequisites</span></span>
<span data-ttu-id="c8c51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8c51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8c51-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8c51-110">Permission type</span></span>|<span data-ttu-id="c8c51-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8c51-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8c51-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8c51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8c51-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8c51-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8c51-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8c51-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8c51-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8c51-115">Not supported.</span></span>|
|<span data-ttu-id="c8c51-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c8c51-116">Application</span></span>|<span data-ttu-id="c8c51-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8c51-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8c51-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8c51-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8c51-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c8c51-119">Optional query parameters</span></span>
<span data-ttu-id="c8c51-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c8c51-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8c51-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8c51-121">Request headers</span></span>
|<span data-ttu-id="c8c51-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8c51-122">Header</span></span>|<span data-ttu-id="c8c51-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c8c51-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8c51-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8c51-124">Authorization</span></span>|<span data-ttu-id="c8c51-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8c51-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8c51-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c8c51-126">Accept</span></span>|<span data-ttu-id="c8c51-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c8c51-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8c51-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8c51-128">Request body</span></span>
<span data-ttu-id="c8c51-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8c51-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8c51-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8c51-130">Response</span></span>
<span data-ttu-id="c8c51-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c8c51-131">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8c51-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c8c51-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8c51-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8c51-133">Request</span></span>
<span data-ttu-id="c8c51-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8c51-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="c8c51-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8c51-135">Response</span></span>
<span data-ttu-id="c8c51-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8c51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




