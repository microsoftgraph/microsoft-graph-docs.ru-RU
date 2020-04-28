---
title: Создание Девицеманажементскриптграупассигнмент
description: Создание нового объекта Девицеманажементскриптграупассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d78dfba82625f21defc51fcbc0920e6509eef945
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43380455"
---
# <a name="create-devicemanagementscriptgroupassignment"></a><span data-ttu-id="33f22-103">Создание Девицеманажементскриптграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="33f22-103">Create deviceManagementScriptGroupAssignment</span></span>

<span data-ttu-id="33f22-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33f22-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33f22-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33f22-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33f22-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33f22-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33f22-107">Создание нового объекта [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="33f22-107">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33f22-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="33f22-108">Prerequisites</span></span>
<span data-ttu-id="33f22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33f22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33f22-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33f22-111">Permission type</span></span>|<span data-ttu-id="33f22-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33f22-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33f22-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33f22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33f22-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33f22-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="33f22-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33f22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33f22-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33f22-116">Not supported.</span></span>|
|<span data-ttu-id="33f22-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33f22-117">Application</span></span>|<span data-ttu-id="33f22-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33f22-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33f22-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33f22-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="33f22-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="33f22-120">Request headers</span></span>
|<span data-ttu-id="33f22-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33f22-121">Header</span></span>|<span data-ttu-id="33f22-122">Значение</span><span class="sxs-lookup"><span data-stu-id="33f22-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33f22-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33f22-123">Authorization</span></span>|<span data-ttu-id="33f22-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33f22-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33f22-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33f22-125">Accept</span></span>|<span data-ttu-id="33f22-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33f22-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33f22-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="33f22-127">Request body</span></span>
<span data-ttu-id="33f22-128">В тексте запроса добавьте представление объекта Девицеманажементскриптграупассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33f22-128">In the request body, supply a JSON representation for the deviceManagementScriptGroupAssignment object.</span></span>

<span data-ttu-id="33f22-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементскриптграупассигнмент.</span><span class="sxs-lookup"><span data-stu-id="33f22-129">The following table shows the properties that are required when you create the deviceManagementScriptGroupAssignment.</span></span>

|<span data-ttu-id="33f22-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="33f22-130">Property</span></span>|<span data-ttu-id="33f22-131">Тип</span><span class="sxs-lookup"><span data-stu-id="33f22-131">Type</span></span>|<span data-ttu-id="33f22-132">Описание</span><span class="sxs-lookup"><span data-stu-id="33f22-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33f22-133">id</span><span class="sxs-lookup"><span data-stu-id="33f22-133">id</span></span>|<span data-ttu-id="33f22-134">String</span><span class="sxs-lookup"><span data-stu-id="33f22-134">String</span></span>|<span data-ttu-id="33f22-135">Ключ объекта назначения группы сценариев управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="33f22-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="33f22-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="33f22-136">This property is read-only.</span></span>|
|<span data-ttu-id="33f22-137">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="33f22-137">targetGroupId</span></span>|<span data-ttu-id="33f22-138">String</span><span class="sxs-lookup"><span data-stu-id="33f22-138">String</span></span>|<span data-ttu-id="33f22-139">Идентификатор группы Azure Active Directory, на которую ориентирован сценарий.</span><span class="sxs-lookup"><span data-stu-id="33f22-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="33f22-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="33f22-140">Response</span></span>
<span data-ttu-id="33f22-141">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33f22-141">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33f22-142">Пример</span><span class="sxs-lookup"><span data-stu-id="33f22-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="33f22-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="33f22-143">Request</span></span>
<span data-ttu-id="33f22-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33f22-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/groupAssignments
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="33f22-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="33f22-145">Response</span></span>
<span data-ttu-id="33f22-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33f22-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



