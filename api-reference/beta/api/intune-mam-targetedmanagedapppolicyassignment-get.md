---
title: Get targetedManagedAppPolicyAssignment
description: Чтение свойств и связей объекта targetedManagedAppPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d093ef5724b8d1eafb6645defddfa21244a4200b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149046"
---
# <a name="get-targetedmanagedapppolicyassignment"></a><span data-ttu-id="53403-103">Get targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="53403-103">Get targetedManagedAppPolicyAssignment</span></span>

<span data-ttu-id="53403-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53403-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53403-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53403-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53403-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53403-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53403-107">Чтение свойств и связей объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="53403-107">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53403-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="53403-108">Prerequisites</span></span>
<span data-ttu-id="53403-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53403-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53403-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53403-111">Permission type</span></span>|<span data-ttu-id="53403-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53403-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53403-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53403-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53403-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53403-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="53403-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53403-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53403-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53403-116">Not supported.</span></span>|
|<span data-ttu-id="53403-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="53403-117">Application</span></span>|<span data-ttu-id="53403-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53403-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53403-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53403-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53403-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="53403-120">Optional query parameters</span></span>
<span data-ttu-id="53403-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="53403-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53403-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53403-122">Request headers</span></span>
|<span data-ttu-id="53403-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53403-123">Header</span></span>|<span data-ttu-id="53403-124">Значение</span><span class="sxs-lookup"><span data-stu-id="53403-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53403-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="53403-125">Authorization</span></span>|<span data-ttu-id="53403-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53403-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53403-127">Accept</span><span class="sxs-lookup"><span data-stu-id="53403-127">Accept</span></span>|<span data-ttu-id="53403-128">application/json</span><span class="sxs-lookup"><span data-stu-id="53403-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53403-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53403-129">Request body</span></span>
<span data-ttu-id="53403-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53403-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53403-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="53403-131">Response</span></span>
<span data-ttu-id="53403-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="53403-132">If successful, this method returns a `200 OK` response code and [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53403-133">Пример</span><span class="sxs-lookup"><span data-stu-id="53403-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="53403-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="53403-134">Request</span></span>
<span data-ttu-id="53403-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53403-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="53403-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="53403-136">Response</span></span>
<span data-ttu-id="53403-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53403-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 542

{
  "value": {
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
}
```




