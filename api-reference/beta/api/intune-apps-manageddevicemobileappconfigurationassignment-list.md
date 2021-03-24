---
title: Перечисление объектов managedDeviceMobileAppConfigurationAssignment
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2be31489a119a9674233cb0581c7bbc1c83b31a5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143663"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="0e635-103">Перечисление объектов managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0e635-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

<span data-ttu-id="0e635-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e635-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e635-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e635-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e635-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e635-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e635-107">Список свойств и связей объектов [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0e635-107">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e635-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0e635-108">Prerequisites</span></span>
<span data-ttu-id="0e635-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e635-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e635-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e635-111">Permission type</span></span>|<span data-ttu-id="0e635-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e635-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e635-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e635-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e635-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e635-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0e635-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e635-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e635-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e635-116">Not supported.</span></span>|
|<span data-ttu-id="0e635-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0e635-117">Application</span></span>|<span data-ttu-id="0e635-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e635-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e635-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e635-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0e635-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0e635-120">Request headers</span></span>
|<span data-ttu-id="0e635-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e635-121">Header</span></span>|<span data-ttu-id="0e635-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0e635-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e635-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e635-123">Authorization</span></span>|<span data-ttu-id="0e635-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e635-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e635-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0e635-125">Accept</span></span>|<span data-ttu-id="0e635-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e635-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e635-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e635-127">Request body</span></span>
<span data-ttu-id="0e635-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e635-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e635-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e635-129">Response</span></span>
<span data-ttu-id="0e635-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e635-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e635-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0e635-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e635-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e635-132">Request</span></span>
<span data-ttu-id="0e635-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e635-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="0e635-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e635-134">Response</span></span>
<span data-ttu-id="0e635-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e635-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




