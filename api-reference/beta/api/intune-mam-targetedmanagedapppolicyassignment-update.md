---
title: Обновление объекта targetedManagedAppPolicyAssignment
description: Обновление свойств объекта targetedManagedAppPolicyAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: adcc1fc1fa088e3a9517302f0efe342a7b53da1e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39942228"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="9fe77-103">Обновление объекта targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="9fe77-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="9fe77-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fe77-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fe77-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fe77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fe77-106">Обновление свойств объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9fe77-106">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fe77-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9fe77-107">Prerequisites</span></span>
<span data-ttu-id="9fe77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fe77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fe77-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fe77-110">Permission type</span></span>|<span data-ttu-id="9fe77-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fe77-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fe77-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fe77-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9fe77-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fe77-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9fe77-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fe77-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fe77-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fe77-115">Not supported.</span></span>|
|<span data-ttu-id="9fe77-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fe77-116">Application</span></span>|<span data-ttu-id="9fe77-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fe77-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fe77-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fe77-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9fe77-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9fe77-119">Request headers</span></span>
|<span data-ttu-id="9fe77-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9fe77-120">Header</span></span>|<span data-ttu-id="9fe77-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9fe77-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fe77-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9fe77-122">Authorization</span></span>|<span data-ttu-id="9fe77-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fe77-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fe77-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9fe77-124">Accept</span></span>|<span data-ttu-id="9fe77-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9fe77-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fe77-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9fe77-126">Request body</span></span>
<span data-ttu-id="9fe77-127">В теле запроса добавьте представление объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fe77-127">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="9fe77-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9fe77-128">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="9fe77-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fe77-129">Property</span></span>|<span data-ttu-id="9fe77-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9fe77-130">Type</span></span>|<span data-ttu-id="9fe77-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9fe77-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fe77-132">id</span><span class="sxs-lookup"><span data-stu-id="9fe77-132">id</span></span>|<span data-ttu-id="9fe77-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9fe77-133">String</span></span>|<span data-ttu-id="9fe77-134">Id</span><span class="sxs-lookup"><span data-stu-id="9fe77-134">Id</span></span>|
|<span data-ttu-id="9fe77-135">target</span><span class="sxs-lookup"><span data-stu-id="9fe77-135">target</span></span>|[<span data-ttu-id="9fe77-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9fe77-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9fe77-137">Идентификатор для развертывания в группе или приложении</span><span class="sxs-lookup"><span data-stu-id="9fe77-137">Identifier for deployment to a group or app</span></span>|
|<span data-ttu-id="9fe77-138">source</span><span class="sxs-lookup"><span data-stu-id="9fe77-138">source</span></span>|[<span data-ttu-id="9fe77-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="9fe77-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="9fe77-140">Тип ресурса, используемого для развертывания в группу, Direct или в упаковке/набор политик.</span><span class="sxs-lookup"><span data-stu-id="9fe77-140">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="9fe77-141">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="9fe77-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="9fe77-142">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="9fe77-142">sourceId</span></span>|<span data-ttu-id="9fe77-143">Строка</span><span class="sxs-lookup"><span data-stu-id="9fe77-143">String</span></span>|<span data-ttu-id="9fe77-144">Идентификатор ресурса, используемого для развертывания в группе</span><span class="sxs-lookup"><span data-stu-id="9fe77-144">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="9fe77-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fe77-145">Response</span></span>
<span data-ttu-id="9fe77-146">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9fe77-146">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fe77-147">Пример</span><span class="sxs-lookup"><span data-stu-id="9fe77-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fe77-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fe77-148">Request</span></span>
<span data-ttu-id="9fe77-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fe77-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="9fe77-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fe77-150">Response</span></span>
<span data-ttu-id="9fe77-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9fe77-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 284

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```





