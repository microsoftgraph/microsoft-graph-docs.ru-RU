---
title: Обновление объекта enrollmentConfigurationAssignment
description: Обновление свойств объекта enrollmentConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ab02a29b0e0803484be4fb0e1930f7ba3fd987ae
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941654"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="a4f55-103">Обновление объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a4f55-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="a4f55-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4f55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4f55-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4f55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4f55-106">Обновление свойств объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a4f55-106">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4f55-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a4f55-107">Prerequisites</span></span>
<span data-ttu-id="a4f55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4f55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4f55-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4f55-110">Permission type</span></span>|<span data-ttu-id="a4f55-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4f55-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4f55-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4f55-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4f55-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4f55-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a4f55-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4f55-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4f55-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4f55-115">Not supported.</span></span>|
|<span data-ttu-id="a4f55-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4f55-116">Application</span></span>|<span data-ttu-id="a4f55-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4f55-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4f55-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4f55-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="a4f55-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a4f55-119">Request headers</span></span>
|<span data-ttu-id="a4f55-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4f55-120">Header</span></span>|<span data-ttu-id="a4f55-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a4f55-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4f55-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4f55-122">Authorization</span></span>|<span data-ttu-id="a4f55-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4f55-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4f55-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a4f55-124">Accept</span></span>|<span data-ttu-id="a4f55-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4f55-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4f55-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a4f55-126">Request body</span></span>
<span data-ttu-id="a4f55-127">В теле запроса добавьте представление объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4f55-127">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="a4f55-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a4f55-128">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="a4f55-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4f55-129">Property</span></span>|<span data-ttu-id="a4f55-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a4f55-130">Type</span></span>|<span data-ttu-id="a4f55-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a4f55-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4f55-132">id</span><span class="sxs-lookup"><span data-stu-id="a4f55-132">id</span></span>|<span data-ttu-id="a4f55-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a4f55-133">String</span></span>|<span data-ttu-id="a4f55-134">Ключ назначения конфигурации регистрации</span><span class="sxs-lookup"><span data-stu-id="a4f55-134">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="a4f55-135">target</span><span class="sxs-lookup"><span data-stu-id="a4f55-135">target</span></span>|[<span data-ttu-id="a4f55-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a4f55-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a4f55-137">Представляет назначение управляемым устройствам в клиенте.</span><span class="sxs-lookup"><span data-stu-id="a4f55-137">Represents an assignment to managed devices in the tenant</span></span>|
|<span data-ttu-id="a4f55-138">source</span><span class="sxs-lookup"><span data-stu-id="a4f55-138">source</span></span>|[<span data-ttu-id="a4f55-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="a4f55-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="a4f55-140">Тип ресурса, используемого для развертывания, в группу, Direct или набор политик.</span><span class="sxs-lookup"><span data-stu-id="a4f55-140">Type of resource used for deployment to a group, direct or policySet.</span></span> <span data-ttu-id="a4f55-141">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="a4f55-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="a4f55-142">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="a4f55-142">sourceId</span></span>|<span data-ttu-id="a4f55-143">Строка</span><span class="sxs-lookup"><span data-stu-id="a4f55-143">String</span></span>|<span data-ttu-id="a4f55-144">Идентификатор ресурса, используемого для развертывания в группе</span><span class="sxs-lookup"><span data-stu-id="a4f55-144">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="a4f55-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4f55-145">Response</span></span>
<span data-ttu-id="a4f55-146">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a4f55-146">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4f55-147">Пример</span><span class="sxs-lookup"><span data-stu-id="a4f55-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4f55-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4f55-148">Request</span></span>
<span data-ttu-id="a4f55-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4f55-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
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

### <a name="response"></a><span data-ttu-id="a4f55-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4f55-150">Response</span></span>
<span data-ttu-id="a4f55-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4f55-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





