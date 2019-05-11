---
title: Создание объекта enrollmentConfigurationAssignment
description: Создание объекта enrollmentConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16a316a0f6c06080c3962749242ed01073dc23f7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900049"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="a57be-103">Создание объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a57be-103">Create enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="a57be-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a57be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a57be-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a57be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a57be-106">Создание объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a57be-106">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a57be-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a57be-107">Prerequisites</span></span>
<span data-ttu-id="a57be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a57be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a57be-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a57be-110">Permission type</span></span>|<span data-ttu-id="a57be-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a57be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a57be-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a57be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a57be-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a57be-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a57be-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a57be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a57be-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a57be-115">Not supported.</span></span>|
|<span data-ttu-id="a57be-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a57be-116">Application</span></span>|<span data-ttu-id="a57be-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a57be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a57be-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a57be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a57be-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a57be-119">Request headers</span></span>
|<span data-ttu-id="a57be-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a57be-120">Header</span></span>|<span data-ttu-id="a57be-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a57be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a57be-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a57be-122">Authorization</span></span>|<span data-ttu-id="a57be-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a57be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a57be-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a57be-124">Accept</span></span>|<span data-ttu-id="a57be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a57be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a57be-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a57be-126">Request body</span></span>
<span data-ttu-id="a57be-127">В теле запроса добавьте представление объекта enrollmentConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a57be-127">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="a57be-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта enrollmentConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="a57be-128">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="a57be-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a57be-129">Property</span></span>|<span data-ttu-id="a57be-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a57be-130">Type</span></span>|<span data-ttu-id="a57be-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a57be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a57be-132">id</span><span class="sxs-lookup"><span data-stu-id="a57be-132">id</span></span>|<span data-ttu-id="a57be-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a57be-133">String</span></span>|<span data-ttu-id="a57be-134">Ключ назначения конфигурации регистрации</span><span class="sxs-lookup"><span data-stu-id="a57be-134">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="a57be-135">target</span><span class="sxs-lookup"><span data-stu-id="a57be-135">target</span></span>|[<span data-ttu-id="a57be-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a57be-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a57be-137">Представляет назначение управляемым устройствам в клиенте.</span><span class="sxs-lookup"><span data-stu-id="a57be-137">Represents an assignment to managed devices in the tenant</span></span>|



## <a name="response"></a><span data-ttu-id="a57be-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a57be-138">Response</span></span>
<span data-ttu-id="a57be-139">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a57be-139">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a57be-140">Пример</span><span class="sxs-lookup"><span data-stu-id="a57be-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a57be-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a57be-141">Request</span></span>
<span data-ttu-id="a57be-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a57be-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a57be-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a57be-143">Response</span></span>
<span data-ttu-id="a57be-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a57be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




