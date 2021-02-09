---
title: Обновление appleEnrollmentProfileAssignment
description: Обновление свойств объекта appleEnrollmentProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f10a0d383f0fe0475a7178b3f3a97b07eded50a4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159964"
---
# <a name="update-appleenrollmentprofileassignment"></a><span data-ttu-id="63dc9-103">Обновление appleEnrollmentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="63dc9-103">Update appleEnrollmentProfileAssignment</span></span>

<span data-ttu-id="63dc9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63dc9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63dc9-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63dc9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63dc9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63dc9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63dc9-107">Обновление свойств объекта [appleEnrollmentProfileAssignment.](../resources/intune-enrollment-appleenrollmentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="63dc9-107">Update the properties of a [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63dc9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="63dc9-108">Prerequisites</span></span>
<span data-ttu-id="63dc9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63dc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63dc9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63dc9-111">Permission type</span></span>|<span data-ttu-id="63dc9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="63dc9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63dc9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63dc9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63dc9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63dc9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="63dc9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63dc9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63dc9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63dc9-116">Not supported.</span></span>|
|<span data-ttu-id="63dc9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63dc9-117">Application</span></span>|<span data-ttu-id="63dc9-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63dc9-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63dc9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63dc9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="63dc9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="63dc9-120">Request headers</span></span>
|<span data-ttu-id="63dc9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63dc9-121">Header</span></span>|<span data-ttu-id="63dc9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="63dc9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63dc9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63dc9-123">Authorization</span></span>|<span data-ttu-id="63dc9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63dc9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63dc9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63dc9-125">Accept</span></span>|<span data-ttu-id="63dc9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63dc9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63dc9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63dc9-127">Request body</span></span>
<span data-ttu-id="63dc9-128">В теле запроса укажу представление объекта [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="63dc9-128">In the request body, supply a JSON representation for the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

<span data-ttu-id="63dc9-129">В следующей таблице показаны свойства, необходимые при создании [объекта appleEnrollmentProfileAssignment.](../resources/intune-enrollment-appleenrollmentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="63dc9-129">The following table shows the properties that are required when you create the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md).</span></span>

|<span data-ttu-id="63dc9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="63dc9-130">Property</span></span>|<span data-ttu-id="63dc9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="63dc9-131">Type</span></span>|<span data-ttu-id="63dc9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="63dc9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63dc9-133">id</span><span class="sxs-lookup"><span data-stu-id="63dc9-133">id</span></span>|<span data-ttu-id="63dc9-134">String</span><span class="sxs-lookup"><span data-stu-id="63dc9-134">String</span></span>|<span data-ttu-id="63dc9-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="63dc9-135">The key of the assignment.</span></span>|
|<span data-ttu-id="63dc9-136">target</span><span class="sxs-lookup"><span data-stu-id="63dc9-136">target</span></span>|[<span data-ttu-id="63dc9-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="63dc9-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="63dc9-138">Целевой объект назначения для профиля развертывания, инициированного пользователем Apple.</span><span class="sxs-lookup"><span data-stu-id="63dc9-138">The assignment target for the Apple user initiated deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="63dc9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="63dc9-139">Response</span></span>
<span data-ttu-id="63dc9-140">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="63dc9-140">If successful, this method returns a `200 OK` response code and an updated [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63dc9-141">Пример</span><span class="sxs-lookup"><span data-stu-id="63dc9-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="63dc9-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="63dc9-142">Request</span></span>
<span data-ttu-id="63dc9-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63dc9-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="63dc9-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="63dc9-144">Response</span></span>
<span data-ttu-id="63dc9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63dc9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "id": "5b603771-3771-5b60-7137-605b7137605b",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```




