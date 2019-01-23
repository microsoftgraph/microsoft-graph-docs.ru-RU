---
title: Получение mobileAppInstallStatus
description: Чтение свойства и связи объекта mobileAppInstallStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 37821fe795ec87b9c474b15a238060c513623f12
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424058"
---
# <a name="get-mobileappinstallstatus"></a><span data-ttu-id="5e4ca-103">Получение mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="5e4ca-103">Get mobileAppInstallStatus</span></span>

> <span data-ttu-id="5e4ca-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5e4ca-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5e4ca-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e4ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e4ca-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e4ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e4ca-107">Чтение свойства и связи объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="5e4ca-107">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e4ca-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="5e4ca-108">Prerequisites</span></span>
<span data-ttu-id="5e4ca-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5e4ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5e4ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e4ca-111">Permission type</span></span>|<span data-ttu-id="5e4ca-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e4ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e4ca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e4ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e4ca-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e4ca-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5e4ca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e4ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e4ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e4ca-116">Not supported.</span></span>|
|<span data-ttu-id="5e4ca-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e4ca-117">Application</span></span>|<span data-ttu-id="5e4ca-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e4ca-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e4ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e4ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5e4ca-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5e4ca-120">Optional query parameters</span></span>
<span data-ttu-id="5e4ca-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5e4ca-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e4ca-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e4ca-122">Request headers</span></span>
|<span data-ttu-id="5e4ca-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e4ca-123">Header</span></span>|<span data-ttu-id="5e4ca-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5e4ca-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e4ca-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e4ca-125">Authorization</span></span>|<span data-ttu-id="5e4ca-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5e4ca-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e4ca-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5e4ca-127">Accept</span></span>|<span data-ttu-id="5e4ca-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5e4ca-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e4ca-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e4ca-129">Request body</span></span>
<span data-ttu-id="5e4ca-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5e4ca-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e4ca-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e4ca-131">Response</span></span>
<span data-ttu-id="5e4ca-132">Успешно завершена, этот метод возвращает `200 OK` объект [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5e4ca-132">If successful, this method returns a `200 OK` response code and [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e4ca-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5e4ca-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e4ca-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e4ca-134">Request</span></span>
<span data-ttu-id="5e4ca-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e4ca-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
```

### <a name="response"></a><span data-ttu-id="5e4ca-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e4ca-136">Response</span></span>
<span data-ttu-id="5e4ca-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5e4ca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 645

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
    "id": "7560ee45-ee45-7560-45ee-607545ee6075",
    "deviceName": "Device Name value",
    "deviceId": "Device Id value",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "mobileAppInstallStatusValue": "failed",
    "installState": "failed",
    "installStateDetail": "seeInstallErrorCode",
    "errorCode": 9,
    "osVersion": "Os Version value",
    "osDescription": "Os Description value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value",
    "displayVersion": "Display Version value"
  }
}
```




