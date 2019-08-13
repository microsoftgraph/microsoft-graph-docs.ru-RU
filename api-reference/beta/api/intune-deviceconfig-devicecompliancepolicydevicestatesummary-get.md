---
title: Get deviceCompliancePolicyDeviceStateSummary
description: Чтение свойств и связей объекта deviceCompliancePolicyDeviceStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aab30607d02a9196524d947bf22cdec9da198e95
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346228"
---
# <a name="get-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="25c93-103">Get deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="25c93-103">Get deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="25c93-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25c93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25c93-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25c93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25c93-106">Чтение свойств и связей объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="25c93-106">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25c93-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="25c93-107">Prerequisites</span></span>
<span data-ttu-id="25c93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25c93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25c93-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25c93-110">Permission type</span></span>|<span data-ttu-id="25c93-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="25c93-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25c93-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25c93-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25c93-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="25c93-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="25c93-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25c93-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25c93-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25c93-115">Not supported.</span></span>|
|<span data-ttu-id="25c93-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25c93-116">Application</span></span>|<span data-ttu-id="25c93-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="25c93-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25c93-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25c93-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="25c93-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="25c93-119">Optional query parameters</span></span>
<span data-ttu-id="25c93-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="25c93-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25c93-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25c93-121">Request headers</span></span>
|<span data-ttu-id="25c93-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25c93-122">Header</span></span>|<span data-ttu-id="25c93-123">Значение</span><span class="sxs-lookup"><span data-stu-id="25c93-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25c93-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25c93-124">Authorization</span></span>|<span data-ttu-id="25c93-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25c93-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25c93-126">Accept</span><span class="sxs-lookup"><span data-stu-id="25c93-126">Accept</span></span>|<span data-ttu-id="25c93-127">application/json</span><span class="sxs-lookup"><span data-stu-id="25c93-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25c93-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="25c93-128">Request body</span></span>
<span data-ttu-id="25c93-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="25c93-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25c93-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="25c93-130">Response</span></span>
<span data-ttu-id="25c93-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="25c93-131">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25c93-132">Пример</span><span class="sxs-lookup"><span data-stu-id="25c93-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="25c93-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="25c93-133">Request</span></span>
<span data-ttu-id="25c93-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25c93-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

### <a name="response"></a><span data-ttu-id="25c93-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="25c93-135">Response</span></span>
<span data-ttu-id="25c93-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25c93-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
    "inGracePeriodCount": 2,
    "configManagerCount": 2,
    "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
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






