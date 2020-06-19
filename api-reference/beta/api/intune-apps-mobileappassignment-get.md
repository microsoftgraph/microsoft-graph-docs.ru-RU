---
title: Get mobileAppAssignment
description: Чтение свойств и связей объекта mobileAppAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: df5dad617e34ceb47c312d490a22cbf6b029927d
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793334"
---
# <a name="get-mobileappassignment"></a><span data-ttu-id="47d2e-103">Get mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="47d2e-103">Get mobileAppAssignment</span></span>

<span data-ttu-id="47d2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47d2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47d2e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47d2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47d2e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47d2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47d2e-107">Чтение свойств и связей объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="47d2e-107">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47d2e-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="47d2e-108">Prerequisites</span></span>
<span data-ttu-id="47d2e-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="47d2e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="47d2e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47d2e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47d2e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47d2e-111">Permission type</span></span>|<span data-ttu-id="47d2e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47d2e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47d2e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47d2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47d2e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="47d2e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="47d2e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47d2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47d2e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47d2e-116">Not supported.</span></span>|
|<span data-ttu-id="47d2e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47d2e-117">Application</span></span>|<span data-ttu-id="47d2e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="47d2e-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47d2e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47d2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47d2e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="47d2e-120">Optional query parameters</span></span>
<span data-ttu-id="47d2e-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="47d2e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47d2e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47d2e-122">Request headers</span></span>
|<span data-ttu-id="47d2e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47d2e-123">Header</span></span>|<span data-ttu-id="47d2e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="47d2e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47d2e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47d2e-125">Authorization</span></span>|<span data-ttu-id="47d2e-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47d2e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47d2e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="47d2e-127">Accept</span></span>|<span data-ttu-id="47d2e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="47d2e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47d2e-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="47d2e-129">Request body</span></span>
<span data-ttu-id="47d2e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47d2e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47d2e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="47d2e-131">Response</span></span>
<span data-ttu-id="47d2e-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="47d2e-132">If successful, this method returns a `200 OK` response code and [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47d2e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="47d2e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="47d2e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="47d2e-134">Request</span></span>
<span data-ttu-id="47d2e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47d2e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="47d2e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="47d2e-136">Response</span></span>
<span data-ttu-id="47d2e-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="47d2e-137">Here is an example of the response.</span></span> <span data-ttu-id="47d2e-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="47d2e-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="47d2e-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="47d2e-139">All of the properties will be returned from an actual call.</span></span>
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



