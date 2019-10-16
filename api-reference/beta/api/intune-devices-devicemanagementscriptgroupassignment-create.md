---
title: Создание Девицеманажементскриптграупассигнмент
description: Создание нового объекта Девицеманажементскриптграупассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 16503a1590b56062127d9388adefbfd2c1f0863f
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37530421"
---
# <a name="create-devicemanagementscriptgroupassignment"></a><span data-ttu-id="cb357-103">Создание Девицеманажементскриптграупассигнмент</span><span class="sxs-lookup"><span data-stu-id="cb357-103">Create deviceManagementScriptGroupAssignment</span></span>

> <span data-ttu-id="cb357-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb357-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb357-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb357-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb357-106">Создание нового объекта [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="cb357-106">Create a new [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb357-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cb357-107">Prerequisites</span></span>
<span data-ttu-id="cb357-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb357-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb357-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb357-110">Permission type</span></span>|<span data-ttu-id="cb357-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb357-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb357-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb357-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb357-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb357-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cb357-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb357-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb357-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb357-115">Not supported.</span></span>|
|<span data-ttu-id="cb357-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="cb357-116">Application</span></span>|<span data-ttu-id="cb357-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb357-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb357-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb357-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="cb357-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb357-119">Request headers</span></span>
|<span data-ttu-id="cb357-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb357-120">Header</span></span>|<span data-ttu-id="cb357-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cb357-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb357-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb357-122">Authorization</span></span>|<span data-ttu-id="cb357-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb357-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb357-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cb357-124">Accept</span></span>|<span data-ttu-id="cb357-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cb357-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb357-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb357-126">Request body</span></span>
<span data-ttu-id="cb357-127">В тексте запроса добавьте представление объекта Девицеманажементскриптграупассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb357-127">In the request body, supply a JSON representation for the deviceManagementScriptGroupAssignment object.</span></span>

<span data-ttu-id="cb357-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементскриптграупассигнмент.</span><span class="sxs-lookup"><span data-stu-id="cb357-128">The following table shows the properties that are required when you create the deviceManagementScriptGroupAssignment.</span></span>

|<span data-ttu-id="cb357-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb357-129">Property</span></span>|<span data-ttu-id="cb357-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cb357-130">Type</span></span>|<span data-ttu-id="cb357-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cb357-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb357-132">id</span><span class="sxs-lookup"><span data-stu-id="cb357-132">id</span></span>|<span data-ttu-id="cb357-133">String</span><span class="sxs-lookup"><span data-stu-id="cb357-133">String</span></span>|<span data-ttu-id="cb357-134">Ключ объекта назначения группы сценариев управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="cb357-134">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="cb357-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb357-135">This property is read-only.</span></span>|
|<span data-ttu-id="cb357-136">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="cb357-136">targetGroupId</span></span>|<span data-ttu-id="cb357-137">String</span><span class="sxs-lookup"><span data-stu-id="cb357-137">String</span></span>|<span data-ttu-id="cb357-138">Идентификатор группы Azure Active Directory, на которую ориентирован сценарий.</span><span class="sxs-lookup"><span data-stu-id="cb357-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="cb357-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb357-139">Response</span></span>
<span data-ttu-id="cb357-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cb357-140">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb357-141">Пример</span><span class="sxs-lookup"><span data-stu-id="cb357-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb357-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb357-142">Request</span></span>
<span data-ttu-id="cb357-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb357-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="cb357-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb357-144">Response</span></span>
<span data-ttu-id="cb357-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb357-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






