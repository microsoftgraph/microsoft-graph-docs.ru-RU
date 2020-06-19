---
title: Обновление объекта enrollmentConfigurationAssignment
description: Обновление свойств объекта enrollmentConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aa4556309abf27cb92defa45869b072b1d351eea
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791779"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="b408e-103">Обновление объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b408e-103">Update enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="b408e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b408e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b408e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b408e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b408e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b408e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b408e-107">Обновление свойств объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b408e-107">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b408e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b408e-108">Prerequisites</span></span>
<span data-ttu-id="b408e-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b408e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b408e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b408e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b408e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b408e-111">Permission type</span></span>|<span data-ttu-id="b408e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b408e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b408e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b408e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b408e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b408e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b408e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b408e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b408e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b408e-116">Not supported.</span></span>|
|<span data-ttu-id="b408e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b408e-117">Application</span></span>|<span data-ttu-id="b408e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b408e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b408e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b408e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b408e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b408e-120">Request headers</span></span>
|<span data-ttu-id="b408e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b408e-121">Header</span></span>|<span data-ttu-id="b408e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b408e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b408e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b408e-123">Authorization</span></span>|<span data-ttu-id="b408e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b408e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b408e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b408e-125">Accept</span></span>|<span data-ttu-id="b408e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b408e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b408e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b408e-127">Request body</span></span>
<span data-ttu-id="b408e-128">В теле запроса добавьте представление объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b408e-128">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="b408e-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b408e-129">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="b408e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b408e-130">Property</span></span>|<span data-ttu-id="b408e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b408e-131">Type</span></span>|<span data-ttu-id="b408e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b408e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b408e-133">id</span><span class="sxs-lookup"><span data-stu-id="b408e-133">id</span></span>|<span data-ttu-id="b408e-134">String</span><span class="sxs-lookup"><span data-stu-id="b408e-134">String</span></span>|<span data-ttu-id="b408e-135">Ключ назначения конфигурации регистрации</span><span class="sxs-lookup"><span data-stu-id="b408e-135">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="b408e-136">target</span><span class="sxs-lookup"><span data-stu-id="b408e-136">target</span></span>|[<span data-ttu-id="b408e-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b408e-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b408e-138">Представляет назначение управляемым устройствам в клиенте.</span><span class="sxs-lookup"><span data-stu-id="b408e-138">Represents an assignment to managed devices in the tenant</span></span>|
|<span data-ttu-id="b408e-139">source</span><span class="sxs-lookup"><span data-stu-id="b408e-139">source</span></span>|[<span data-ttu-id="b408e-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="b408e-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="b408e-141">Тип ресурса, используемого для развертывания, в группу, Direct или набор политик.</span><span class="sxs-lookup"><span data-stu-id="b408e-141">Type of resource used for deployment to a group, direct or policySet.</span></span> <span data-ttu-id="b408e-142">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="b408e-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="b408e-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="b408e-143">sourceId</span></span>|<span data-ttu-id="b408e-144">String</span><span class="sxs-lookup"><span data-stu-id="b408e-144">String</span></span>|<span data-ttu-id="b408e-145">Идентификатор ресурса, используемого для развертывания в группе</span><span class="sxs-lookup"><span data-stu-id="b408e-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="b408e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b408e-146">Response</span></span>
<span data-ttu-id="b408e-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b408e-147">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b408e-148">Пример</span><span class="sxs-lookup"><span data-stu-id="b408e-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="b408e-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="b408e-149">Request</span></span>
<span data-ttu-id="b408e-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b408e-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 389

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="b408e-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="b408e-151">Response</span></span>
<span data-ttu-id="b408e-152">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="b408e-152">Here is an example of the response.</span></span> <span data-ttu-id="b408e-153">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b408e-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b408e-154">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b408e-154">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 438

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



