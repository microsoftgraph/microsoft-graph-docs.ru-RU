---
title: Создание объекта enrollmentConfigurationAssignment
description: Создание объекта enrollmentConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 55d17ee41ad4ba6a6198398d2ac87357d9201552
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758012"
---
# <a name="create-enrollmentconfigurationassignment"></a><span data-ttu-id="1769c-103">Создание объекта enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1769c-103">Create enrollmentConfigurationAssignment</span></span>

<span data-ttu-id="1769c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1769c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1769c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1769c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1769c-106">Создание объекта [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1769c-106">Create a new [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1769c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1769c-107">Prerequisites</span></span>
<span data-ttu-id="1769c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1769c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1769c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1769c-110">Permission type</span></span>|<span data-ttu-id="1769c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1769c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1769c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1769c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1769c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1769c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1769c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1769c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1769c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1769c-115">Not supported.</span></span>|
|<span data-ttu-id="1769c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1769c-116">Application</span></span>|<span data-ttu-id="1769c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1769c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1769c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1769c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1769c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1769c-119">Request headers</span></span>
|<span data-ttu-id="1769c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1769c-120">Header</span></span>|<span data-ttu-id="1769c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1769c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1769c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1769c-122">Authorization</span></span>|<span data-ttu-id="1769c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1769c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1769c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1769c-124">Accept</span></span>|<span data-ttu-id="1769c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1769c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1769c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1769c-126">Request body</span></span>
<span data-ttu-id="1769c-127">В теле запроса добавьте представление объекта enrollmentConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1769c-127">In the request body, supply a JSON representation for the enrollmentConfigurationAssignment object.</span></span>

<span data-ttu-id="1769c-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта enrollmentConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="1769c-128">The following table shows the properties that are required when you create the enrollmentConfigurationAssignment.</span></span>

|<span data-ttu-id="1769c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1769c-129">Property</span></span>|<span data-ttu-id="1769c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1769c-130">Type</span></span>|<span data-ttu-id="1769c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1769c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1769c-132">id</span><span class="sxs-lookup"><span data-stu-id="1769c-132">id</span></span>|<span data-ttu-id="1769c-133">String</span><span class="sxs-lookup"><span data-stu-id="1769c-133">String</span></span>|<span data-ttu-id="1769c-134">Ключ назначения конфигурации регистрации</span><span class="sxs-lookup"><span data-stu-id="1769c-134">Key of the enrollment configuration assignment</span></span>|
|<span data-ttu-id="1769c-135">target</span><span class="sxs-lookup"><span data-stu-id="1769c-135">target</span></span>|[<span data-ttu-id="1769c-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1769c-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1769c-137">Представляет назначение управляемым устройствам в клиенте</span><span class="sxs-lookup"><span data-stu-id="1769c-137">Represents an assignment to managed devices in the tenant</span></span>|



## <a name="response"></a><span data-ttu-id="1769c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1769c-138">Response</span></span>
<span data-ttu-id="1769c-139">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1769c-139">If successful, this method returns a `201 Created` response code and a [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1769c-140">Пример</span><span class="sxs-lookup"><span data-stu-id="1769c-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="1769c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="1769c-141">Request</span></span>
<span data-ttu-id="1769c-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1769c-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
Content-type: application/json
Content-length: 225

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="1769c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="1769c-143">Response</span></span>
<span data-ttu-id="1769c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1769c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 274

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "collectionId": "Collection Id value"
  }
}
```




