---
title: Обновление Девицеманажементресаурцеакцесспрофилеассигнмент
description: Обновление свойств объекта Девицеманажементресаурцеакцесспрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 32f2a64c0e6b4db08182919514bf5eb14755fd3e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302338"
---
# <a name="update-devicemanagementresourceaccessprofileassignment"></a><span data-ttu-id="9f35e-103">Обновление Девицеманажементресаурцеакцесспрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="9f35e-103">Update deviceManagementResourceAccessProfileAssignment</span></span>

<span data-ttu-id="9f35e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f35e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f35e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f35e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f35e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f35e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f35e-107">Обновление свойств объекта [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9f35e-107">Update the properties of a [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f35e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f35e-108">Prerequisites</span></span>
<span data-ttu-id="9f35e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f35e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f35e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f35e-111">Permission type</span></span>|<span data-ttu-id="9f35e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f35e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f35e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f35e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f35e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f35e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9f35e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f35e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f35e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f35e-116">Not supported.</span></span>|
|<span data-ttu-id="9f35e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f35e-117">Application</span></span>|<span data-ttu-id="9f35e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f35e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f35e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f35e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments/{deviceManagementResourceAccessProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9f35e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9f35e-120">Request headers</span></span>
|<span data-ttu-id="9f35e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f35e-121">Header</span></span>|<span data-ttu-id="9f35e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9f35e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f35e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f35e-123">Authorization</span></span>|<span data-ttu-id="9f35e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f35e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f35e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9f35e-125">Accept</span></span>|<span data-ttu-id="9f35e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f35e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f35e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f35e-127">Request body</span></span>
<span data-ttu-id="9f35e-128">В тексте запроса добавьте представление объекта [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f35e-128">In the request body, supply a JSON representation for the [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object.</span></span>

<span data-ttu-id="9f35e-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9f35e-129">The following table shows the properties that are required when you create the [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md).</span></span>

|<span data-ttu-id="9f35e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f35e-130">Property</span></span>|<span data-ttu-id="9f35e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9f35e-131">Type</span></span>|<span data-ttu-id="9f35e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9f35e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f35e-133">id</span><span class="sxs-lookup"><span data-stu-id="9f35e-133">id</span></span>|<span data-ttu-id="9f35e-134">String</span><span class="sxs-lookup"><span data-stu-id="9f35e-134">String</span></span>|<span data-ttu-id="9f35e-135">Уникальный идентификатор для назначений</span><span class="sxs-lookup"><span data-stu-id="9f35e-135">Unique identifier for the Assignments</span></span>|
|<span data-ttu-id="9f35e-136">intent</span><span class="sxs-lookup"><span data-stu-id="9f35e-136">intent</span></span>|[<span data-ttu-id="9f35e-137">девицеманажементресаурцеакцесспрофилеинтент</span><span class="sxs-lookup"><span data-stu-id="9f35e-137">deviceManagementResourceAccessProfileIntent</span></span>](../resources/intune-rapolicy-devicemanagementresourceaccessprofileintent.md)|<span data-ttu-id="9f35e-138">Цель назначения для профиля доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="9f35e-138">The assignment intent for the resource access profile.</span></span> <span data-ttu-id="9f35e-139">Возможные значения: `apply`, `remove`.</span><span class="sxs-lookup"><span data-stu-id="9f35e-139">Possible values are: `apply`, `remove`.</span></span>|
|<span data-ttu-id="9f35e-140">target</span><span class="sxs-lookup"><span data-stu-id="9f35e-140">target</span></span>|[<span data-ttu-id="9f35e-141">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9f35e-141">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9f35e-142">Цель назначения для профиля доступа к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="9f35e-142">The assignment target for the resource access profile.</span></span>|
|<span data-ttu-id="9f35e-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="9f35e-143">sourceId</span></span>|<span data-ttu-id="9f35e-144">String</span><span class="sxs-lookup"><span data-stu-id="9f35e-144">String</span></span>|<span data-ttu-id="9f35e-145">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="9f35e-145">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="9f35e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f35e-146">Response</span></span>
<span data-ttu-id="9f35e-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементресаурцеакцесспрофилеассигнмент](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f35e-147">If successful, this method returns a `200 OK` response code and an updated [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f35e-148">Пример</span><span class="sxs-lookup"><span data-stu-id="9f35e-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f35e-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f35e-149">Request</span></span>
<span data-ttu-id="9f35e-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f35e-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assignments/{deviceManagementResourceAccessProfileAssignmentId}
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

### <a name="response"></a><span data-ttu-id="9f35e-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f35e-151">Response</span></span>
<span data-ttu-id="9f35e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f35e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




