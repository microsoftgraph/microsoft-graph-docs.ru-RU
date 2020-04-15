---
title: Обновление объекта enrollmentConfigurationAssignment
description: Обновление свойств объекта enrollmentConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f4a6d77ec5b4a68c0e074e686aece203aec0cd7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442382"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="bf932-103">Обновление объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="bf932-103">Update enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="bf932-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf932-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf932-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf932-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf932-106">Обновление свойств объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bf932-106">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf932-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bf932-107">Prerequisites</span></span>
<span data-ttu-id="bf932-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf932-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf932-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf932-110">Permission type</span></span>|<span data-ttu-id="bf932-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf932-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf932-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf932-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf932-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf932-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bf932-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf932-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf932-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf932-115">Not supported.</span></span>|
|<span data-ttu-id="bf932-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf932-116">Application</span></span>|<span data-ttu-id="bf932-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf932-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf932-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf932-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="bf932-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bf932-119">Request headers</span></span>
|<span data-ttu-id="bf932-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf932-120">Header</span></span>|<span data-ttu-id="bf932-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bf932-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf932-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf932-122">Authorization</span></span>|<span data-ttu-id="bf932-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf932-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf932-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bf932-124">Accept</span></span>|<span data-ttu-id="bf932-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf932-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf932-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bf932-126">Request body</span></span>
<span data-ttu-id="bf932-127">В теле запроса добавьте представление объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf932-127">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="bf932-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bf932-128">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="bf932-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf932-129">Property</span></span>|<span data-ttu-id="bf932-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bf932-130">Type</span></span>|<span data-ttu-id="bf932-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bf932-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf932-132">id</span><span class="sxs-lookup"><span data-stu-id="bf932-132">id</span></span>|<span data-ttu-id="bf932-133">String</span><span class="sxs-lookup"><span data-stu-id="bf932-133">String</span></span>|<span data-ttu-id="bf932-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="bf932-134">Not yet documented</span></span>|
|<span data-ttu-id="bf932-135">target</span><span class="sxs-lookup"><span data-stu-id="bf932-135">target</span></span>|[<span data-ttu-id="bf932-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bf932-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bf932-137">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="bf932-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bf932-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf932-138">Response</span></span>
<span data-ttu-id="bf932-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bf932-139">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf932-140">Пример</span><span class="sxs-lookup"><span data-stu-id="bf932-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf932-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf932-141">Request</span></span>
<span data-ttu-id="bf932-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf932-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="bf932-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf932-143">Response</span></span>
<span data-ttu-id="bf932-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf932-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```






