---
title: Создание объекта enrollmentConfigurationAssignment
description: Создание объекта enrollmentConfigurationAssignment.
ms.openlocfilehash: 844415cb5e1b2a7160fdf08a992ffbd472d8e70c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080475"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="82196-103">Создание объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="82196-103">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="82196-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="82196-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82196-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82196-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82196-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="82196-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82196-107">Создание объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="82196-107">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82196-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="82196-108">Prerequisites</span></span>
<span data-ttu-id="82196-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82196-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82196-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82196-111">Permission type</span></span>|<span data-ttu-id="82196-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82196-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82196-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82196-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82196-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82196-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="82196-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82196-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82196-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82196-116">Not supported.</span></span>|
|<span data-ttu-id="82196-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82196-117">Application</span></span>|<span data-ttu-id="82196-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82196-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82196-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82196-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="82196-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82196-120">Request headers</span></span>
|<span data-ttu-id="82196-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82196-121">Header</span></span>|<span data-ttu-id="82196-122">Значение</span><span class="sxs-lookup"><span data-stu-id="82196-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82196-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="82196-123">Authorization</span></span>|<span data-ttu-id="82196-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="82196-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82196-125">Accept</span><span class="sxs-lookup"><span data-stu-id="82196-125">Accept</span></span>|<span data-ttu-id="82196-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82196-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82196-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="82196-127">Request body</span></span>
<span data-ttu-id="82196-128">В теле запроса добавьте представление объекта enrollmentConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82196-128">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="82196-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта enrollmentConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="82196-129">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="82196-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="82196-130">Property</span></span>|<span data-ttu-id="82196-131">Тип</span><span class="sxs-lookup"><span data-stu-id="82196-131">Type</span></span>|<span data-ttu-id="82196-132">Описание</span><span class="sxs-lookup"><span data-stu-id="82196-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82196-133">id</span><span class="sxs-lookup"><span data-stu-id="82196-133">id</span></span>|<span data-ttu-id="82196-134">String</span><span class="sxs-lookup"><span data-stu-id="82196-134">String</span></span>|<span data-ttu-id="82196-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="82196-135">Not yet documented</span></span>|
|<span data-ttu-id="82196-136">target</span><span class="sxs-lookup"><span data-stu-id="82196-136">target</span></span>|[<span data-ttu-id="82196-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="82196-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="82196-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="82196-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="82196-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="82196-139">Response</span></span>
<span data-ttu-id="82196-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="82196-140">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82196-141">Пример</span><span class="sxs-lookup"><span data-stu-id="82196-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="82196-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="82196-142">Request</span></span>
<span data-ttu-id="82196-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82196-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="82196-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="82196-144">Response</span></span>
<span data-ttu-id="82196-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="82196-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





