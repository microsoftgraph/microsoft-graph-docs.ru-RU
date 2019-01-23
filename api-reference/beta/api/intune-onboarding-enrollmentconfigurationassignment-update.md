---
title: Обновление объекта enrollmentConfigurationAssignment
description: Обновление свойств объекта enrollmentConfigurationAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 928abb0869a401015a6485e240d5ebd2336a7d3f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403604"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="7ec49-103">Обновление объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="7ec49-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="7ec49-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7ec49-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7ec49-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ec49-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ec49-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ec49-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ec49-107">Обновление свойств объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7ec49-107">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ec49-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7ec49-108">Prerequisites</span></span>
<span data-ttu-id="7ec49-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7ec49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7ec49-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ec49-111">Permission type</span></span>|<span data-ttu-id="7ec49-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ec49-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ec49-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ec49-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7ec49-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ec49-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7ec49-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ec49-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ec49-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ec49-116">Not supported.</span></span>|
|<span data-ttu-id="7ec49-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ec49-117">Application</span></span>|<span data-ttu-id="7ec49-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ec49-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ec49-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ec49-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7ec49-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ec49-120">Request headers</span></span>
|<span data-ttu-id="7ec49-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ec49-121">Header</span></span>|<span data-ttu-id="7ec49-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7ec49-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ec49-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ec49-123">Authorization</span></span>|<span data-ttu-id="7ec49-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7ec49-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ec49-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7ec49-125">Accept</span></span>|<span data-ttu-id="7ec49-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7ec49-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ec49-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ec49-127">Request body</span></span>
<span data-ttu-id="7ec49-128">В теле запроса добавьте представление объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ec49-128">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="7ec49-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7ec49-129">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="7ec49-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ec49-130">Property</span></span>|<span data-ttu-id="7ec49-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7ec49-131">Type</span></span>|<span data-ttu-id="7ec49-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7ec49-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ec49-133">id</span><span class="sxs-lookup"><span data-stu-id="7ec49-133">id</span></span>|<span data-ttu-id="7ec49-134">String</span><span class="sxs-lookup"><span data-stu-id="7ec49-134">String</span></span>|<span data-ttu-id="7ec49-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7ec49-135">Not yet documented</span></span>|
|<span data-ttu-id="7ec49-136">target</span><span class="sxs-lookup"><span data-stu-id="7ec49-136">target</span></span>|[<span data-ttu-id="7ec49-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7ec49-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7ec49-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7ec49-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7ec49-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ec49-139">Response</span></span>
<span data-ttu-id="7ec49-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7ec49-140">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ec49-141">Пример</span><span class="sxs-lookup"><span data-stu-id="7ec49-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ec49-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ec49-142">Request</span></span>
<span data-ttu-id="7ec49-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ec49-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7ec49-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ec49-144">Response</span></span>
<span data-ttu-id="7ec49-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7ec49-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




