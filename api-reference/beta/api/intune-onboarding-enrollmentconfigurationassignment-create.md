---
title: Создание объекта enrollmentConfigurationAssignment
description: Создание объекта enrollmentConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 09780e959d50a433893b70edcd308420c55be2f4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709224"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="8b627-103">Создание объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="8b627-103">Create enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="8b627-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b627-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b627-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b627-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b627-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b627-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b627-107">Создание объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8b627-107">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b627-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8b627-108">Prerequisites</span></span>
<span data-ttu-id="8b627-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b627-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b627-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b627-111">Permission type</span></span>|<span data-ttu-id="8b627-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b627-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b627-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b627-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8b627-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b627-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8b627-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b627-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b627-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b627-116">Not supported.</span></span>|
|<span data-ttu-id="8b627-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b627-117">Application</span></span>|<span data-ttu-id="8b627-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b627-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b627-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b627-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8b627-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8b627-120">Request headers</span></span>
|<span data-ttu-id="8b627-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b627-121">Header</span></span>|<span data-ttu-id="8b627-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8b627-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b627-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b627-123">Authorization</span></span>|<span data-ttu-id="8b627-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b627-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b627-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8b627-125">Accept</span></span>|<span data-ttu-id="8b627-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b627-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b627-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8b627-127">Request body</span></span>
<span data-ttu-id="8b627-128">В теле запроса добавьте представление объекта enrollmentConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b627-128">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="8b627-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта enrollmentConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="8b627-129">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="8b627-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b627-130">Property</span></span>|<span data-ttu-id="8b627-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8b627-131">Type</span></span>|<span data-ttu-id="8b627-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8b627-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b627-133">id</span><span class="sxs-lookup"><span data-stu-id="8b627-133">id</span></span>|<span data-ttu-id="8b627-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8b627-134">String</span></span>|<span data-ttu-id="8b627-135">Ключ назначения конфигурации регистрации</span><span class="sxs-lookup"><span data-stu-id="8b627-135">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="8b627-136">target</span><span class="sxs-lookup"><span data-stu-id="8b627-136">target</span></span>|[<span data-ttu-id="8b627-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8b627-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8b627-138">Представляет назначение управляемым устройствам в клиенте.</span><span class="sxs-lookup"><span data-stu-id="8b627-138">Represents an assignment to managed devices in the tenant</span></span>|
|<span data-ttu-id="8b627-139">source</span><span class="sxs-lookup"><span data-stu-id="8b627-139">source</span></span>|[<span data-ttu-id="8b627-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="8b627-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="8b627-141">Тип ресурса, используемого для развертывания, в группу, Direct или набор политик.</span><span class="sxs-lookup"><span data-stu-id="8b627-141">Type of resource used for deployment to a group, direct or policySet.</span></span> <span data-ttu-id="8b627-142">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="8b627-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="8b627-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="8b627-143">sourceId</span></span>|<span data-ttu-id="8b627-144">Строка</span><span class="sxs-lookup"><span data-stu-id="8b627-144">String</span></span>|<span data-ttu-id="8b627-145">Идентификатор ресурса, используемого для развертывания в группе</span><span class="sxs-lookup"><span data-stu-id="8b627-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="8b627-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b627-146">Response</span></span>
<span data-ttu-id="8b627-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8b627-147">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b627-148">Пример</span><span class="sxs-lookup"><span data-stu-id="8b627-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b627-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b627-149">Request</span></span>
<span data-ttu-id="8b627-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b627-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8b627-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b627-151">Response</span></span>
<span data-ttu-id="8b627-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b627-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





