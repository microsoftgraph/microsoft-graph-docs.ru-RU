---
title: Перечисление объектов targetedManagedAppPolicyAssignment
description: Список свойств и связей объектов targetedManagedAppPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a07e57d5718b1fb9e53c612f9ea9e898c51f95ac
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791912"
---
# <a name="list-targetedmanagedapppolicyassignments"></a><span data-ttu-id="91019-103">Перечисление объектов targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="91019-103">List targetedManagedAppPolicyAssignments</span></span>

<span data-ttu-id="91019-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91019-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91019-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91019-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91019-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91019-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91019-107">Список свойств и связей объектов [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="91019-107">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91019-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="91019-108">Prerequisites</span></span>
<span data-ttu-id="91019-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91019-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91019-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91019-111">Permission type</span></span>|<span data-ttu-id="91019-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="91019-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91019-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91019-113">Delegated (work or school account)</span></span>|<span data-ttu-id="91019-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="91019-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="91019-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91019-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91019-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91019-116">Not supported.</span></span>|
|<span data-ttu-id="91019-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91019-117">Application</span></span>|<span data-ttu-id="91019-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="91019-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91019-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91019-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="91019-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="91019-120">Request headers</span></span>
|<span data-ttu-id="91019-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91019-121">Header</span></span>|<span data-ttu-id="91019-122">Значение</span><span class="sxs-lookup"><span data-stu-id="91019-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91019-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91019-123">Authorization</span></span>|<span data-ttu-id="91019-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91019-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91019-125">Accept</span><span class="sxs-lookup"><span data-stu-id="91019-125">Accept</span></span>|<span data-ttu-id="91019-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91019-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91019-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="91019-127">Request body</span></span>
<span data-ttu-id="91019-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91019-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91019-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="91019-129">Response</span></span>
<span data-ttu-id="91019-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="91019-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91019-131">Пример</span><span class="sxs-lookup"><span data-stu-id="91019-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="91019-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="91019-132">Request</span></span>
<span data-ttu-id="91019-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91019-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
```

### <a name="response"></a><span data-ttu-id="91019-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="91019-134">Response</span></span>
<span data-ttu-id="91019-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91019-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 508

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```



