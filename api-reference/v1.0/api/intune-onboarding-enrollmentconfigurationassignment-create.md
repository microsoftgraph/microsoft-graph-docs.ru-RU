---
title: Создание объекта enrollmentConfigurationAssignment
description: Создание объекта enrollmentConfigurationAssignment.
ms.openlocfilehash: 48afdefb08b9520a2ce4564bd0cc528bed7d0012
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025004"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="b8156-103">Создание объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b8156-103">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="b8156-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b8156-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8156-105">Создание объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b8156-105">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8156-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b8156-106">Prerequisites</span></span>
<span data-ttu-id="b8156-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8156-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8156-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8156-109">Permission type</span></span>|<span data-ttu-id="b8156-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8156-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8156-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8156-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8156-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8156-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b8156-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8156-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8156-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8156-114">Not supported.</span></span>|
|<span data-ttu-id="b8156-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8156-115">Application</span></span>|<span data-ttu-id="b8156-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8156-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8156-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8156-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b8156-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8156-118">Request headers</span></span>
|<span data-ttu-id="b8156-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8156-119">Header</span></span>|<span data-ttu-id="b8156-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b8156-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8156-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8156-121">Authorization</span></span>|<span data-ttu-id="b8156-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b8156-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8156-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b8156-123">Accept</span></span>|<span data-ttu-id="b8156-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b8156-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8156-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b8156-125">Request body</span></span>
<span data-ttu-id="b8156-126">В теле запроса добавьте представление объекта enrollmentConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8156-126">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="b8156-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта enrollmentConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="b8156-127">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="b8156-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8156-128">Property</span></span>|<span data-ttu-id="b8156-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b8156-129">Type</span></span>|<span data-ttu-id="b8156-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b8156-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8156-131">id</span><span class="sxs-lookup"><span data-stu-id="b8156-131">id</span></span>|<span data-ttu-id="b8156-132">String</span><span class="sxs-lookup"><span data-stu-id="b8156-132">String</span></span>|<span data-ttu-id="b8156-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b8156-133">Not yet documented</span></span>|
|<span data-ttu-id="b8156-134">target</span><span class="sxs-lookup"><span data-stu-id="b8156-134">target</span></span>|[<span data-ttu-id="b8156-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b8156-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b8156-136">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b8156-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b8156-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8156-137">Response</span></span>
<span data-ttu-id="b8156-138">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b8156-138">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8156-139">Пример</span><span class="sxs-lookup"><span data-stu-id="b8156-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8156-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8156-140">Request</span></span>
<span data-ttu-id="b8156-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8156-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b8156-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="b8156-142">Response</span></span>
<span data-ttu-id="b8156-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b8156-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



