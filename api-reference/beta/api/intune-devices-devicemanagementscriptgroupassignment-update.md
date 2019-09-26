---
title: Обновление Девицеманажементскриптграупассигнмент
description: Обновление свойств объекта Девицеманажементскриптграупассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 25edfdba027d045fe36f1971eccbade0f0a8cf20
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37180477"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="9d3f7-103">Обновление Девицеманажементскриптграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="9d3f7-103">Update deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="9d3f7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d3f7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d3f7-106">Обновление свойств объекта [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9d3f7-106">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d3f7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9d3f7-107">Prerequisites</span></span>
<span data-ttu-id="9d3f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d3f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d3f7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d3f7-110">Permission type</span></span>|<span data-ttu-id="9d3f7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d3f7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d3f7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d3f7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9d3f7-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d3f7-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9d3f7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d3f7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d3f7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-115">Not supported.</span></span>|
|<span data-ttu-id="9d3f7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d3f7-116">Application</span></span>|<span data-ttu-id="9d3f7-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d3f7-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d3f7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d3f7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9d3f7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d3f7-119">Request headers</span></span>
|<span data-ttu-id="9d3f7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d3f7-120">Header</span></span>|<span data-ttu-id="9d3f7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9d3f7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d3f7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d3f7-122">Authorization</span></span>|<span data-ttu-id="9d3f7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d3f7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9d3f7-124">Accept</span></span>|<span data-ttu-id="9d3f7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9d3f7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d3f7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9d3f7-126">Request body</span></span>
<span data-ttu-id="9d3f7-127">В тексте запроса добавьте представление объекта [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-127">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="9d3f7-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9d3f7-128">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="9d3f7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d3f7-129">Property</span></span>|<span data-ttu-id="9d3f7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9d3f7-130">Type</span></span>|<span data-ttu-id="9d3f7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9d3f7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d3f7-132">id</span><span class="sxs-lookup"><span data-stu-id="9d3f7-132">id</span></span>|<span data-ttu-id="9d3f7-133">String</span><span class="sxs-lookup"><span data-stu-id="9d3f7-133">String</span></span>|<span data-ttu-id="9d3f7-134">Ключ объекта назначения группы сценариев управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-134">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="9d3f7-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-135">This property is read-only.</span></span>|
|<span data-ttu-id="9d3f7-136">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="9d3f7-136">targetGroupId</span></span>|<span data-ttu-id="9d3f7-137">String.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-137">String</span></span>|<span data-ttu-id="9d3f7-138">Идентификатор группы Azure Active Directory, на которую ориентирован сценарий.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="9d3f7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d3f7-139">Response</span></span>
<span data-ttu-id="9d3f7-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d3f7-141">Пример</span><span class="sxs-lookup"><span data-stu-id="9d3f7-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d3f7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d3f7-142">Request</span></span>
<span data-ttu-id="9d3f7-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="9d3f7-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d3f7-144">Response</span></span>
<span data-ttu-id="9d3f7-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d3f7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




