---
title: Создание Девицеманажементресаурцеакцесспрофилеассигнмент
description: Создание нового объекта Девицеманажементресаурцеакцесспрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1053da56d274206d7f050797350d8948d55fa7b3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302050"
---
# <a name="create-devicemanagementresourceaccessprofileassignment"></a><span data-ttu-id="8a3da-103">Создание Девицеманажементресаурцеакцесспрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="8a3da-103">Create deviceManagementResourceAccessProfileAssignment</span></span>

<span data-ttu-id="8a3da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a3da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a3da-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a3da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a3da-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a3da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a3da-107">Создание нового объекта [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="8a3da-107">Create a new [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a3da-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8a3da-108">Prerequisites</span></span>
<span data-ttu-id="8a3da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a3da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a3da-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a3da-111">Permission type</span></span>|<span data-ttu-id="8a3da-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a3da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a3da-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a3da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a3da-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a3da-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8a3da-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a3da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a3da-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a3da-116">Not supported.</span></span>|
|<span data-ttu-id="8a3da-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8a3da-117">Application</span></span>|<span data-ttu-id="8a3da-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a3da-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a3da-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a3da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8a3da-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8a3da-120">Request headers</span></span>
|<span data-ttu-id="8a3da-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a3da-121">Header</span></span>|<span data-ttu-id="8a3da-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8a3da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a3da-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a3da-123">Authorization</span></span>|<span data-ttu-id="8a3da-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a3da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a3da-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8a3da-125">Accept</span></span>|<span data-ttu-id="8a3da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a3da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a3da-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a3da-127">Request body</span></span>
<span data-ttu-id="8a3da-128">В тексте запроса добавьте представление объекта Девицеманажементресаурцеакцесспрофилеассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a3da-128">In the request body, supply a JSON representation for the deviceManagementResourceAccessProfileAssignment object.</span></span>

<span data-ttu-id="8a3da-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементресаурцеакцесспрофилеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="8a3da-129">The following table shows the properties that are required when you create the deviceManagementResourceAccessProfileAssignment.</span></span>

|<span data-ttu-id="8a3da-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a3da-130">Property</span></span>|<span data-ttu-id="8a3da-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8a3da-131">Type</span></span>|<span data-ttu-id="8a3da-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8a3da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a3da-133">id</span><span class="sxs-lookup"><span data-stu-id="8a3da-133">id</span></span>|<span data-ttu-id="8a3da-134">String</span><span class="sxs-lookup"><span data-stu-id="8a3da-134">String</span></span>|<span data-ttu-id="8a3da-135">Уникальный идентификатор для назначений</span><span class="sxs-lookup"><span data-stu-id="8a3da-135">Unique identifier for the Assignments</span></span>|
|<span data-ttu-id="8a3da-136">intent</span><span class="sxs-lookup"><span data-stu-id="8a3da-136">intent</span></span>|[<span data-ttu-id="8a3da-137">девицеманажементресаурцеакцесспрофилеинтент</span><span class="sxs-lookup"><span data-stu-id="8a3da-137">deviceManagementResourceAccessProfileIntent</span></span>](../resources/intune-rapolicy-devicemanagementresourceaccessprofileintent.md)|<span data-ttu-id="8a3da-138">Цель назначения для профиля доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="8a3da-138">The assignment intent for the resource access profile.</span></span> <span data-ttu-id="8a3da-139">Возможные значения: `apply`, `remove`.</span><span class="sxs-lookup"><span data-stu-id="8a3da-139">Possible values are: `apply`, `remove`.</span></span>|
|<span data-ttu-id="8a3da-140">target</span><span class="sxs-lookup"><span data-stu-id="8a3da-140">target</span></span>|[<span data-ttu-id="8a3da-141">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8a3da-141">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8a3da-142">Цель назначения для профиля доступа к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="8a3da-142">The assignment target for the resource access profile.</span></span>|
|<span data-ttu-id="8a3da-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="8a3da-143">sourceId</span></span>|<span data-ttu-id="8a3da-144">String</span><span class="sxs-lookup"><span data-stu-id="8a3da-144">String</span></span>|<span data-ttu-id="8a3da-145">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="8a3da-145">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="8a3da-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a3da-146">Response</span></span>
<span data-ttu-id="8a3da-147">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8a3da-147">If successful, this method returns a `201 Created` response code and a [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a3da-148">Пример</span><span class="sxs-lookup"><span data-stu-id="8a3da-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a3da-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a3da-149">Request</span></span>
<span data-ttu-id="8a3da-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a3da-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments
Content-type: application/json
Content-length: 399

{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
  "intent": "remove",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="8a3da-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a3da-151">Response</span></span>
<span data-ttu-id="8a3da-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a3da-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 448

{
  "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
  "id": "4ebb8d4e-8d4e-4ebb-4e8d-bb4e4e8dbb4e",
  "intent": "remove",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "sourceId": "Source Id value"
}
```




