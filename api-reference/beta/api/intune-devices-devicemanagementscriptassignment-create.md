---
title: Создание deviceManagementScriptAssignment
description: Создание нового объекта deviceManagementScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9fbb39816cc4a542c74fd166be431df2e71f7273
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611995"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="6df56-103">Создание deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="6df56-103">Create deviceManagementScriptAssignment</span></span>

<span data-ttu-id="6df56-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6df56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6df56-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6df56-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6df56-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6df56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6df56-107">Создание нового [объекта deviceManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6df56-107">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6df56-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6df56-108">Prerequisites</span></span>
<span data-ttu-id="6df56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6df56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6df56-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6df56-111">Permission type</span></span>|<span data-ttu-id="6df56-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6df56-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6df56-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6df56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6df56-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6df56-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6df56-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6df56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6df56-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6df56-116">Not supported.</span></span>|
|<span data-ttu-id="6df56-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6df56-117">Application</span></span>|<span data-ttu-id="6df56-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6df56-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6df56-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6df56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
POST /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6df56-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6df56-120">Request headers</span></span>
|<span data-ttu-id="6df56-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6df56-121">Header</span></span>|<span data-ttu-id="6df56-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6df56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6df56-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6df56-123">Authorization</span></span>|<span data-ttu-id="6df56-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6df56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6df56-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6df56-125">Accept</span></span>|<span data-ttu-id="6df56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6df56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6df56-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6df56-127">Request body</span></span>
<span data-ttu-id="6df56-128">В теле запроса поставляем представление JSON для объекта deviceManagementScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="6df56-128">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="6df56-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="6df56-129">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="6df56-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6df56-130">Property</span></span>|<span data-ttu-id="6df56-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6df56-131">Type</span></span>|<span data-ttu-id="6df56-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6df56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6df56-133">id</span><span class="sxs-lookup"><span data-stu-id="6df56-133">id</span></span>|<span data-ttu-id="6df56-134">String</span><span class="sxs-lookup"><span data-stu-id="6df56-134">String</span></span>|<span data-ttu-id="6df56-135">Ключ объекта группового назначения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="6df56-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="6df56-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6df56-136">This property is read-only.</span></span>|
|<span data-ttu-id="6df56-137">target</span><span class="sxs-lookup"><span data-stu-id="6df56-137">target</span></span>|[<span data-ttu-id="6df56-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6df56-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6df56-139">Id группы Azure Active Directory, на который мы нацелены сценарий.</span><span class="sxs-lookup"><span data-stu-id="6df56-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="6df56-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6df56-140">Response</span></span>
<span data-ttu-id="6df56-141">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6df56-141">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6df56-142">Пример</span><span class="sxs-lookup"><span data-stu-id="6df56-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="6df56-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="6df56-143">Request</span></span>
<span data-ttu-id="6df56-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6df56-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
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

### <a name="response"></a><span data-ttu-id="6df56-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="6df56-145">Response</span></span>
<span data-ttu-id="6df56-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6df56-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




