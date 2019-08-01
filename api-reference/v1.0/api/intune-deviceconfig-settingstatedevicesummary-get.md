---
title: Get settingStateDeviceSummary
description: Чтение свойств и связей объекта settingStateDeviceSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e703e1744089f20c53c99f303d10618b3f4021af
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017058"
---
# <a name="get-settingstatedevicesummary"></a><span data-ttu-id="1bd83-103">Get settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="1bd83-103">Get settingStateDeviceSummary</span></span>

> <span data-ttu-id="1bd83-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1bd83-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bd83-105">Чтение свойств и связей объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="1bd83-105">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bd83-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1bd83-106">Prerequisites</span></span>
<span data-ttu-id="1bd83-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bd83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bd83-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bd83-109">Permission type</span></span>|<span data-ttu-id="1bd83-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bd83-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bd83-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bd83-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1bd83-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bd83-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1bd83-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bd83-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bd83-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bd83-114">Not supported.</span></span>|
|<span data-ttu-id="1bd83-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1bd83-115">Application</span></span>|<span data-ttu-id="1bd83-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bd83-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bd83-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bd83-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1bd83-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1bd83-118">Optional query parameters</span></span>
<span data-ttu-id="1bd83-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1bd83-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1bd83-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bd83-120">Request headers</span></span>
|<span data-ttu-id="1bd83-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1bd83-121">Header</span></span>|<span data-ttu-id="1bd83-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1bd83-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bd83-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1bd83-123">Authorization</span></span>|<span data-ttu-id="1bd83-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bd83-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bd83-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1bd83-125">Accept</span></span>|<span data-ttu-id="1bd83-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1bd83-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bd83-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1bd83-127">Request body</span></span>
<span data-ttu-id="1bd83-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1bd83-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bd83-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1bd83-129">Response</span></span>
<span data-ttu-id="1bd83-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1bd83-130">If successful, this method returns a `200 OK` response code and [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bd83-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1bd83-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bd83-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bd83-132">Request</span></span>
<span data-ttu-id="1bd83-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bd83-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="1bd83-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bd83-134">Response</span></span>
<span data-ttu-id="1bd83-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1bd83-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": {
    "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
    "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
    "settingName": "Setting Name value",
    "instancePath": "Instance Path value",
    "unknownDeviceCount": 2,
    "notApplicableDeviceCount": 8,
    "compliantDeviceCount": 4,
    "remediatedDeviceCount": 5,
    "nonCompliantDeviceCount": 7,
    "errorDeviceCount": 0,
    "conflictDeviceCount": 3
  }
}
```



