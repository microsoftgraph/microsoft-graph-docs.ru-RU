---
title: Get managedDeviceMobileAppConfigurationUserSummary
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationUserSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f95a0a2e9b471afcdea3ba7a8554c1ebad1ee17b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824229"
---
# <a name="get-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="621ea-103">Get managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="621ea-103">Get managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="621ea-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="621ea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="621ea-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="621ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="621ea-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="621ea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="621ea-107">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="621ea-107">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="621ea-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="621ea-108">Prerequisites</span></span>
<span data-ttu-id="621ea-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="621ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="621ea-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="621ea-111">Permission type</span></span>|<span data-ttu-id="621ea-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="621ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="621ea-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="621ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="621ea-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="621ea-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="621ea-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="621ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="621ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="621ea-116">Not supported.</span></span>|
|<span data-ttu-id="621ea-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="621ea-117">Application</span></span>|<span data-ttu-id="621ea-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="621ea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="621ea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="621ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="621ea-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="621ea-120">Optional query parameters</span></span>
<span data-ttu-id="621ea-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="621ea-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="621ea-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="621ea-122">Request headers</span></span>
|<span data-ttu-id="621ea-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="621ea-123">Header</span></span>|<span data-ttu-id="621ea-124">Значение</span><span class="sxs-lookup"><span data-stu-id="621ea-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="621ea-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="621ea-125">Authorization</span></span>|<span data-ttu-id="621ea-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="621ea-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="621ea-127">Accept</span><span class="sxs-lookup"><span data-stu-id="621ea-127">Accept</span></span>|<span data-ttu-id="621ea-128">application/json</span><span class="sxs-lookup"><span data-stu-id="621ea-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="621ea-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="621ea-129">Request body</span></span>
<span data-ttu-id="621ea-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="621ea-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="621ea-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="621ea-131">Response</span></span>
<span data-ttu-id="621ea-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="621ea-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="621ea-133">Пример</span><span class="sxs-lookup"><span data-stu-id="621ea-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="621ea-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="621ea-134">Request</span></span>
<span data-ttu-id="621ea-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="621ea-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

### <a name="response"></a><span data-ttu-id="621ea-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="621ea-136">Response</span></span>
<span data-ttu-id="621ea-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="621ea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
    "id": "7b953742-3742-7b95-4237-957b4237957b",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```





