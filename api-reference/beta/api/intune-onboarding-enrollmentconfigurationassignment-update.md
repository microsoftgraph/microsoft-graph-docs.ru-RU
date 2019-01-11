---
title: Обновление объекта enrollmentConfigurationAssignment
description: Обновление свойств объекта enrollmentConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8f4aba8c5e1cd6a392661e84d60cf11496ec39f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868105"
---
# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="e9d91-103">Обновление объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e9d91-103">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="e9d91-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e9d91-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9d91-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9d91-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9d91-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e9d91-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9d91-107">Обновление свойств объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e9d91-107">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e9d91-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e9d91-108">Prerequisites</span></span>
<span data-ttu-id="e9d91-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9d91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9d91-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9d91-111">Permission type</span></span>|<span data-ttu-id="e9d91-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9d91-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9d91-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9d91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9d91-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9d91-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e9d91-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9d91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9d91-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9d91-116">Not supported.</span></span>|
|<span data-ttu-id="e9d91-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9d91-117">Application</span></span>|<span data-ttu-id="e9d91-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9d91-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9d91-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9d91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e9d91-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9d91-120">Request headers</span></span>
|<span data-ttu-id="e9d91-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9d91-121">Header</span></span>|<span data-ttu-id="e9d91-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e9d91-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9d91-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9d91-123">Authorization</span></span>|<span data-ttu-id="e9d91-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e9d91-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9d91-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9d91-125">Accept</span></span>|<span data-ttu-id="e9d91-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9d91-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9d91-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9d91-127">Request body</span></span>
<span data-ttu-id="e9d91-128">В теле запроса добавьте представление объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9d91-128">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="e9d91-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e9d91-129">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="e9d91-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9d91-130">Property</span></span>|<span data-ttu-id="e9d91-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e9d91-131">Type</span></span>|<span data-ttu-id="e9d91-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e9d91-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9d91-133">id</span><span class="sxs-lookup"><span data-stu-id="e9d91-133">id</span></span>|<span data-ttu-id="e9d91-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e9d91-134">String</span></span>|<span data-ttu-id="e9d91-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e9d91-135">Not yet documented</span></span>|
|<span data-ttu-id="e9d91-136">target</span><span class="sxs-lookup"><span data-stu-id="e9d91-136">target</span></span>|[<span data-ttu-id="e9d91-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e9d91-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e9d91-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e9d91-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e9d91-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9d91-139">Response</span></span>
<span data-ttu-id="e9d91-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e9d91-140">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9d91-141">Пример</span><span class="sxs-lookup"><span data-stu-id="e9d91-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="e9d91-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9d91-142">Request</span></span>
<span data-ttu-id="e9d91-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9d91-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e9d91-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9d91-144">Response</span></span>
<span data-ttu-id="e9d91-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e9d91-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





