---
title: Создание Девицеманажементинтентассигнмент
description: Создание нового объекта Девицеманажементинтентассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 63eb168a175613fdca7c84559fcd5c368958c446
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792578"
---
# <a name="create-devicemanagementintentassignment"></a><span data-ttu-id="b6f0f-103">Создание Девицеманажементинтентассигнмент</span><span class="sxs-lookup"><span data-stu-id="b6f0f-103">Create deviceManagementIntentAssignment</span></span>

<span data-ttu-id="b6f0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6f0f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6f0f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6f0f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6f0f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6f0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6f0f-107">Создание нового объекта [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="b6f0f-107">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6f0f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b6f0f-108">Prerequisites</span></span>
<span data-ttu-id="b6f0f-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b6f0f-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b6f0f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6f0f-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6f0f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6f0f-111">Permission type</span></span>|<span data-ttu-id="b6f0f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6f0f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6f0f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6f0f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6f0f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6f0f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6f0f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6f0f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6f0f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6f0f-116">Not supported.</span></span>|
|<span data-ttu-id="b6f0f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6f0f-117">Application</span></span>|<span data-ttu-id="b6f0f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6f0f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6f0f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6f0f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b6f0f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b6f0f-120">Request headers</span></span>
|<span data-ttu-id="b6f0f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6f0f-121">Header</span></span>|<span data-ttu-id="b6f0f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b6f0f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6f0f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6f0f-123">Authorization</span></span>|<span data-ttu-id="b6f0f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6f0f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6f0f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6f0f-125">Accept</span></span>|<span data-ttu-id="b6f0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6f0f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6f0f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b6f0f-127">Request body</span></span>
<span data-ttu-id="b6f0f-128">В тексте запроса добавьте представление объекта Девицеманажементинтентассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6f0f-128">In the request body, supply a JSON representation for the deviceManagementIntentAssignment object.</span></span>

<span data-ttu-id="b6f0f-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтентассигнмент.</span><span class="sxs-lookup"><span data-stu-id="b6f0f-129">The following table shows the properties that are required when you create the deviceManagementIntentAssignment.</span></span>

|<span data-ttu-id="b6f0f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6f0f-130">Property</span></span>|<span data-ttu-id="b6f0f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b6f0f-131">Type</span></span>|<span data-ttu-id="b6f0f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b6f0f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6f0f-133">id</span><span class="sxs-lookup"><span data-stu-id="b6f0f-133">id</span></span>|<span data-ttu-id="b6f0f-134">String</span><span class="sxs-lookup"><span data-stu-id="b6f0f-134">String</span></span>|<span data-ttu-id="b6f0f-135">Идентификатор назначения</span><span class="sxs-lookup"><span data-stu-id="b6f0f-135">The assignment ID</span></span>|
|<span data-ttu-id="b6f0f-136">target</span><span class="sxs-lookup"><span data-stu-id="b6f0f-136">target</span></span>|[<span data-ttu-id="b6f0f-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b6f0f-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b6f0f-138">Цель назначения</span><span class="sxs-lookup"><span data-stu-id="b6f0f-138">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="b6f0f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6f0f-139">Response</span></span>
<span data-ttu-id="b6f0f-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b6f0f-140">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6f0f-141">Пример</span><span class="sxs-lookup"><span data-stu-id="b6f0f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6f0f-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6f0f-142">Request</span></span>
<span data-ttu-id="b6f0f-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6f0f-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments
Content-type: application/json
Content-length: 327

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="b6f0f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6f0f-144">Response</span></span>
<span data-ttu-id="b6f0f-145">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="b6f0f-145">Here is an example of the response.</span></span> <span data-ttu-id="b6f0f-146">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b6f0f-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b6f0f-147">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b6f0f-147">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 376

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



