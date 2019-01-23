---
title: Get deviceComplianceSettingState
description: Чтение свойств и связей объекта deviceComplianceSettingState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: acbd148b60fffa11144d457fb4dee20082cd6145
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418304"
---
# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="c5c91-103">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="c5c91-103">Get deviceComplianceSettingState</span></span>

> <span data-ttu-id="c5c91-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5c91-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c5c91-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5c91-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5c91-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5c91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5c91-107">Чтение свойств и связей объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="c5c91-107">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5c91-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c5c91-108">Prerequisites</span></span>
<span data-ttu-id="c5c91-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5c91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c5c91-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5c91-111">Permission type</span></span>|<span data-ttu-id="c5c91-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5c91-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5c91-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5c91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5c91-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5c91-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c5c91-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5c91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5c91-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5c91-116">Not supported.</span></span>|
|<span data-ttu-id="c5c91-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5c91-117">Application</span></span>|<span data-ttu-id="c5c91-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5c91-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5c91-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5c91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5c91-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c5c91-120">Optional query parameters</span></span>
<span data-ttu-id="c5c91-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c5c91-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5c91-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5c91-122">Request headers</span></span>
|<span data-ttu-id="c5c91-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5c91-123">Header</span></span>|<span data-ttu-id="c5c91-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c5c91-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5c91-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5c91-125">Authorization</span></span>|<span data-ttu-id="c5c91-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c5c91-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5c91-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c5c91-127">Accept</span></span>|<span data-ttu-id="c5c91-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c5c91-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5c91-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5c91-129">Request body</span></span>
<span data-ttu-id="c5c91-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5c91-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5c91-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5c91-131">Response</span></span>
<span data-ttu-id="c5c91-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c5c91-132">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5c91-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c5c91-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5c91-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5c91-134">Request</span></span>
<span data-ttu-id="c5c91-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5c91-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="c5c91-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5c91-136">Response</span></span>
<span data-ttu-id="c5c91-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c5c91-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




