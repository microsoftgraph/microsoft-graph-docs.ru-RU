---
title: Получение объекта managedDeviceMobileAppConfigurationDeviceSummary
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationDeviceSummary.
author: tfitzmac
ms.openlocfilehash: 12a9f069f4a34bc0f38c85c0f0a4a1566237e5e1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309487"
---
# <a name="get-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="1d002-103">Получение объекта managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="1d002-103">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="1d002-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1d002-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d002-105">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="1d002-105">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d002-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1d002-106">Prerequisites</span></span>
<span data-ttu-id="1d002-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d002-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d002-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d002-109">Permission type</span></span>|<span data-ttu-id="1d002-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d002-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d002-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d002-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1d002-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d002-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1d002-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d002-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d002-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d002-114">Not supported.</span></span>|
|<span data-ttu-id="1d002-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d002-115">Application</span></span>|<span data-ttu-id="1d002-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d002-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d002-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d002-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1d002-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1d002-118">Optional query parameters</span></span>
<span data-ttu-id="1d002-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1d002-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1d002-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d002-120">Request headers</span></span>
|<span data-ttu-id="1d002-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d002-121">Header</span></span>|<span data-ttu-id="1d002-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1d002-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d002-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d002-123">Authorization</span></span>|<span data-ttu-id="1d002-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1d002-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d002-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d002-125">Accept</span></span>|<span data-ttu-id="1d002-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d002-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d002-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d002-127">Request body</span></span>
<span data-ttu-id="1d002-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d002-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d002-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d002-129">Response</span></span>
<span data-ttu-id="1d002-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1d002-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d002-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1d002-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d002-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d002-132">Request</span></span>
<span data-ttu-id="1d002-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d002-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

### <a name="response"></a><span data-ttu-id="1d002-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d002-134">Response</span></span>
<span data-ttu-id="1d002-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1d002-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
    "id": "9997c455-c455-9997-55c4-979955c49799",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```



