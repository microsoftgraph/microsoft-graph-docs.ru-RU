---
title: Обновление объекта enrollmentConfigurationAssignment
description: Обновление свойств объекта enrollmentConfigurationAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9db69b7734012bc9d59fecca6d8103be1a97f24d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362297"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="7038d-103">Обновление объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="7038d-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="7038d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7038d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7038d-105">Обновление свойств объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7038d-105">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7038d-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7038d-106">Prerequisites</span></span>
<span data-ttu-id="7038d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7038d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7038d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7038d-109">Permission type</span></span>|<span data-ttu-id="7038d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7038d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7038d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7038d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7038d-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7038d-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7038d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7038d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7038d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7038d-114">Not supported.</span></span>|
|<span data-ttu-id="7038d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7038d-115">Application</span></span>|<span data-ttu-id="7038d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7038d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7038d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7038d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7038d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7038d-118">Request headers</span></span>
|<span data-ttu-id="7038d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7038d-119">Header</span></span>|<span data-ttu-id="7038d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7038d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7038d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7038d-121">Authorization</span></span>|<span data-ttu-id="7038d-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7038d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7038d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7038d-123">Accept</span></span>|<span data-ttu-id="7038d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7038d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7038d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7038d-125">Request body</span></span>
<span data-ttu-id="7038d-126">В теле запроса добавьте представление объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7038d-126">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="7038d-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7038d-127">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="7038d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7038d-128">Property</span></span>|<span data-ttu-id="7038d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7038d-129">Type</span></span>|<span data-ttu-id="7038d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7038d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7038d-131">id</span><span class="sxs-lookup"><span data-stu-id="7038d-131">id</span></span>|<span data-ttu-id="7038d-132">String</span><span class="sxs-lookup"><span data-stu-id="7038d-132">String</span></span>|<span data-ttu-id="7038d-133">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7038d-133">Not yet documented</span></span>|
|<span data-ttu-id="7038d-134">target</span><span class="sxs-lookup"><span data-stu-id="7038d-134">target</span></span>|[<span data-ttu-id="7038d-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7038d-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7038d-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7038d-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7038d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="7038d-137">Response</span></span>
<span data-ttu-id="7038d-138">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7038d-138">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7038d-139">Пример</span><span class="sxs-lookup"><span data-stu-id="7038d-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="7038d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="7038d-140">Request</span></span>
<span data-ttu-id="7038d-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7038d-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7038d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="7038d-142">Response</span></span>
<span data-ttu-id="7038d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7038d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




