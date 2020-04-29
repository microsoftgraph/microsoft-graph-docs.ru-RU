---
title: Обновление объекта targetedManagedAppPolicyAssignment
description: Обновление свойств объекта targetedManagedAppPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 285186526de68c02f12de2e03736160bbebdfd47
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43397796"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="ff0db-103">Обновление объекта targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="ff0db-103">Update targetedManagedAppPolicyAssignment</span></span>

<span data-ttu-id="ff0db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff0db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff0db-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff0db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff0db-106">Обновление свойств объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff0db-106">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff0db-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ff0db-107">Prerequisites</span></span>
<span data-ttu-id="ff0db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff0db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff0db-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff0db-110">Permission type</span></span>|<span data-ttu-id="ff0db-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff0db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff0db-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff0db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ff0db-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff0db-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ff0db-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff0db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff0db-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff0db-115">Not supported.</span></span>|
|<span data-ttu-id="ff0db-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff0db-116">Application</span></span>|<span data-ttu-id="ff0db-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff0db-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff0db-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff0db-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="ff0db-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ff0db-119">Request headers</span></span>
|<span data-ttu-id="ff0db-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff0db-120">Header</span></span>|<span data-ttu-id="ff0db-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ff0db-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff0db-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff0db-122">Authorization</span></span>|<span data-ttu-id="ff0db-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff0db-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff0db-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ff0db-124">Accept</span></span>|<span data-ttu-id="ff0db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ff0db-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff0db-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ff0db-126">Request body</span></span>
<span data-ttu-id="ff0db-127">В теле запроса добавьте представление объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff0db-127">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="ff0db-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff0db-128">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="ff0db-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff0db-129">Property</span></span>|<span data-ttu-id="ff0db-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ff0db-130">Type</span></span>|<span data-ttu-id="ff0db-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ff0db-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff0db-132">id</span><span class="sxs-lookup"><span data-stu-id="ff0db-132">id</span></span>|<span data-ttu-id="ff0db-133">String</span><span class="sxs-lookup"><span data-stu-id="ff0db-133">String</span></span>|<span data-ttu-id="ff0db-134">Id</span><span class="sxs-lookup"><span data-stu-id="ff0db-134">Id</span></span>|
|<span data-ttu-id="ff0db-135">target</span><span class="sxs-lookup"><span data-stu-id="ff0db-135">target</span></span>|[<span data-ttu-id="ff0db-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ff0db-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ff0db-137">Идентификатор для развертывания группы или приложения</span><span class="sxs-lookup"><span data-stu-id="ff0db-137">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="ff0db-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff0db-138">Response</span></span>
<span data-ttu-id="ff0db-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ff0db-139">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff0db-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ff0db-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff0db-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff0db-141">Request</span></span>
<span data-ttu-id="ff0db-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff0db-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ff0db-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff0db-143">Response</span></span>
<span data-ttu-id="ff0db-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff0db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```






