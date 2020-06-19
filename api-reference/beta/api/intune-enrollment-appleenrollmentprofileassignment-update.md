---
title: Обновление Апплинроллментпрофилеассигнмент
description: Обновление свойств объекта Апплинроллментпрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a49f2f9a2685c50af76c39b47b774e274483cd2d
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792066"
---
# <a name="update-appleenrollmentprofileassignment"></a><span data-ttu-id="5fce5-103">Обновление Апплинроллментпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="5fce5-103">Update appleEnrollmentProfileAssignment</span></span>

<span data-ttu-id="5fce5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fce5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5fce5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fce5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5fce5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5fce5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fce5-107">Обновление свойств объекта [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5fce5-107">Update the properties of a [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fce5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5fce5-108">Prerequisites</span></span>
<span data-ttu-id="5fce5-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5fce5-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5fce5-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fce5-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fce5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5fce5-111">Permission type</span></span>|<span data-ttu-id="5fce5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5fce5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fce5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5fce5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5fce5-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fce5-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5fce5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5fce5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fce5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fce5-116">Not supported.</span></span>|
|<span data-ttu-id="5fce5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5fce5-117">Application</span></span>|<span data-ttu-id="5fce5-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fce5-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fce5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5fce5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="5fce5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5fce5-120">Request headers</span></span>
|<span data-ttu-id="5fce5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5fce5-121">Header</span></span>|<span data-ttu-id="5fce5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5fce5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fce5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5fce5-123">Authorization</span></span>|<span data-ttu-id="5fce5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5fce5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fce5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5fce5-125">Accept</span></span>|<span data-ttu-id="5fce5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5fce5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fce5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5fce5-127">Request body</span></span>
<span data-ttu-id="5fce5-128">В тексте запроса добавьте представление объекта [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fce5-128">In the request body, supply a JSON representation for the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object.</span></span>

<span data-ttu-id="5fce5-129">В следующей таблице приведены свойства, необходимые при создании [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5fce5-129">The following table shows the properties that are required when you create the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md).</span></span>

|<span data-ttu-id="5fce5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fce5-130">Property</span></span>|<span data-ttu-id="5fce5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5fce5-131">Type</span></span>|<span data-ttu-id="5fce5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5fce5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fce5-133">id</span><span class="sxs-lookup"><span data-stu-id="5fce5-133">id</span></span>|<span data-ttu-id="5fce5-134">String</span><span class="sxs-lookup"><span data-stu-id="5fce5-134">String</span></span>|<span data-ttu-id="5fce5-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="5fce5-135">The key of the assignment.</span></span>|
|<span data-ttu-id="5fce5-136">target</span><span class="sxs-lookup"><span data-stu-id="5fce5-136">target</span></span>|[<span data-ttu-id="5fce5-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5fce5-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5fce5-138">Цель назначения для профиля развертывания, инициированного пользователем Apple.</span><span class="sxs-lookup"><span data-stu-id="5fce5-138">The assignment target for the Apple user initiated deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="5fce5-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fce5-139">Response</span></span>
<span data-ttu-id="5fce5-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5fce5-140">If successful, this method returns a `200 OK` response code and an updated [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fce5-141">Пример</span><span class="sxs-lookup"><span data-stu-id="5fce5-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fce5-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="5fce5-142">Request</span></span>
<span data-ttu-id="5fce5-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5fce5-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments/{appleEnrollmentProfileAssignmentId}
Content-type: application/json
Content-length: 327

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="5fce5-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fce5-144">Response</span></span>
<span data-ttu-id="5fce5-145">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="5fce5-145">Here is an example of the response.</span></span> <span data-ttu-id="5fce5-146">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="5fce5-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5fce5-147">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5fce5-147">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
  "id": "5b603771-3771-5b60-7137-605b7137605b",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



