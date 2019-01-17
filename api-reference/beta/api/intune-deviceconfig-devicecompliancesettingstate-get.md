---
title: Get deviceComplianceSettingState
description: Чтение свойств и связей объекта deviceComplianceSettingState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7cf582975883ef3027443719ea00596305093eac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916791"
---
# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="4ee72-103">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="4ee72-103">Get deviceComplianceSettingState</span></span>

> <span data-ttu-id="4ee72-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4ee72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ee72-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ee72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ee72-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4ee72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ee72-107">Чтение свойств и связей объекта [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span><span class="sxs-lookup"><span data-stu-id="4ee72-107">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ee72-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4ee72-108">Prerequisites</span></span>
<span data-ttu-id="4ee72-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ee72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ee72-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ee72-111">Permission type</span></span>|<span data-ttu-id="4ee72-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ee72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ee72-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ee72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4ee72-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ee72-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4ee72-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ee72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ee72-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ee72-116">Not supported.</span></span>|
|<span data-ttu-id="4ee72-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ee72-117">Application</span></span>|<span data-ttu-id="4ee72-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ee72-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ee72-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ee72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ee72-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4ee72-120">Optional query parameters</span></span>
<span data-ttu-id="4ee72-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4ee72-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4ee72-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ee72-122">Request headers</span></span>
|<span data-ttu-id="4ee72-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ee72-123">Header</span></span>|<span data-ttu-id="4ee72-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4ee72-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ee72-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ee72-125">Authorization</span></span>|<span data-ttu-id="4ee72-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4ee72-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ee72-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4ee72-127">Accept</span></span>|<span data-ttu-id="4ee72-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4ee72-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ee72-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ee72-129">Request body</span></span>
<span data-ttu-id="4ee72-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ee72-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ee72-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ee72-131">Response</span></span>
<span data-ttu-id="4ee72-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4ee72-132">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ee72-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4ee72-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ee72-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ee72-134">Request</span></span>
<span data-ttu-id="4ee72-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ee72-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="4ee72-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ee72-136">Response</span></span>
<span data-ttu-id="4ee72-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4ee72-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





