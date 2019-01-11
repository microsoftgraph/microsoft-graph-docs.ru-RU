---
title: Get managedDeviceMobileAppConfigurationUserSummary
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationUserSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 44f47f55bb87af08d1cbd6f718e4be61fd56d145
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845495"
---
# <a name="get-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="4cef2-103">Get managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="4cef2-103">Get managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="4cef2-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4cef2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4cef2-105">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="4cef2-105">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4cef2-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4cef2-106">Prerequisites</span></span>
<span data-ttu-id="4cef2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cef2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cef2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cef2-109">Permission type</span></span>|<span data-ttu-id="4cef2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cef2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cef2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cef2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4cef2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4cef2-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4cef2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cef2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cef2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cef2-114">Not supported.</span></span>|
|<span data-ttu-id="4cef2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cef2-115">Application</span></span>|<span data-ttu-id="4cef2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cef2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cef2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cef2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4cef2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4cef2-118">Optional query parameters</span></span>
<span data-ttu-id="4cef2-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4cef2-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4cef2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4cef2-120">Request headers</span></span>
|<span data-ttu-id="4cef2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4cef2-121">Header</span></span>|<span data-ttu-id="4cef2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4cef2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cef2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cef2-123">Authorization</span></span>|<span data-ttu-id="4cef2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4cef2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cef2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4cef2-125">Accept</span></span>|<span data-ttu-id="4cef2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4cef2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cef2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4cef2-127">Request body</span></span>
<span data-ttu-id="4cef2-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4cef2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cef2-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4cef2-129">Response</span></span>
<span data-ttu-id="4cef2-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4cef2-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cef2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4cef2-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4cef2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cef2-132">Request</span></span>
<span data-ttu-id="4cef2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4cef2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

### <a name="response"></a><span data-ttu-id="4cef2-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="4cef2-134">Response</span></span>
<span data-ttu-id="4cef2-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4cef2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 383

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
    "id": "7b953742-3742-7b95-4237-957b4237957b",
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



