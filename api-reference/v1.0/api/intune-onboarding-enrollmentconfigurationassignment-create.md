---
title: Создание объекта enrollmentConfigurationAssignment
description: Создание объекта enrollmentConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a999e3286881d3e736904ed9c8e722aa78d28204
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582782"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="d02b1-103">Создание объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d02b1-103">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="d02b1-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d02b1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d02b1-105">Создание объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d02b1-105">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d02b1-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d02b1-106">Prerequisites</span></span>
<span data-ttu-id="d02b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d02b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d02b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d02b1-109">Permission type</span></span>|<span data-ttu-id="d02b1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d02b1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d02b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d02b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d02b1-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d02b1-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d02b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d02b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d02b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d02b1-114">Not supported.</span></span>|
|<span data-ttu-id="d02b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d02b1-115">Application</span></span>|<span data-ttu-id="d02b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d02b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d02b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d02b1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d02b1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d02b1-118">Request headers</span></span>
|<span data-ttu-id="d02b1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d02b1-119">Header</span></span>|<span data-ttu-id="d02b1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d02b1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d02b1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d02b1-121">Authorization</span></span>|<span data-ttu-id="d02b1-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d02b1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d02b1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d02b1-123">Accept</span></span>|<span data-ttu-id="d02b1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d02b1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d02b1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d02b1-125">Request body</span></span>
<span data-ttu-id="d02b1-126">В теле запроса добавьте представление объекта enrollmentConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d02b1-126">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="d02b1-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта enrollmentConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="d02b1-127">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="d02b1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d02b1-128">Property</span></span>|<span data-ttu-id="d02b1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d02b1-129">Type</span></span>|<span data-ttu-id="d02b1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d02b1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d02b1-131">id</span><span class="sxs-lookup"><span data-stu-id="d02b1-131">id</span></span>|<span data-ttu-id="d02b1-132">String</span><span class="sxs-lookup"><span data-stu-id="d02b1-132">String</span></span>|<span data-ttu-id="d02b1-133">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d02b1-133">Not yet documented</span></span>|
|<span data-ttu-id="d02b1-134">target</span><span class="sxs-lookup"><span data-stu-id="d02b1-134">target</span></span>|[<span data-ttu-id="d02b1-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d02b1-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d02b1-136">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d02b1-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d02b1-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d02b1-137">Response</span></span>
<span data-ttu-id="d02b1-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d02b1-138">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d02b1-139">Пример</span><span class="sxs-lookup"><span data-stu-id="d02b1-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="d02b1-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="d02b1-140">Request</span></span>
<span data-ttu-id="d02b1-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d02b1-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d02b1-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d02b1-142">Response</span></span>
<span data-ttu-id="d02b1-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d02b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



