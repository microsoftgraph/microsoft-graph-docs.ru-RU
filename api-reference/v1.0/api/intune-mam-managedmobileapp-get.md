---
title: Получение объекта managedMobileApp
description: Чтение свойств и связей объекта managedMobileApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4866bf1c545df9c55e29b9f9715ff4d3611f89a1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751540"
---
# <a name="get-managedmobileapp"></a><span data-ttu-id="7d3f8-103">Получение объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="7d3f8-103">Get managedMobileApp</span></span>

<span data-ttu-id="7d3f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d3f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d3f8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d3f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d3f8-106">Чтение свойств и связей объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3f8-106">Read properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d3f8-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7d3f8-107">Prerequisites</span></span>
<span data-ttu-id="7d3f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d3f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d3f8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d3f8-110">Permission type</span></span>|<span data-ttu-id="7d3f8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d3f8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d3f8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d3f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7d3f8-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d3f8-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7d3f8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d3f8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d3f8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d3f8-115">Not supported.</span></span>|
|<span data-ttu-id="7d3f8-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7d3f8-116">Application</span></span>|<span data-ttu-id="7d3f8-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d3f8-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d3f8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d3f8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d3f8-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7d3f8-119">Optional query parameters</span></span>
<span data-ttu-id="7d3f8-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7d3f8-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d3f8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d3f8-121">Request headers</span></span>
|<span data-ttu-id="7d3f8-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d3f8-122">Header</span></span>|<span data-ttu-id="7d3f8-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7d3f8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d3f8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d3f8-124">Authorization</span></span>|<span data-ttu-id="7d3f8-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d3f8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d3f8-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7d3f8-126">Accept</span></span>|<span data-ttu-id="7d3f8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7d3f8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d3f8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d3f8-128">Request body</span></span>
<span data-ttu-id="7d3f8-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d3f8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d3f8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d3f8-130">Response</span></span>
<span data-ttu-id="7d3f8-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7d3f8-131">If successful, this method returns a `200 OK` response code and [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d3f8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7d3f8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d3f8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d3f8-133">Request</span></span>
<span data-ttu-id="7d3f8-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d3f8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
```

### <a name="response"></a><span data-ttu-id="7d3f8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d3f8-135">Response</span></span>
<span data-ttu-id="7d3f8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d3f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 308

{
  "value": {
    "@odata.type": "#microsoft.graph.managedMobileApp",
    "mobileAppIdentifier": {
      "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
      "packageId": "Package Id value"
    },
    "id": "0a129715-9715-0a12-1597-120a1597120a",
    "version": "Version value"
  }
}
```




