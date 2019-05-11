---
title: Обновление объекта targetedManagedAppPolicyAssignment
description: Обновление свойств объекта targetedManagedAppPolicyAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4a1fbfeffb3504ab806783372278dd790f41b3e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33903111"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="95e28-103">Обновление объекта targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="95e28-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="95e28-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95e28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95e28-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95e28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95e28-106">Обновление свойств объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="95e28-106">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95e28-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="95e28-107">Prerequisites</span></span>
<span data-ttu-id="95e28-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95e28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95e28-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95e28-110">Permission type</span></span>|<span data-ttu-id="95e28-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95e28-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95e28-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95e28-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95e28-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e28-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="95e28-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95e28-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95e28-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95e28-115">Not supported.</span></span>|
|<span data-ttu-id="95e28-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95e28-116">Application</span></span>|<span data-ttu-id="95e28-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95e28-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95e28-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95e28-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="95e28-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95e28-119">Request headers</span></span>
|<span data-ttu-id="95e28-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95e28-120">Header</span></span>|<span data-ttu-id="95e28-121">Значение</span><span class="sxs-lookup"><span data-stu-id="95e28-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95e28-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95e28-122">Authorization</span></span>|<span data-ttu-id="95e28-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95e28-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95e28-124">Accept</span><span class="sxs-lookup"><span data-stu-id="95e28-124">Accept</span></span>|<span data-ttu-id="95e28-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95e28-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95e28-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95e28-126">Request body</span></span>
<span data-ttu-id="95e28-127">В теле запроса добавьте представление объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95e28-127">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="95e28-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="95e28-128">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="95e28-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="95e28-129">Property</span></span>|<span data-ttu-id="95e28-130">Тип</span><span class="sxs-lookup"><span data-stu-id="95e28-130">Type</span></span>|<span data-ttu-id="95e28-131">Описание</span><span class="sxs-lookup"><span data-stu-id="95e28-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95e28-132">id</span><span class="sxs-lookup"><span data-stu-id="95e28-132">id</span></span>|<span data-ttu-id="95e28-133">Строка</span><span class="sxs-lookup"><span data-stu-id="95e28-133">String</span></span>|<span data-ttu-id="95e28-134">Id</span><span class="sxs-lookup"><span data-stu-id="95e28-134">Id</span></span>|
|<span data-ttu-id="95e28-135">target</span><span class="sxs-lookup"><span data-stu-id="95e28-135">target</span></span>|[<span data-ttu-id="95e28-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="95e28-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="95e28-137">Идентификатор для развертывания группы или приложения</span><span class="sxs-lookup"><span data-stu-id="95e28-137">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="95e28-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="95e28-138">Response</span></span>
<span data-ttu-id="95e28-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="95e28-139">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95e28-140">Пример</span><span class="sxs-lookup"><span data-stu-id="95e28-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="95e28-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="95e28-141">Request</span></span>
<span data-ttu-id="95e28-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95e28-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="95e28-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="95e28-143">Response</span></span>
<span data-ttu-id="95e28-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95e28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




