---
title: Обновление deviceManagementScriptGroupAssignment
description: Обновление свойств объекта deviceManagementScriptGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3ec8b9e31d7e80bbc7f2733832aa5f75213a04fa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150404"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="179db-103">Обновление deviceManagementScriptGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="179db-103">Update deviceManagementScriptGroupAssignment</span></span>

<span data-ttu-id="179db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="179db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="179db-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="179db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="179db-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="179db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="179db-107">Обновление свойств объекта [deviceManagementScriptGroupAssignment.](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="179db-107">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="179db-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="179db-108">Prerequisites</span></span>
<span data-ttu-id="179db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="179db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="179db-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="179db-111">Permission type</span></span>|<span data-ttu-id="179db-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="179db-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="179db-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="179db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="179db-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="179db-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="179db-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="179db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="179db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="179db-116">Not supported.</span></span>|
|<span data-ttu-id="179db-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="179db-117">Application</span></span>|<span data-ttu-id="179db-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="179db-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="179db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="179db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="179db-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="179db-120">Request headers</span></span>
|<span data-ttu-id="179db-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="179db-121">Header</span></span>|<span data-ttu-id="179db-122">Значение</span><span class="sxs-lookup"><span data-stu-id="179db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="179db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="179db-123">Authorization</span></span>|<span data-ttu-id="179db-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="179db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="179db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="179db-125">Accept</span></span>|<span data-ttu-id="179db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="179db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="179db-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="179db-127">Request body</span></span>
<span data-ttu-id="179db-128">В теле запроса поставляем представление JSON для [объекта deviceManagementScriptGroupAssignment.](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="179db-128">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="179db-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementScriptGroupAssignment.](../resources/intune-devices-devicemanagementscriptgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="179db-129">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="179db-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="179db-130">Property</span></span>|<span data-ttu-id="179db-131">Тип</span><span class="sxs-lookup"><span data-stu-id="179db-131">Type</span></span>|<span data-ttu-id="179db-132">Описание</span><span class="sxs-lookup"><span data-stu-id="179db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="179db-133">id</span><span class="sxs-lookup"><span data-stu-id="179db-133">id</span></span>|<span data-ttu-id="179db-134">Строка</span><span class="sxs-lookup"><span data-stu-id="179db-134">String</span></span>|<span data-ttu-id="179db-135">Ключ объекта группового назначения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="179db-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="179db-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="179db-136">This property is read-only.</span></span>|
|<span data-ttu-id="179db-137">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="179db-137">targetGroupId</span></span>|<span data-ttu-id="179db-138">Строка</span><span class="sxs-lookup"><span data-stu-id="179db-138">String</span></span>|<span data-ttu-id="179db-139">Id группы Azure Active Directory, на который мы нацелены сценарий.</span><span class="sxs-lookup"><span data-stu-id="179db-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="179db-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="179db-140">Response</span></span>
<span data-ttu-id="179db-141">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="179db-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="179db-142">Пример</span><span class="sxs-lookup"><span data-stu-id="179db-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="179db-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="179db-143">Request</span></span>
<span data-ttu-id="179db-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="179db-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="179db-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="179db-145">Response</span></span>
<span data-ttu-id="179db-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="179db-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```




