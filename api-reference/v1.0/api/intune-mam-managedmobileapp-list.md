---
title: Перечисление объектов managedMobileApp
description: Список свойств и связей объектов managedMobileApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4c827245642c3096b729853f5f8fd21a361b3862
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751533"
---
# <a name="list-managedmobileapps"></a><span data-ttu-id="36c55-103">Перечисление объектов managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="36c55-103">List managedMobileApps</span></span>

<span data-ttu-id="36c55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36c55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36c55-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36c55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36c55-106">Список свойств и связей объектов [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="36c55-106">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36c55-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="36c55-107">Prerequisites</span></span>
<span data-ttu-id="36c55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36c55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36c55-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36c55-110">Permission type</span></span>|<span data-ttu-id="36c55-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36c55-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36c55-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36c55-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36c55-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36c55-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="36c55-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36c55-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36c55-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36c55-115">Not supported.</span></span>|
|<span data-ttu-id="36c55-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="36c55-116">Application</span></span>|<span data-ttu-id="36c55-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36c55-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36c55-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36c55-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps
```

## <a name="request-headers"></a><span data-ttu-id="36c55-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="36c55-119">Request headers</span></span>
|<span data-ttu-id="36c55-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36c55-120">Header</span></span>|<span data-ttu-id="36c55-121">Значение</span><span class="sxs-lookup"><span data-stu-id="36c55-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36c55-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36c55-122">Authorization</span></span>|<span data-ttu-id="36c55-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36c55-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36c55-124">Accept</span><span class="sxs-lookup"><span data-stu-id="36c55-124">Accept</span></span>|<span data-ttu-id="36c55-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36c55-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36c55-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36c55-126">Request body</span></span>
<span data-ttu-id="36c55-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36c55-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36c55-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="36c55-128">Response</span></span>
<span data-ttu-id="36c55-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="36c55-129">If successful, this method returns a `200 OK` response code and a collection of [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36c55-130">Пример</span><span class="sxs-lookup"><span data-stu-id="36c55-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="36c55-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="36c55-131">Request</span></span>
<span data-ttu-id="36c55-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36c55-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
```

### <a name="response"></a><span data-ttu-id="36c55-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="36c55-133">Response</span></span>
<span data-ttu-id="36c55-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36c55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 336

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```




