---
title: Обновление deviceManagementScriptAssignment
description: Обновление свойств объекта deviceManagementScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2f59afa720ead4e1e56b4f73b7ca49a205715318
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150495"
---
# <a name="update-devicemanagementscriptassignment"></a><span data-ttu-id="aff09-103">Обновление deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="aff09-103">Update deviceManagementScriptAssignment</span></span>

<span data-ttu-id="aff09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aff09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aff09-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aff09-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aff09-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aff09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aff09-107">Обновление свойств объекта [deviceManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="aff09-107">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aff09-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aff09-108">Prerequisites</span></span>
<span data-ttu-id="aff09-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aff09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aff09-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aff09-111">Permission type</span></span>|<span data-ttu-id="aff09-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aff09-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aff09-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aff09-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aff09-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aff09-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="aff09-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aff09-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aff09-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aff09-116">Not supported.</span></span>|
|<span data-ttu-id="aff09-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="aff09-117">Application</span></span>|<span data-ttu-id="aff09-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aff09-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aff09-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aff09-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="aff09-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="aff09-120">Request headers</span></span>
|<span data-ttu-id="aff09-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aff09-121">Header</span></span>|<span data-ttu-id="aff09-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aff09-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aff09-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aff09-123">Authorization</span></span>|<span data-ttu-id="aff09-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aff09-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aff09-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aff09-125">Accept</span></span>|<span data-ttu-id="aff09-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aff09-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aff09-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aff09-127">Request body</span></span>
<span data-ttu-id="aff09-128">В теле запроса поставляем представление JSON для [объекта deviceManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="aff09-128">In the request body, supply a JSON representation for the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

<span data-ttu-id="aff09-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="aff09-129">The following table shows the properties that are required when you create the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

|<span data-ttu-id="aff09-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="aff09-130">Property</span></span>|<span data-ttu-id="aff09-131">Тип</span><span class="sxs-lookup"><span data-stu-id="aff09-131">Type</span></span>|<span data-ttu-id="aff09-132">Описание</span><span class="sxs-lookup"><span data-stu-id="aff09-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aff09-133">id</span><span class="sxs-lookup"><span data-stu-id="aff09-133">id</span></span>|<span data-ttu-id="aff09-134">Строка</span><span class="sxs-lookup"><span data-stu-id="aff09-134">String</span></span>|<span data-ttu-id="aff09-135">Ключ объекта группового назначения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="aff09-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="aff09-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aff09-136">This property is read-only.</span></span>|
|<span data-ttu-id="aff09-137">target</span><span class="sxs-lookup"><span data-stu-id="aff09-137">target</span></span>|[<span data-ttu-id="aff09-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="aff09-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="aff09-139">Id группы Azure Active Directory, на который мы нацелены сценарий.</span><span class="sxs-lookup"><span data-stu-id="aff09-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="aff09-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="aff09-140">Response</span></span>
<span data-ttu-id="aff09-141">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="aff09-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aff09-142">Пример</span><span class="sxs-lookup"><span data-stu-id="aff09-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="aff09-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="aff09-143">Request</span></span>
<span data-ttu-id="aff09-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aff09-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="aff09-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="aff09-145">Response</span></span>
<span data-ttu-id="aff09-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aff09-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```




