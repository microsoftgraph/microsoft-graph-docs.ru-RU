---
title: Get managedDeviceMobileAppConfigurationUserStatus
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 53ca0f65d4c69e9ba082e6dea002f38053023ee5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471654"
---
# <a name="get-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="6c0b9-103">Get managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="6c0b9-103">Get managedDeviceMobileAppConfigurationUserStatus</span></span>

<span data-ttu-id="6c0b9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c0b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c0b9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c0b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c0b9-106">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="6c0b9-106">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c0b9-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6c0b9-107">Prerequisites</span></span>
<span data-ttu-id="6c0b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c0b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c0b9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c0b9-110">Permission type</span></span>|<span data-ttu-id="6c0b9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c0b9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c0b9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c0b9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c0b9-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c0b9-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6c0b9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c0b9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c0b9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c0b9-115">Not supported.</span></span>|
|<span data-ttu-id="6c0b9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c0b9-116">Application</span></span>|<span data-ttu-id="6c0b9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c0b9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c0b9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c0b9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c0b9-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6c0b9-119">Optional query parameters</span></span>
<span data-ttu-id="6c0b9-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6c0b9-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c0b9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c0b9-121">Request headers</span></span>
|<span data-ttu-id="6c0b9-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c0b9-122">Header</span></span>|<span data-ttu-id="6c0b9-123">Значение</span><span class="sxs-lookup"><span data-stu-id="6c0b9-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c0b9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c0b9-124">Authorization</span></span>|<span data-ttu-id="6c0b9-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c0b9-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c0b9-126">Accept</span><span class="sxs-lookup"><span data-stu-id="6c0b9-126">Accept</span></span>|<span data-ttu-id="6c0b9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6c0b9-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c0b9-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6c0b9-128">Request body</span></span>
<span data-ttu-id="6c0b9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c0b9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c0b9-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c0b9-130">Response</span></span>
<span data-ttu-id="6c0b9-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6c0b9-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c0b9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6c0b9-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c0b9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c0b9-133">Request</span></span>
<span data-ttu-id="6c0b9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c0b9-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="6c0b9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c0b9-135">Response</span></span>
<span data-ttu-id="6c0b9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c0b9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






