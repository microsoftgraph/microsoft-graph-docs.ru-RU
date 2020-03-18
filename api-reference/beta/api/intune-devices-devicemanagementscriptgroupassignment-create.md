---
title: Создание Девицеманажементскриптграупассигнмент
description: Создание нового объекта Девицеманажементскриптграупассигнмент.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7c6980fe83c3cb935139a5bac49f2a9883c5d4b8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42768557"
---
# <a name="create-devicemanagementscriptgroupassignment"></a><span data-ttu-id="75c2e-103">Создание Девицеманажементскриптграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="75c2e-103">Create deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="75c2e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75c2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75c2e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75c2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75c2e-106">Создание нового объекта [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="75c2e-106">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75c2e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="75c2e-107">Prerequisites</span></span>
<span data-ttu-id="75c2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75c2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75c2e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75c2e-110">Permission type</span></span>|<span data-ttu-id="75c2e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75c2e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75c2e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75c2e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75c2e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75c2e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="75c2e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75c2e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75c2e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75c2e-115">Not supported.</span></span>|
|<span data-ttu-id="75c2e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="75c2e-116">Application</span></span>|<span data-ttu-id="75c2e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75c2e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75c2e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75c2e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="75c2e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="75c2e-119">Request headers</span></span>
|<span data-ttu-id="75c2e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75c2e-120">Header</span></span>|<span data-ttu-id="75c2e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="75c2e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75c2e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="75c2e-122">Authorization</span></span>|<span data-ttu-id="75c2e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75c2e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75c2e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="75c2e-124">Accept</span></span>|<span data-ttu-id="75c2e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75c2e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75c2e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75c2e-126">Request body</span></span>
<span data-ttu-id="75c2e-127">В тексте запроса добавьте представление объекта Девицеманажементскриптграупассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75c2e-127">In the request body, supply a JSON representation for the deviceManagementScriptGroupAssignment object.</span></span>

<span data-ttu-id="75c2e-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементскриптграупассигнмент.</span><span class="sxs-lookup"><span data-stu-id="75c2e-128">The following table shows the properties that are required when you create the deviceManagementScriptGroupAssignment.</span></span>

|<span data-ttu-id="75c2e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="75c2e-129">Property</span></span>|<span data-ttu-id="75c2e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="75c2e-130">Type</span></span>|<span data-ttu-id="75c2e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="75c2e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75c2e-132">id</span><span class="sxs-lookup"><span data-stu-id="75c2e-132">id</span></span>|<span data-ttu-id="75c2e-133">String</span><span class="sxs-lookup"><span data-stu-id="75c2e-133">String</span></span>|<span data-ttu-id="75c2e-134">Ключ объекта назначения группы сценариев управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="75c2e-134">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="75c2e-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="75c2e-135">This property is read-only.</span></span>|
|<span data-ttu-id="75c2e-136">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="75c2e-136">targetGroupId</span></span>|<span data-ttu-id="75c2e-137">String</span><span class="sxs-lookup"><span data-stu-id="75c2e-137">String</span></span>|<span data-ttu-id="75c2e-138">Идентификатор группы Azure Active Directory, на которую ориентирован сценарий.</span><span class="sxs-lookup"><span data-stu-id="75c2e-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="75c2e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="75c2e-139">Response</span></span>
<span data-ttu-id="75c2e-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75c2e-140">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75c2e-141">Пример</span><span class="sxs-lookup"><span data-stu-id="75c2e-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="75c2e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="75c2e-142">Request</span></span>
<span data-ttu-id="75c2e-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75c2e-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="75c2e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="75c2e-144">Response</span></span>
<span data-ttu-id="75c2e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75c2e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```




