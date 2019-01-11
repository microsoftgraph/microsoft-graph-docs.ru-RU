---
title: Get managedDeviceMobileAppConfigurationUserStatus
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: da13ebadbf98a130e5b12cb2e76f3fd9c61fde27
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824054"
---
# <a name="get-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="68465-103">Get managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="68465-103">Get managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="68465-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="68465-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68465-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68465-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68465-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="68465-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68465-107">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="68465-107">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68465-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="68465-108">Prerequisites</span></span>
<span data-ttu-id="68465-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68465-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68465-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68465-111">Permission type</span></span>|<span data-ttu-id="68465-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68465-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68465-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68465-113">Delegated (work or school account)</span></span>|<span data-ttu-id="68465-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="68465-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="68465-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68465-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68465-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68465-116">Not supported.</span></span>|
|<span data-ttu-id="68465-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68465-117">Application</span></span>|<span data-ttu-id="68465-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68465-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68465-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68465-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68465-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="68465-120">Optional query parameters</span></span>
<span data-ttu-id="68465-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="68465-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="68465-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68465-122">Request headers</span></span>
|<span data-ttu-id="68465-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68465-123">Header</span></span>|<span data-ttu-id="68465-124">Значение</span><span class="sxs-lookup"><span data-stu-id="68465-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68465-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="68465-125">Authorization</span></span>|<span data-ttu-id="68465-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="68465-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68465-127">Accept</span><span class="sxs-lookup"><span data-stu-id="68465-127">Accept</span></span>|<span data-ttu-id="68465-128">application/json</span><span class="sxs-lookup"><span data-stu-id="68465-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68465-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="68465-129">Request body</span></span>
<span data-ttu-id="68465-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68465-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68465-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="68465-131">Response</span></span>
<span data-ttu-id="68465-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="68465-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68465-133">Пример</span><span class="sxs-lookup"><span data-stu-id="68465-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="68465-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="68465-134">Request</span></span>
<span data-ttu-id="68465-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68465-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="68465-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="68465-136">Response</span></span>
<span data-ttu-id="68465-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="68465-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 388

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
    "id": "44960944-0944-4496-4409-964444099644",
    "userDisplayName": "User Display Name value",
    "devicesCount": 12,
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```





