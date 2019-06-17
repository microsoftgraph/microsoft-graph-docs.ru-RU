---
title: Get deviceComplianceSettingState
description: Чтение свойств и связей объекта deviceComplianceSettingState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: df1aa0a1c621f38a942875703b73bba70d045a52
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968191"
---
# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="70173-103">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="70173-103">Get deviceComplianceSettingState</span></span>

> <span data-ttu-id="70173-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70173-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70173-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70173-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70173-106">Чтение свойств и связей объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="70173-106">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70173-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="70173-107">Prerequisites</span></span>
<span data-ttu-id="70173-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70173-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70173-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70173-110">Permission type</span></span>|<span data-ttu-id="70173-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="70173-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70173-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70173-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70173-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="70173-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="70173-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70173-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70173-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70173-115">Not supported.</span></span>|
|<span data-ttu-id="70173-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70173-116">Application</span></span>|<span data-ttu-id="70173-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70173-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70173-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70173-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70173-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="70173-119">Optional query parameters</span></span>
<span data-ttu-id="70173-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="70173-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70173-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70173-121">Request headers</span></span>
|<span data-ttu-id="70173-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70173-122">Header</span></span>|<span data-ttu-id="70173-123">Значение</span><span class="sxs-lookup"><span data-stu-id="70173-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70173-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70173-124">Authorization</span></span>|<span data-ttu-id="70173-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70173-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70173-126">Accept</span><span class="sxs-lookup"><span data-stu-id="70173-126">Accept</span></span>|<span data-ttu-id="70173-127">application/json</span><span class="sxs-lookup"><span data-stu-id="70173-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70173-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="70173-128">Request body</span></span>
<span data-ttu-id="70173-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70173-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70173-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="70173-130">Response</span></span>
<span data-ttu-id="70173-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="70173-131">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70173-132">Пример</span><span class="sxs-lookup"><span data-stu-id="70173-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="70173-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="70173-133">Request</span></span>
<span data-ttu-id="70173-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70173-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="70173-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="70173-135">Response</span></span>
<span data-ttu-id="70173-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70173-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





