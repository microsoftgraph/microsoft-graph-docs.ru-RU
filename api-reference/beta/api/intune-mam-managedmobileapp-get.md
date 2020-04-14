---
title: Получение объекта managedMobileApp
description: Чтение свойств и связей объекта managedMobileApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f768f70f43ce9f2ea5cff7b8cfd0f81508ae194
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468265"
---
# <a name="get-managedmobileapp"></a><span data-ttu-id="df029-103">Получение объекта managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="df029-103">Get managedMobileApp</span></span>

<span data-ttu-id="df029-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df029-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df029-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df029-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df029-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="df029-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df029-107">Чтение свойств и связей объекта [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="df029-107">Read properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df029-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="df029-108">Prerequisites</span></span>
<span data-ttu-id="df029-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df029-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df029-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df029-111">Permission type</span></span>|<span data-ttu-id="df029-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="df029-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df029-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df029-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df029-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="df029-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="df029-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df029-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df029-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df029-116">Not supported.</span></span>|
|<span data-ttu-id="df029-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df029-117">Application</span></span>|<span data-ttu-id="df029-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="df029-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df029-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df029-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="df029-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="df029-120">Optional query parameters</span></span>
<span data-ttu-id="df029-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="df029-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="df029-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df029-122">Request headers</span></span>
|<span data-ttu-id="df029-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="df029-123">Header</span></span>|<span data-ttu-id="df029-124">Значение</span><span class="sxs-lookup"><span data-stu-id="df029-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df029-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="df029-125">Authorization</span></span>|<span data-ttu-id="df029-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df029-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df029-127">Accept</span><span class="sxs-lookup"><span data-stu-id="df029-127">Accept</span></span>|<span data-ttu-id="df029-128">application/json</span><span class="sxs-lookup"><span data-stu-id="df029-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df029-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="df029-129">Request body</span></span>
<span data-ttu-id="df029-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="df029-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df029-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="df029-131">Response</span></span>
<span data-ttu-id="df029-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [managedMobileApp](../resources/intune-mam-managedmobileapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="df029-132">If successful, this method returns a `200 OK` response code and [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df029-133">Пример</span><span class="sxs-lookup"><span data-stu-id="df029-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="df029-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="df029-134">Request</span></span>
<span data-ttu-id="df029-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df029-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
```

### <a name="response"></a><span data-ttu-id="df029-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="df029-136">Response</span></span>
<span data-ttu-id="df029-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df029-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": {
    "@odata.type": "#microsoft.graph.managedMobileApp",
    "mobileAppIdentifier": {
      "@odata.type": "microsoft.graph.mobileAppIdentifier"
    },
    "id": "0a129715-9715-0a12-1597-120a1597120a",
    "version": "Version value"
  }
}
```



