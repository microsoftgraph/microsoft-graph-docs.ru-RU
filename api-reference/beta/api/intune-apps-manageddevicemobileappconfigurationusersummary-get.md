---
title: Get managedDeviceMobileAppConfigurationUserSummary
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationUserSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1c496212ab188e3e1131045ef1cf96ab514a8c82
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39936789"
---
# <a name="get-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="b4b80-103">Get managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="b4b80-103">Get managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="b4b80-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4b80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4b80-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4b80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4b80-106">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="b4b80-106">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4b80-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b4b80-107">Prerequisites</span></span>
<span data-ttu-id="b4b80-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4b80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4b80-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4b80-110">Permission type</span></span>|<span data-ttu-id="b4b80-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4b80-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4b80-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4b80-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b4b80-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4b80-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b4b80-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4b80-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4b80-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4b80-115">Not supported.</span></span>|
|<span data-ttu-id="b4b80-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4b80-116">Application</span></span>|<span data-ttu-id="b4b80-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4b80-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4b80-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4b80-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4b80-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b4b80-119">Optional query parameters</span></span>
<span data-ttu-id="b4b80-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b4b80-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4b80-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4b80-121">Request headers</span></span>
|<span data-ttu-id="b4b80-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4b80-122">Header</span></span>|<span data-ttu-id="b4b80-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b4b80-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4b80-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4b80-124">Authorization</span></span>|<span data-ttu-id="b4b80-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4b80-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4b80-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b4b80-126">Accept</span></span>|<span data-ttu-id="b4b80-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b4b80-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4b80-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b4b80-128">Request body</span></span>
<span data-ttu-id="b4b80-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4b80-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4b80-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4b80-130">Response</span></span>
<span data-ttu-id="b4b80-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b4b80-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4b80-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b4b80-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4b80-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4b80-133">Request</span></span>
<span data-ttu-id="b4b80-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4b80-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

### <a name="response"></a><span data-ttu-id="b4b80-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4b80-135">Response</span></span>
<span data-ttu-id="b4b80-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4b80-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





