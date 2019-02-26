---
title: Обновление объекта enrollmentConfigurationAssignment
description: Обновление свойств объекта enrollmentConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d33fb62ec3b476717c535e26de02d68a4bda098
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160538"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="ff7c2-103">Обновление объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ff7c2-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="ff7c2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff7c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff7c2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff7c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff7c2-106">Обновление свойств объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff7c2-106">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff7c2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ff7c2-107">Prerequisites</span></span>
<span data-ttu-id="ff7c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ff7c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ff7c2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff7c2-110">Permission type</span></span>|<span data-ttu-id="ff7c2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff7c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff7c2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff7c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ff7c2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff7c2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ff7c2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff7c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff7c2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff7c2-115">Not supported.</span></span>|
|<span data-ttu-id="ff7c2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff7c2-116">Application</span></span>|<span data-ttu-id="ff7c2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff7c2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff7c2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff7c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ff7c2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff7c2-119">Request headers</span></span>
|<span data-ttu-id="ff7c2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff7c2-120">Header</span></span>|<span data-ttu-id="ff7c2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ff7c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff7c2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff7c2-122">Authorization</span></span>|<span data-ttu-id="ff7c2-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ff7c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff7c2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ff7c2-124">Accept</span></span>|<span data-ttu-id="ff7c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ff7c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff7c2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ff7c2-126">Request body</span></span>
<span data-ttu-id="ff7c2-127">В теле запроса добавьте представление объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff7c2-127">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="ff7c2-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff7c2-128">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="ff7c2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff7c2-129">Property</span></span>|<span data-ttu-id="ff7c2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ff7c2-130">Type</span></span>|<span data-ttu-id="ff7c2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ff7c2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff7c2-132">id</span><span class="sxs-lookup"><span data-stu-id="ff7c2-132">id</span></span>|<span data-ttu-id="ff7c2-133">String</span><span class="sxs-lookup"><span data-stu-id="ff7c2-133">String</span></span>|<span data-ttu-id="ff7c2-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ff7c2-134">Not yet documented</span></span>|
|<span data-ttu-id="ff7c2-135">target</span><span class="sxs-lookup"><span data-stu-id="ff7c2-135">target</span></span>|[<span data-ttu-id="ff7c2-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ff7c2-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ff7c2-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ff7c2-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ff7c2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff7c2-138">Response</span></span>
<span data-ttu-id="ff7c2-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ff7c2-139">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff7c2-140">Пример</span><span class="sxs-lookup"><span data-stu-id="ff7c2-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff7c2-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff7c2-141">Request</span></span>
<span data-ttu-id="ff7c2-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff7c2-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ff7c2-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff7c2-143">Response</span></span>
<span data-ttu-id="ff7c2-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ff7c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




