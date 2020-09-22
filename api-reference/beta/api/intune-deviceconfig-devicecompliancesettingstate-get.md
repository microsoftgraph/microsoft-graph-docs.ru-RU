---
title: Get deviceComplianceSettingState
description: Чтение свойств и связей объекта deviceComplianceSettingState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 00dcde4f66032564e3f762baa53f6bae04f33c99
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011678"
---
# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="292d1-103">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="292d1-103">Get deviceComplianceSettingState</span></span>

<span data-ttu-id="292d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="292d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="292d1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="292d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="292d1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="292d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="292d1-107">Чтение свойств и связей объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="292d1-107">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="292d1-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="292d1-108">Prerequisites</span></span>
<span data-ttu-id="292d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="292d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="292d1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="292d1-111">Permission type</span></span>|<span data-ttu-id="292d1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="292d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="292d1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="292d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="292d1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="292d1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="292d1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="292d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="292d1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="292d1-116">Not supported.</span></span>|
|<span data-ttu-id="292d1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="292d1-117">Application</span></span>|<span data-ttu-id="292d1-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="292d1-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="292d1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="292d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="292d1-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="292d1-120">Optional query parameters</span></span>
<span data-ttu-id="292d1-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="292d1-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="292d1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="292d1-122">Request headers</span></span>
|<span data-ttu-id="292d1-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="292d1-123">Header</span></span>|<span data-ttu-id="292d1-124">Значение</span><span class="sxs-lookup"><span data-stu-id="292d1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="292d1-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="292d1-125">Authorization</span></span>|<span data-ttu-id="292d1-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="292d1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="292d1-127">Accept</span><span class="sxs-lookup"><span data-stu-id="292d1-127">Accept</span></span>|<span data-ttu-id="292d1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="292d1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="292d1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="292d1-129">Request body</span></span>
<span data-ttu-id="292d1-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="292d1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="292d1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="292d1-131">Response</span></span>
<span data-ttu-id="292d1-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="292d1-132">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="292d1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="292d1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="292d1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="292d1-134">Request</span></span>
<span data-ttu-id="292d1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="292d1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="292d1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="292d1-136">Response</span></span>
<span data-ttu-id="292d1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="292d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






