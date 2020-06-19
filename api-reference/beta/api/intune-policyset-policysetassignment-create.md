---
title: Создание Полицисетассигнмент
description: Создание нового объекта Полицисетассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b0c8a931a50b10f7694312bd618bdc20000299ca
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791716"
---
# <a name="create-policysetassignment"></a><span data-ttu-id="6015e-103">Создание Полицисетассигнмент</span><span class="sxs-lookup"><span data-stu-id="6015e-103">Create policySetAssignment</span></span>

<span data-ttu-id="6015e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6015e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6015e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6015e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6015e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6015e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6015e-107">Создание нового объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6015e-107">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6015e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6015e-108">Prerequisites</span></span>
<span data-ttu-id="6015e-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6015e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6015e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6015e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6015e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6015e-111">Permission type</span></span>|<span data-ttu-id="6015e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6015e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6015e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6015e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6015e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6015e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6015e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6015e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6015e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6015e-116">Not supported.</span></span>|
|<span data-ttu-id="6015e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6015e-117">Application</span></span>|<span data-ttu-id="6015e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6015e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6015e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6015e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6015e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6015e-120">Request headers</span></span>
|<span data-ttu-id="6015e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6015e-121">Header</span></span>|<span data-ttu-id="6015e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6015e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6015e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6015e-123">Authorization</span></span>|<span data-ttu-id="6015e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6015e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6015e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6015e-125">Accept</span></span>|<span data-ttu-id="6015e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6015e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6015e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6015e-127">Request body</span></span>
<span data-ttu-id="6015e-128">В тексте запроса добавьте представление объекта Полицисетассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6015e-128">In the request body, supply a JSON representation for the policySetAssignment object.</span></span>

<span data-ttu-id="6015e-129">В следующей таблице приведены свойства, необходимые при создании Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="6015e-129">The following table shows the properties that are required when you create the policySetAssignment.</span></span>

|<span data-ttu-id="6015e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6015e-130">Property</span></span>|<span data-ttu-id="6015e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6015e-131">Type</span></span>|<span data-ttu-id="6015e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6015e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6015e-133">id</span><span class="sxs-lookup"><span data-stu-id="6015e-133">id</span></span>|<span data-ttu-id="6015e-134">String</span><span class="sxs-lookup"><span data-stu-id="6015e-134">String</span></span>|<span data-ttu-id="6015e-135">Ключ Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="6015e-135">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="6015e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6015e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6015e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6015e-137">DateTimeOffset</span></span>|<span data-ttu-id="6015e-138">Время последнего изменения Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="6015e-138">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="6015e-139">target</span><span class="sxs-lookup"><span data-stu-id="6015e-139">target</span></span>|[<span data-ttu-id="6015e-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6015e-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6015e-141">Целевая группа Полицисетассигнмент</span><span class="sxs-lookup"><span data-stu-id="6015e-141">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="6015e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6015e-142">Response</span></span>
<span data-ttu-id="6015e-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6015e-143">If successful, this method returns a `201 Created` response code and a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6015e-144">Пример</span><span class="sxs-lookup"><span data-stu-id="6015e-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="6015e-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="6015e-145">Request</span></span>
<span data-ttu-id="6015e-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6015e-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="6015e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="6015e-147">Response</span></span>
<span data-ttu-id="6015e-148">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="6015e-148">Here is an example of the response.</span></span> <span data-ttu-id="6015e-149">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="6015e-149">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6015e-150">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="6015e-150">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 427

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



