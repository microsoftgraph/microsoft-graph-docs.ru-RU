---
title: Создание appleEnrollmentProfileAssignment
description: Создание объекта appleEnrollmentProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: abbe00b85784e06596e5a93fa4eeb858ff6549bc
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161182"
---
# <a name="create-appleenrollmentprofileassignment"></a><span data-ttu-id="7c4f2-103">Создание appleEnrollmentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="7c4f2-103">Create appleEnrollmentProfileAssignment</span></span>

<span data-ttu-id="7c4f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c4f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c4f2-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c4f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c4f2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c4f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c4f2-107">Создание объекта [appleEnrollmentProfileAssignment.](../resources/intune-enrollment-appleenrollmentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7c4f2-107">Create a new [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c4f2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7c4f2-108">Prerequisites</span></span>
<span data-ttu-id="7c4f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c4f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c4f2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c4f2-111">Permission type</span></span>|<span data-ttu-id="7c4f2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c4f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c4f2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c4f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c4f2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c4f2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7c4f2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c4f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c4f2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c4f2-116">Not supported.</span></span>|
|<span data-ttu-id="7c4f2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c4f2-117">Application</span></span>|<span data-ttu-id="7c4f2-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c4f2-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c4f2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c4f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7c4f2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7c4f2-120">Request headers</span></span>
|<span data-ttu-id="7c4f2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c4f2-121">Header</span></span>|<span data-ttu-id="7c4f2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7c4f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c4f2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c4f2-123">Authorization</span></span>|<span data-ttu-id="7c4f2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c4f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c4f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7c4f2-125">Accept</span></span>|<span data-ttu-id="7c4f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c4f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c4f2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c4f2-127">Request body</span></span>
<span data-ttu-id="7c4f2-128">В теле запроса укажу представление объекта appleEnrollmentProfileAssignment в JSON.</span><span class="sxs-lookup"><span data-stu-id="7c4f2-128">In the request body, supply a JSON representation for the appleEnrollmentProfileAssignment object.</span></span>

<span data-ttu-id="7c4f2-129">В следующей таблице показаны свойства, необходимые при создании объекта appleEnrollmentProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="7c4f2-129">The following table shows the properties that are required when you create the appleEnrollmentProfileAssignment.</span></span>

|<span data-ttu-id="7c4f2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c4f2-130">Property</span></span>|<span data-ttu-id="7c4f2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7c4f2-131">Type</span></span>|<span data-ttu-id="7c4f2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7c4f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c4f2-133">id</span><span class="sxs-lookup"><span data-stu-id="7c4f2-133">id</span></span>|<span data-ttu-id="7c4f2-134">String</span><span class="sxs-lookup"><span data-stu-id="7c4f2-134">String</span></span>|<span data-ttu-id="7c4f2-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="7c4f2-135">The key of the assignment.</span></span>|
|<span data-ttu-id="7c4f2-136">target</span><span class="sxs-lookup"><span data-stu-id="7c4f2-136">target</span></span>|[<span data-ttu-id="7c4f2-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7c4f2-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7c4f2-138">Целевой объект назначения для профиля развертывания, инициированного пользователем Apple.</span><span class="sxs-lookup"><span data-stu-id="7c4f2-138">The assignment target for the Apple user initiated deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="7c4f2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c4f2-139">Response</span></span>
<span data-ttu-id="7c4f2-140">В случае успешного выполнения этот метод возвращает код отклика и объект `201 Created` [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7c4f2-140">If successful, this method returns a `201 Created` response code and a [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c4f2-141">Пример</span><span class="sxs-lookup"><span data-stu-id="7c4f2-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c4f2-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c4f2-142">Request</span></span>
<span data-ttu-id="7c4f2-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c4f2-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
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

### <a name="response"></a><span data-ttu-id="7c4f2-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c4f2-144">Response</span></span>
<span data-ttu-id="7c4f2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c4f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




