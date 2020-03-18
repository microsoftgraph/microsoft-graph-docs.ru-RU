---
title: Создание объекта enrollmentConfigurationAssignment
description: Создание объекта enrollmentConfigurationAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ff95425c059126c4e69052f05905cb999498b2ee
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802848"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="6a109-103">Создание объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6a109-103">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="6a109-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a109-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a109-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a109-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a109-106">Создание объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6a109-106">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a109-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6a109-107">Prerequisites</span></span>
<span data-ttu-id="6a109-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a109-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a109-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a109-110">Permission type</span></span>|<span data-ttu-id="6a109-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a109-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a109-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a109-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a109-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a109-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6a109-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a109-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a109-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a109-115">Not supported.</span></span>|
|<span data-ttu-id="6a109-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6a109-116">Application</span></span>|<span data-ttu-id="6a109-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a109-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a109-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a109-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6a109-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6a109-119">Request headers</span></span>
|<span data-ttu-id="6a109-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6a109-120">Header</span></span>|<span data-ttu-id="6a109-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6a109-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a109-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a109-122">Authorization</span></span>|<span data-ttu-id="6a109-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a109-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a109-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6a109-124">Accept</span></span>|<span data-ttu-id="6a109-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a109-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a109-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a109-126">Request body</span></span>
<span data-ttu-id="6a109-127">В теле запроса добавьте представление объекта enrollmentConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a109-127">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="6a109-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта enrollmentConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="6a109-128">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="6a109-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a109-129">Property</span></span>|<span data-ttu-id="6a109-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6a109-130">Type</span></span>|<span data-ttu-id="6a109-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6a109-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a109-132">id</span><span class="sxs-lookup"><span data-stu-id="6a109-132">id</span></span>|<span data-ttu-id="6a109-133">String</span><span class="sxs-lookup"><span data-stu-id="6a109-133">String</span></span>|<span data-ttu-id="6a109-134">Ключ назначения конфигурации регистрации</span><span class="sxs-lookup"><span data-stu-id="6a109-134">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="6a109-135">target</span><span class="sxs-lookup"><span data-stu-id="6a109-135">target</span></span>|[<span data-ttu-id="6a109-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6a109-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6a109-137">Представляет назначение управляемым устройствам в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6a109-137">Represents an assignment to managed devices in the tenant</span></span>|
|<span data-ttu-id="6a109-138">source</span><span class="sxs-lookup"><span data-stu-id="6a109-138">source</span></span>|[<span data-ttu-id="6a109-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="6a109-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="6a109-140">Тип ресурса, используемого для развертывания, в группу, Direct или набор политик.</span><span class="sxs-lookup"><span data-stu-id="6a109-140">Type of resource used for deployment to a group, direct or policySet.</span></span> <span data-ttu-id="6a109-141">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="6a109-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="6a109-142">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="6a109-142">sourceId</span></span>|<span data-ttu-id="6a109-143">String</span><span class="sxs-lookup"><span data-stu-id="6a109-143">String</span></span>|<span data-ttu-id="6a109-144">Идентификатор ресурса, используемого для развертывания в группе</span><span class="sxs-lookup"><span data-stu-id="6a109-144">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="6a109-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a109-145">Response</span></span>
<span data-ttu-id="6a109-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6a109-146">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a109-147">Пример</span><span class="sxs-lookup"><span data-stu-id="6a109-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a109-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a109-148">Request</span></span>
<span data-ttu-id="6a109-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a109-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 234

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="6a109-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a109-150">Response</span></span>
<span data-ttu-id="6a109-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a109-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 283

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```




