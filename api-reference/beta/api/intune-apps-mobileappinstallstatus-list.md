---
title: Список Мобилеаппинсталлстатусес
description: Список свойств и связей объектов mobileAppInstallStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b89f954b3d34029f29bce8c972aa4cf09a096d03
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144683"
---
# <a name="list-mobileappinstallstatuses"></a><span data-ttu-id="fe725-103">Список Мобилеаппинсталлстатусес</span><span class="sxs-lookup"><span data-stu-id="fe725-103">List mobileAppInstallStatuses</span></span>

> <span data-ttu-id="fe725-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe725-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe725-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe725-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe725-106">Список свойств и связей объектов [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="fe725-106">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe725-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fe725-107">Prerequisites</span></span>
<span data-ttu-id="fe725-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fe725-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fe725-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe725-110">Permission type</span></span>|<span data-ttu-id="fe725-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe725-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe725-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe725-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fe725-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe725-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fe725-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe725-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe725-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe725-115">Not supported.</span></span>|
|<span data-ttu-id="fe725-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe725-116">Application</span></span>|<span data-ttu-id="fe725-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe725-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe725-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe725-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="fe725-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe725-119">Request headers</span></span>
|<span data-ttu-id="fe725-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe725-120">Header</span></span>|<span data-ttu-id="fe725-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fe725-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe725-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe725-122">Authorization</span></span>|<span data-ttu-id="fe725-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fe725-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe725-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fe725-124">Accept</span></span>|<span data-ttu-id="fe725-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fe725-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe725-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe725-126">Request body</span></span>
<span data-ttu-id="fe725-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe725-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe725-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe725-128">Response</span></span>
<span data-ttu-id="fe725-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe725-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe725-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fe725-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe725-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe725-131">Request</span></span>
<span data-ttu-id="fe725-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe725-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="fe725-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe725-133">Response</span></span>
<span data-ttu-id="fe725-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe725-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 687

{
  "value": [
    {
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
  ]
}
```




