---
title: Обновление объекта targetedManagedAppPolicyAssignment
description: Обновление свойств объекта targetedManagedAppPolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2beaa0f25b5000eb02fdc4942a63b66e58f8549d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018115"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="6d053-103">Обновление объекта targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="6d053-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="6d053-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d053-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d053-105">Обновление свойств объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6d053-105">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d053-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6d053-106">Prerequisites</span></span>
<span data-ttu-id="6d053-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d053-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d053-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d053-109">Permission type</span></span>|<span data-ttu-id="6d053-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d053-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d053-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d053-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6d053-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d053-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6d053-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d053-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d053-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d053-114">Not supported.</span></span>|
|<span data-ttu-id="6d053-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d053-115">Application</span></span>|<span data-ttu-id="6d053-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d053-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d053-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d053-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="6d053-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d053-118">Request headers</span></span>
|<span data-ttu-id="6d053-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d053-119">Header</span></span>|<span data-ttu-id="6d053-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6d053-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d053-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d053-121">Authorization</span></span>|<span data-ttu-id="6d053-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d053-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d053-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6d053-123">Accept</span></span>|<span data-ttu-id="6d053-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6d053-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d053-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6d053-125">Request body</span></span>
<span data-ttu-id="6d053-126">В теле запроса добавьте представление объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d053-126">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="6d053-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6d053-127">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="6d053-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d053-128">Property</span></span>|<span data-ttu-id="6d053-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6d053-129">Type</span></span>|<span data-ttu-id="6d053-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6d053-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d053-131">id</span><span class="sxs-lookup"><span data-stu-id="6d053-131">id</span></span>|<span data-ttu-id="6d053-132">String</span><span class="sxs-lookup"><span data-stu-id="6d053-132">String</span></span>|<span data-ttu-id="6d053-133">Id</span><span class="sxs-lookup"><span data-stu-id="6d053-133">Id</span></span>|
|<span data-ttu-id="6d053-134">target</span><span class="sxs-lookup"><span data-stu-id="6d053-134">target</span></span>|[<span data-ttu-id="6d053-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6d053-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6d053-136">Идентификатор для развертывания группы или приложения</span><span class="sxs-lookup"><span data-stu-id="6d053-136">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="6d053-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d053-137">Response</span></span>
<span data-ttu-id="6d053-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6d053-138">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d053-139">Пример</span><span class="sxs-lookup"><span data-stu-id="6d053-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d053-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d053-140">Request</span></span>
<span data-ttu-id="6d053-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d053-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6d053-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d053-142">Response</span></span>
<span data-ttu-id="6d053-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d053-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



