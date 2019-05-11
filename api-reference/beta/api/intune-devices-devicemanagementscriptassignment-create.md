---
title: Создание Девицеманажементскриптассигнмент
description: Создание нового объекта Девицеманажементскриптассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54e5848e79608b0dd9955316071531fb87f022a6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909892"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="1ee36-103">Создание Девицеманажементскриптассигнмент</span><span class="sxs-lookup"><span data-stu-id="1ee36-103">Create deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="1ee36-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ee36-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ee36-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ee36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ee36-106">Создание нового объекта [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1ee36-106">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ee36-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1ee36-107">Prerequisites</span></span>
<span data-ttu-id="1ee36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ee36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ee36-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ee36-110">Permission type</span></span>|<span data-ttu-id="1ee36-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ee36-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ee36-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ee36-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ee36-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee36-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1ee36-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ee36-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ee36-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ee36-115">Not supported.</span></span>|
|<span data-ttu-id="1ee36-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ee36-116">Application</span></span>|<span data-ttu-id="1ee36-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ee36-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ee36-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ee36-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1ee36-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ee36-119">Request headers</span></span>
|<span data-ttu-id="1ee36-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ee36-120">Header</span></span>|<span data-ttu-id="1ee36-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1ee36-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ee36-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ee36-122">Authorization</span></span>|<span data-ttu-id="1ee36-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ee36-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ee36-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1ee36-124">Accept</span></span>|<span data-ttu-id="1ee36-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1ee36-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ee36-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ee36-126">Request body</span></span>
<span data-ttu-id="1ee36-127">В тексте запроса добавьте представление объекта Девицеманажементскриптассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ee36-127">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="1ee36-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементскриптассигнмент.</span><span class="sxs-lookup"><span data-stu-id="1ee36-128">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="1ee36-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ee36-129">Property</span></span>|<span data-ttu-id="1ee36-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1ee36-130">Type</span></span>|<span data-ttu-id="1ee36-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1ee36-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ee36-132">id</span><span class="sxs-lookup"><span data-stu-id="1ee36-132">id</span></span>|<span data-ttu-id="1ee36-133">Строка</span><span class="sxs-lookup"><span data-stu-id="1ee36-133">String</span></span>|<span data-ttu-id="1ee36-134">Ключ объекта назначения группы сценариев управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="1ee36-134">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="1ee36-135">target</span><span class="sxs-lookup"><span data-stu-id="1ee36-135">target</span></span>|[<span data-ttu-id="1ee36-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1ee36-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1ee36-137">Идентификатор группы Azure Active Directory, на которую ориентирован сценарий.</span><span class="sxs-lookup"><span data-stu-id="1ee36-137">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="1ee36-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ee36-138">Response</span></span>
<span data-ttu-id="1ee36-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ee36-139">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ee36-140">Пример</span><span class="sxs-lookup"><span data-stu-id="1ee36-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ee36-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ee36-141">Request</span></span>
<span data-ttu-id="1ee36-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ee36-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="1ee36-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ee36-143">Response</span></span>
<span data-ttu-id="1ee36-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ee36-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




