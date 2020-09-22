---
title: Get mobileAppAssignment
description: Чтение свойств и связей объекта mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 421a01eee08f8bec2b03ddceb1ddf740fe5a5652
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977581"
---
# <a name="get-mobileappassignment"></a><span data-ttu-id="5ca24-103">Get mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="5ca24-103">Get mobileAppAssignment</span></span>

<span data-ttu-id="5ca24-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ca24-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ca24-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ca24-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ca24-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ca24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ca24-107">Чтение свойств и связей объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5ca24-107">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ca24-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5ca24-108">Prerequisites</span></span>
<span data-ttu-id="5ca24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ca24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ca24-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ca24-111">Permission type</span></span>|<span data-ttu-id="5ca24-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ca24-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ca24-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ca24-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ca24-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ca24-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5ca24-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ca24-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ca24-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ca24-116">Not supported.</span></span>|
|<span data-ttu-id="5ca24-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ca24-117">Application</span></span>|<span data-ttu-id="5ca24-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ca24-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ca24-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ca24-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ca24-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="5ca24-120">Optional query parameters</span></span>
<span data-ttu-id="5ca24-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5ca24-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ca24-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ca24-122">Request headers</span></span>
|<span data-ttu-id="5ca24-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ca24-123">Header</span></span>|<span data-ttu-id="5ca24-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5ca24-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ca24-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ca24-125">Authorization</span></span>|<span data-ttu-id="5ca24-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ca24-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ca24-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5ca24-127">Accept</span></span>|<span data-ttu-id="5ca24-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5ca24-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ca24-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5ca24-129">Request body</span></span>
<span data-ttu-id="5ca24-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ca24-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ca24-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ca24-131">Response</span></span>
<span data-ttu-id="5ca24-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5ca24-132">If successful, this method returns a `200 OK` response code and [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ca24-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5ca24-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ca24-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ca24-134">Request</span></span>
<span data-ttu-id="5ca24-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ca24-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="5ca24-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ca24-136">Response</span></span>
<span data-ttu-id="5ca24-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ca24-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 689

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppAssignment",
    "id": "591620b7-20b7-5916-b720-1659b7201659",
    "intent": "required",
    "target": {
      "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    },
    "settings": {
      "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings",
      "vpnConfigurationId": "Vpn Configuration Id value",
      "uninstallOnDeviceRemoval": true
    },
    "source": "policySets",
    "sourceId": "Source Id value"
  }
}
```






