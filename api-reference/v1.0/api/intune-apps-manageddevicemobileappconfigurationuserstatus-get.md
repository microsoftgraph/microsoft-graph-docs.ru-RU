---
title: Get managedDeviceMobileAppConfigurationUserStatus
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fe2ece00f7f6984446a2df398a67bf0855cc261b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013978"
---
# <a name="get-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="ac3b8-103">Get managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ac3b8-103">Get managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="ac3b8-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ac3b8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac3b8-105">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="ac3b8-105">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac3b8-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ac3b8-106">Prerequisites</span></span>
<span data-ttu-id="ac3b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac3b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac3b8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac3b8-109">Permission type</span></span>|<span data-ttu-id="ac3b8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac3b8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac3b8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac3b8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ac3b8-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ac3b8-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ac3b8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac3b8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac3b8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac3b8-114">Not supported.</span></span>|
|<span data-ttu-id="ac3b8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac3b8-115">Application</span></span>|<span data-ttu-id="ac3b8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac3b8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac3b8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac3b8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac3b8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ac3b8-118">Optional query parameters</span></span>
<span data-ttu-id="ac3b8-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ac3b8-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac3b8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac3b8-120">Request headers</span></span>
|<span data-ttu-id="ac3b8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ac3b8-121">Header</span></span>|<span data-ttu-id="ac3b8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ac3b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac3b8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac3b8-123">Authorization</span></span>|<span data-ttu-id="ac3b8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac3b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac3b8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ac3b8-125">Accept</span></span>|<span data-ttu-id="ac3b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac3b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac3b8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ac3b8-127">Request body</span></span>
<span data-ttu-id="ac3b8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ac3b8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac3b8-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ac3b8-129">Response</span></span>
<span data-ttu-id="ac3b8-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ac3b8-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac3b8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ac3b8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac3b8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac3b8-132">Request</span></span>
<span data-ttu-id="ac3b8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac3b8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="ac3b8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac3b8-134">Response</span></span>
<span data-ttu-id="ac3b8-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ac3b8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



