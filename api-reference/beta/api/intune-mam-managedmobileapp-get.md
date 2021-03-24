---
title: Получение объекта managedMobileApp
description: Чтение свойств и связей объекта managedMobileApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e956d4759cb8465163d63a0492c222cba8183b41
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135252"
---
# <a name="get-managedmobileapp"></a><span data-ttu-id="5bc49-103">Получение объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="5bc49-103">Get managedMobileApp</span></span>

<span data-ttu-id="5bc49-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bc49-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5bc49-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bc49-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bc49-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5bc49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bc49-107">Чтение свойств и связей объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5bc49-107">Read properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bc49-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5bc49-108">Prerequisites</span></span>
<span data-ttu-id="5bc49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bc49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bc49-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bc49-111">Permission type</span></span>|<span data-ttu-id="5bc49-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bc49-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bc49-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bc49-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5bc49-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bc49-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5bc49-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bc49-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bc49-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bc49-116">Not supported.</span></span>|
|<span data-ttu-id="5bc49-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5bc49-117">Application</span></span>|<span data-ttu-id="5bc49-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bc49-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bc49-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bc49-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="5bc49-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5bc49-120">Optional query parameters</span></span>
<span data-ttu-id="5bc49-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5bc49-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bc49-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5bc49-122">Request headers</span></span>
|<span data-ttu-id="5bc49-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5bc49-123">Header</span></span>|<span data-ttu-id="5bc49-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5bc49-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bc49-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bc49-125">Authorization</span></span>|<span data-ttu-id="5bc49-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5bc49-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bc49-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5bc49-127">Accept</span></span>|<span data-ttu-id="5bc49-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5bc49-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bc49-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5bc49-129">Request body</span></span>
<span data-ttu-id="5bc49-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5bc49-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bc49-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bc49-131">Response</span></span>
<span data-ttu-id="5bc49-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5bc49-132">If successful, this method returns a `200 OK` response code and [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bc49-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5bc49-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bc49-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bc49-134">Request</span></span>
<span data-ttu-id="5bc49-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5bc49-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
```

### <a name="response"></a><span data-ttu-id="5bc49-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bc49-136">Response</span></span>
<span data-ttu-id="5bc49-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5bc49-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 309

{
  "value": {
    "@odata.type": "#microsoft.graph.managedMobileApp",
    "mobileAppIdentifier": {
      "@odata.type": "microsoft.graph.windowsAppIdentifier",
      "windowsAppId": "Windows App Id value"
    },
    "id": "0a129715-9715-0a12-1597-120a1597120a",
    "version": "Version value"
  }
}
```




