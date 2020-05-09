---
title: Обновление объекта enrollmentConfigurationAssignment
description: Обновление свойств объекта enrollmentConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8fe867edace02c5b1735783491d9e760cf799dc3
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178320"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="4235c-103">Обновление объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4235c-103">Update enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="4235c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4235c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4235c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4235c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4235c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4235c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4235c-107">Обновление свойств объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4235c-107">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4235c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4235c-108">Prerequisites</span></span>
<span data-ttu-id="4235c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4235c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4235c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4235c-111">Permission type</span></span>|<span data-ttu-id="4235c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4235c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4235c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4235c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4235c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4235c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4235c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4235c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4235c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4235c-116">Not supported.</span></span>|
|<span data-ttu-id="4235c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4235c-117">Application</span></span>|<span data-ttu-id="4235c-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4235c-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4235c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4235c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4235c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4235c-120">Request headers</span></span>
|<span data-ttu-id="4235c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4235c-121">Header</span></span>|<span data-ttu-id="4235c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4235c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4235c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4235c-123">Authorization</span></span>|<span data-ttu-id="4235c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4235c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4235c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4235c-125">Accept</span></span>|<span data-ttu-id="4235c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4235c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4235c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4235c-127">Request body</span></span>
<span data-ttu-id="4235c-128">В теле запроса добавьте представление объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4235c-128">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="4235c-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4235c-129">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="4235c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4235c-130">Property</span></span>|<span data-ttu-id="4235c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4235c-131">Type</span></span>|<span data-ttu-id="4235c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4235c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4235c-133">id</span><span class="sxs-lookup"><span data-stu-id="4235c-133">id</span></span>|<span data-ttu-id="4235c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4235c-134">String</span></span>|<span data-ttu-id="4235c-135">Ключ назначения конфигурации регистрации</span><span class="sxs-lookup"><span data-stu-id="4235c-135">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="4235c-136">target</span><span class="sxs-lookup"><span data-stu-id="4235c-136">target</span></span>|[<span data-ttu-id="4235c-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4235c-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4235c-138">Представляет назначение управляемым устройствам в клиенте.</span><span class="sxs-lookup"><span data-stu-id="4235c-138">Represents an assignment to managed devices in the tenant</span></span>|
|<span data-ttu-id="4235c-139">source</span><span class="sxs-lookup"><span data-stu-id="4235c-139">source</span></span>|[<span data-ttu-id="4235c-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="4235c-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="4235c-141">Тип ресурса, используемого для развертывания, в группу, Direct или набор политик.</span><span class="sxs-lookup"><span data-stu-id="4235c-141">Type of resource used for deployment to a group, direct or policySet.</span></span> <span data-ttu-id="4235c-142">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="4235c-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="4235c-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="4235c-143">sourceId</span></span>|<span data-ttu-id="4235c-144">Строка</span><span class="sxs-lookup"><span data-stu-id="4235c-144">String</span></span>|<span data-ttu-id="4235c-145">Идентификатор ресурса, используемого для развертывания в группе</span><span class="sxs-lookup"><span data-stu-id="4235c-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="4235c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4235c-146">Response</span></span>
<span data-ttu-id="4235c-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4235c-147">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4235c-148">Пример</span><span class="sxs-lookup"><span data-stu-id="4235c-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="4235c-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="4235c-149">Request</span></span>
<span data-ttu-id="4235c-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4235c-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="4235c-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="4235c-151">Response</span></span>
<span data-ttu-id="4235c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4235c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



