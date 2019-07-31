---
title: Get managedDeviceMobileAppConfigurationUserStatus
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationUserStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0c372490ec8f1b2c2390c0d98681245120503731
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961485"
---
# <a name="get-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="e4bb6-103">Get managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="e4bb6-103">Get managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="e4bb6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4bb6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4bb6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4bb6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4bb6-106">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="e4bb6-106">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4bb6-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e4bb6-107">Prerequisites</span></span>
<span data-ttu-id="e4bb6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4bb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4bb6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4bb6-110">Permission type</span></span>|<span data-ttu-id="e4bb6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4bb6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4bb6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4bb6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4bb6-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4bb6-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e4bb6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4bb6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4bb6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4bb6-115">Not supported.</span></span>|
|<span data-ttu-id="e4bb6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4bb6-116">Application</span></span>|<span data-ttu-id="e4bb6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4bb6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4bb6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4bb6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4bb6-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e4bb6-119">Optional query parameters</span></span>
<span data-ttu-id="e4bb6-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e4bb6-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4bb6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4bb6-121">Request headers</span></span>
|<span data-ttu-id="e4bb6-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4bb6-122">Header</span></span>|<span data-ttu-id="e4bb6-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e4bb6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4bb6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4bb6-124">Authorization</span></span>|<span data-ttu-id="e4bb6-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4bb6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4bb6-126">Accept</span><span class="sxs-lookup"><span data-stu-id="e4bb6-126">Accept</span></span>|<span data-ttu-id="e4bb6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e4bb6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4bb6-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4bb6-128">Request body</span></span>
<span data-ttu-id="e4bb6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4bb6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4bb6-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4bb6-130">Response</span></span>
<span data-ttu-id="e4bb6-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e4bb6-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4bb6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e4bb6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4bb6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4bb6-133">Request</span></span>
<span data-ttu-id="e4bb6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4bb6-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="e4bb6-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4bb6-135">Response</span></span>
<span data-ttu-id="e4bb6-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4bb6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





