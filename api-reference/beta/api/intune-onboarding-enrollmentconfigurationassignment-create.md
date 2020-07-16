---
title: Создание объекта enrollmentConfigurationAssignment
description: Создание объекта enrollmentConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0dca3b38d73dc8f3d2906630fdd4069d66c8e192
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791800"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="2cc97-103">Создание объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2cc97-103">Create enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="2cc97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cc97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2cc97-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cc97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cc97-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2cc97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cc97-107">Создание объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2cc97-107">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2cc97-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2cc97-108">Prerequisites</span></span>
<span data-ttu-id="2cc97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cc97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cc97-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cc97-111">Permission type</span></span>|<span data-ttu-id="2cc97-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cc97-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cc97-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cc97-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2cc97-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cc97-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2cc97-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cc97-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cc97-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cc97-116">Not supported.</span></span>|
|<span data-ttu-id="2cc97-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2cc97-117">Application</span></span>|<span data-ttu-id="2cc97-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cc97-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cc97-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cc97-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2cc97-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2cc97-120">Request headers</span></span>
|<span data-ttu-id="2cc97-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2cc97-121">Header</span></span>|<span data-ttu-id="2cc97-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2cc97-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cc97-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2cc97-123">Authorization</span></span>|<span data-ttu-id="2cc97-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2cc97-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cc97-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2cc97-125">Accept</span></span>|<span data-ttu-id="2cc97-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2cc97-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cc97-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2cc97-127">Request body</span></span>
<span data-ttu-id="2cc97-128">В теле запроса добавьте представление объекта enrollmentConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cc97-128">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="2cc97-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта enrollmentConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="2cc97-129">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="2cc97-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2cc97-130">Property</span></span>|<span data-ttu-id="2cc97-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2cc97-131">Type</span></span>|<span data-ttu-id="2cc97-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2cc97-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cc97-133">id</span><span class="sxs-lookup"><span data-stu-id="2cc97-133">id</span></span>|<span data-ttu-id="2cc97-134">String</span><span class="sxs-lookup"><span data-stu-id="2cc97-134">String</span></span>|<span data-ttu-id="2cc97-135">Ключ назначения конфигурации регистрации</span><span class="sxs-lookup"><span data-stu-id="2cc97-135">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="2cc97-136">target</span><span class="sxs-lookup"><span data-stu-id="2cc97-136">target</span></span>|[<span data-ttu-id="2cc97-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2cc97-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2cc97-138">Представляет назначение управляемым устройствам в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2cc97-138">Represents an assignment to managed devices in the tenant</span></span>|
|<span data-ttu-id="2cc97-139">source</span><span class="sxs-lookup"><span data-stu-id="2cc97-139">source</span></span>|[<span data-ttu-id="2cc97-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="2cc97-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="2cc97-141">Тип ресурса, используемого для развертывания, в группу, Direct или набор политик.</span><span class="sxs-lookup"><span data-stu-id="2cc97-141">Type of resource used for deployment to a group, direct or policySet.</span></span> <span data-ttu-id="2cc97-142">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="2cc97-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="2cc97-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="2cc97-143">sourceId</span></span>|<span data-ttu-id="2cc97-144">String</span><span class="sxs-lookup"><span data-stu-id="2cc97-144">String</span></span>|<span data-ttu-id="2cc97-145">Идентификатор ресурса, используемого для развертывания в группе</span><span class="sxs-lookup"><span data-stu-id="2cc97-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="2cc97-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cc97-146">Response</span></span>
<span data-ttu-id="2cc97-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2cc97-147">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cc97-148">Пример</span><span class="sxs-lookup"><span data-stu-id="2cc97-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="2cc97-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cc97-149">Request</span></span>
<span data-ttu-id="2cc97-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2cc97-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
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

### <a name="response"></a><span data-ttu-id="2cc97-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cc97-151">Response</span></span>
<span data-ttu-id="2cc97-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2cc97-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



