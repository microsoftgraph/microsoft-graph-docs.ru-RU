---
title: Обновление Девицеманажементскриптграупассигнмент
description: Обновление свойств объекта Девицеманажементскриптграупассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23e3fdcf789b7e7f2a9a0602e46cf8ec0cd72a51
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48689624"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="24fda-103">Обновление Девицеманажементскриптграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="24fda-103">Update deviceManagementScriptGroupAssignment</span></span>

<span data-ttu-id="24fda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24fda-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24fda-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24fda-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24fda-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24fda-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24fda-107">Обновление свойств объекта [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="24fda-107">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24fda-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="24fda-108">Prerequisites</span></span>
<span data-ttu-id="24fda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24fda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24fda-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24fda-111">Permission type</span></span>|<span data-ttu-id="24fda-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24fda-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24fda-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24fda-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24fda-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24fda-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="24fda-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24fda-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24fda-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24fda-116">Not supported.</span></span>|
|<span data-ttu-id="24fda-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24fda-117">Application</span></span>|<span data-ttu-id="24fda-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24fda-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24fda-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24fda-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="24fda-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="24fda-120">Request headers</span></span>
|<span data-ttu-id="24fda-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24fda-121">Header</span></span>|<span data-ttu-id="24fda-122">Значение</span><span class="sxs-lookup"><span data-stu-id="24fda-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24fda-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24fda-123">Authorization</span></span>|<span data-ttu-id="24fda-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24fda-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24fda-125">Accept</span><span class="sxs-lookup"><span data-stu-id="24fda-125">Accept</span></span>|<span data-ttu-id="24fda-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24fda-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24fda-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="24fda-127">Request body</span></span>
<span data-ttu-id="24fda-128">В тексте запроса добавьте представление объекта [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24fda-128">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="24fda-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="24fda-129">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="24fda-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="24fda-130">Property</span></span>|<span data-ttu-id="24fda-131">Тип</span><span class="sxs-lookup"><span data-stu-id="24fda-131">Type</span></span>|<span data-ttu-id="24fda-132">Описание</span><span class="sxs-lookup"><span data-stu-id="24fda-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24fda-133">id</span><span class="sxs-lookup"><span data-stu-id="24fda-133">id</span></span>|<span data-ttu-id="24fda-134">Строка</span><span class="sxs-lookup"><span data-stu-id="24fda-134">String</span></span>|<span data-ttu-id="24fda-135">Ключ объекта назначения группы сценариев управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="24fda-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="24fda-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="24fda-136">This property is read-only.</span></span>|
|<span data-ttu-id="24fda-137">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="24fda-137">targetGroupId</span></span>|<span data-ttu-id="24fda-138">Строка</span><span class="sxs-lookup"><span data-stu-id="24fda-138">String</span></span>|<span data-ttu-id="24fda-139">Идентификатор группы Azure Active Directory, на которую ориентирован сценарий.</span><span class="sxs-lookup"><span data-stu-id="24fda-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="24fda-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="24fda-140">Response</span></span>
<span data-ttu-id="24fda-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24fda-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24fda-142">Пример</span><span class="sxs-lookup"><span data-stu-id="24fda-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="24fda-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="24fda-143">Request</span></span>
<span data-ttu-id="24fda-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24fda-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="24fda-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="24fda-145">Response</span></span>
<span data-ttu-id="24fda-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24fda-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





