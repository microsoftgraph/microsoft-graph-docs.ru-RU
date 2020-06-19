---
title: Перечисление объектов managedDeviceMobileAppConfigurationAssignment
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 440c2ca3cffb9ad0212dcc5ff67fbce8ed9ffa05
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793355"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="55152-103">Перечисление объектов managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="55152-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

<span data-ttu-id="55152-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55152-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55152-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55152-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55152-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55152-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55152-107">Список свойств и связей объектов [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="55152-107">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55152-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="55152-108">Prerequisites</span></span>
<span data-ttu-id="55152-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="55152-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="55152-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55152-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55152-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55152-111">Permission type</span></span>|<span data-ttu-id="55152-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55152-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55152-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55152-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55152-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="55152-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="55152-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55152-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55152-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55152-116">Not supported.</span></span>|
|<span data-ttu-id="55152-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55152-117">Application</span></span>|<span data-ttu-id="55152-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="55152-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55152-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55152-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="55152-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="55152-120">Request headers</span></span>
|<span data-ttu-id="55152-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55152-121">Header</span></span>|<span data-ttu-id="55152-122">Значение</span><span class="sxs-lookup"><span data-stu-id="55152-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55152-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55152-123">Authorization</span></span>|<span data-ttu-id="55152-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55152-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55152-125">Accept</span><span class="sxs-lookup"><span data-stu-id="55152-125">Accept</span></span>|<span data-ttu-id="55152-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55152-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55152-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="55152-127">Request body</span></span>
<span data-ttu-id="55152-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55152-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55152-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="55152-129">Response</span></span>
<span data-ttu-id="55152-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55152-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55152-131">Пример</span><span class="sxs-lookup"><span data-stu-id="55152-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="55152-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="55152-132">Request</span></span>
<span data-ttu-id="55152-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55152-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="55152-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="55152-134">Response</span></span>
<span data-ttu-id="55152-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="55152-135">Here is an example of the response.</span></span> <span data-ttu-id="55152-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="55152-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="55152-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="55152-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 456

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



