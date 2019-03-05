---
title: Создание объекта enrollmentConfigurationAssignment
description: Создание объекта enrollmentConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b7043b3a30aa7dadf086b48024a71ed713e84257
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256058"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="5c36e-103">Создание объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="5c36e-103">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="5c36e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c36e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c36e-105">Создание объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5c36e-105">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c36e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5c36e-106">Prerequisites</span></span>
<span data-ttu-id="5c36e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5c36e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5c36e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c36e-109">Permission type</span></span>|<span data-ttu-id="5c36e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c36e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c36e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c36e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c36e-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c36e-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5c36e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c36e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c36e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c36e-114">Not supported.</span></span>|
|<span data-ttu-id="5c36e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c36e-115">Application</span></span>|<span data-ttu-id="5c36e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c36e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c36e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c36e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="5c36e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c36e-118">Request headers</span></span>
|<span data-ttu-id="5c36e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c36e-119">Header</span></span>|<span data-ttu-id="5c36e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5c36e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c36e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c36e-121">Authorization</span></span>|<span data-ttu-id="5c36e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5c36e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c36e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5c36e-123">Accept</span></span>|<span data-ttu-id="5c36e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5c36e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c36e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c36e-125">Request body</span></span>
<span data-ttu-id="5c36e-126">В теле запроса добавьте представление объекта enrollmentConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c36e-126">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="5c36e-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта enrollmentConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="5c36e-127">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="5c36e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c36e-128">Property</span></span>|<span data-ttu-id="5c36e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5c36e-129">Type</span></span>|<span data-ttu-id="5c36e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5c36e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c36e-131">id</span><span class="sxs-lookup"><span data-stu-id="5c36e-131">id</span></span>|<span data-ttu-id="5c36e-132">String</span><span class="sxs-lookup"><span data-stu-id="5c36e-132">String</span></span>|<span data-ttu-id="5c36e-133">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5c36e-133">Not yet documented</span></span>|
|<span data-ttu-id="5c36e-134">target</span><span class="sxs-lookup"><span data-stu-id="5c36e-134">target</span></span>|[<span data-ttu-id="5c36e-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5c36e-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5c36e-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5c36e-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5c36e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c36e-137">Response</span></span>
<span data-ttu-id="5c36e-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5c36e-138">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c36e-139">Пример</span><span class="sxs-lookup"><span data-stu-id="5c36e-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c36e-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c36e-140">Request</span></span>
<span data-ttu-id="5c36e-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c36e-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="5c36e-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c36e-142">Response</span></span>
<span data-ttu-id="5c36e-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c36e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



