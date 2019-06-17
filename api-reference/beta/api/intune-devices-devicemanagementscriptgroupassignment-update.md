---
title: Обновление Девицеманажементскриптграупассигнмент
description: Обновление свойств объекта Девицеманажементскриптграупассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 542967403d7e1a18576b8c665c1121be2b3c8f0a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958811"
---
# <a name="update-devicemanagementscriptgroupassignment"></a><span data-ttu-id="f9126-103">Обновление Девицеманажементскриптграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="f9126-103">Update deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="f9126-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9126-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9126-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9126-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9126-106">Обновление свойств объекта [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="f9126-106">Update the properties of a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9126-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f9126-107">Prerequisites</span></span>
<span data-ttu-id="f9126-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9126-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9126-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9126-110">Permission type</span></span>|<span data-ttu-id="f9126-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9126-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9126-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9126-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9126-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9126-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f9126-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9126-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9126-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9126-115">Not supported.</span></span>|
|<span data-ttu-id="f9126-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9126-116">Application</span></span>|<span data-ttu-id="f9126-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9126-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9126-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9126-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="f9126-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9126-119">Request headers</span></span>
|<span data-ttu-id="f9126-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9126-120">Header</span></span>|<span data-ttu-id="f9126-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f9126-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9126-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9126-122">Authorization</span></span>|<span data-ttu-id="f9126-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9126-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9126-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f9126-124">Accept</span></span>|<span data-ttu-id="f9126-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9126-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9126-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f9126-126">Request body</span></span>
<span data-ttu-id="f9126-127">В тексте запроса добавьте представление объекта [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9126-127">In the request body, supply a JSON representation for the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

<span data-ttu-id="f9126-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f9126-128">The following table shows the properties that are required when you create the [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).</span></span>

|<span data-ttu-id="f9126-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9126-129">Property</span></span>|<span data-ttu-id="f9126-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f9126-130">Type</span></span>|<span data-ttu-id="f9126-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f9126-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9126-132">id</span><span class="sxs-lookup"><span data-stu-id="f9126-132">id</span></span>|<span data-ttu-id="f9126-133">String</span><span class="sxs-lookup"><span data-stu-id="f9126-133">String</span></span>|<span data-ttu-id="f9126-134">Ключ объекта назначения группы сценариев управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="f9126-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="f9126-135">Таржетграупид</span><span class="sxs-lookup"><span data-stu-id="f9126-135">targetGroupId</span></span>|<span data-ttu-id="f9126-136">String</span><span class="sxs-lookup"><span data-stu-id="f9126-136">String</span></span>|<span data-ttu-id="f9126-137">Идентификатор группы Azure Active Directory, на которую ориентирован сценарий.</span><span class="sxs-lookup"><span data-stu-id="f9126-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="f9126-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9126-138">Response</span></span>
<span data-ttu-id="f9126-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9126-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9126-140">Пример</span><span class="sxs-lookup"><span data-stu-id="f9126-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9126-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9126-141">Request</span></span>
<span data-ttu-id="f9126-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9126-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="f9126-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9126-143">Response</span></span>
<span data-ttu-id="f9126-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9126-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





