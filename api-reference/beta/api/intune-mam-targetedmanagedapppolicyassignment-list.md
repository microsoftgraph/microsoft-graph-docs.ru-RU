---
title: Перечисление объектов targetedManagedAppPolicyAssignment
description: Список свойств и связей объектов targetedManagedAppPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d226b1af5d23a362aeea1165ca619aee1f01476c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149032"
---
# <a name="list-targetedmanagedapppolicyassignments"></a><span data-ttu-id="0a001-103">Перечисление объектов targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="0a001-103">List targetedManagedAppPolicyAssignments</span></span>

<span data-ttu-id="0a001-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a001-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a001-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a001-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a001-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a001-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a001-107">Список свойств и связей объектов [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0a001-107">List properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a001-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0a001-108">Prerequisites</span></span>
<span data-ttu-id="0a001-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a001-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a001-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a001-111">Permission type</span></span>|<span data-ttu-id="0a001-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a001-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a001-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a001-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a001-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a001-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0a001-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a001-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a001-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a001-116">Not supported.</span></span>|
|<span data-ttu-id="0a001-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0a001-117">Application</span></span>|<span data-ttu-id="0a001-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a001-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a001-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a001-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0a001-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0a001-120">Request headers</span></span>
|<span data-ttu-id="0a001-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a001-121">Header</span></span>|<span data-ttu-id="0a001-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0a001-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a001-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a001-123">Authorization</span></span>|<span data-ttu-id="0a001-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a001-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a001-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0a001-125">Accept</span></span>|<span data-ttu-id="0a001-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a001-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a001-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a001-127">Request body</span></span>
<span data-ttu-id="0a001-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a001-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a001-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a001-129">Response</span></span>
<span data-ttu-id="0a001-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0a001-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a001-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0a001-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a001-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a001-132">Request</span></span>
<span data-ttu-id="0a001-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a001-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
```

### <a name="response"></a><span data-ttu-id="0a001-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a001-134">Response</span></span>
<span data-ttu-id="0a001-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a001-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
      "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```




