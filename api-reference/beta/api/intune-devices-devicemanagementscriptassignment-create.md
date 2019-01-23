---
title: Создание deviceManagementScriptAssignment
description: Создание нового объекта deviceManagementScriptAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4cb2ac3d0ac83824197e40850f0a4e503e813ad0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402267"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="2b5c7-103">Создание deviceManagementScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="2b5c7-103">Create deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="2b5c7-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2b5c7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2b5c7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b5c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b5c7-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b5c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b5c7-107">Создание нового объекта [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2b5c7-107">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b5c7-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="2b5c7-108">Prerequisites</span></span>
<span data-ttu-id="2b5c7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2b5c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2b5c7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b5c7-111">Permission type</span></span>|<span data-ttu-id="2b5c7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b5c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b5c7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b5c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b5c7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b5c7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2b5c7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b5c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b5c7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b5c7-116">Not supported.</span></span>|
|<span data-ttu-id="2b5c7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b5c7-117">Application</span></span>|<span data-ttu-id="2b5c7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b5c7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b5c7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b5c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2b5c7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b5c7-120">Request headers</span></span>
|<span data-ttu-id="2b5c7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b5c7-121">Header</span></span>|<span data-ttu-id="2b5c7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2b5c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b5c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b5c7-123">Authorization</span></span>|<span data-ttu-id="2b5c7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2b5c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b5c7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b5c7-125">Accept</span></span>|<span data-ttu-id="2b5c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b5c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b5c7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b5c7-127">Request body</span></span>
<span data-ttu-id="2b5c7-128">В тексте запроса укажите представление JSON для объекта deviceManagementScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="2b5c7-128">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="2b5c7-129">В следующей таблице показаны свойства, которые необходимы для создания deviceManagementScriptAssignment.</span><span class="sxs-lookup"><span data-stu-id="2b5c7-129">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="2b5c7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b5c7-130">Property</span></span>|<span data-ttu-id="2b5c7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2b5c7-131">Type</span></span>|<span data-ttu-id="2b5c7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2b5c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b5c7-133">id</span><span class="sxs-lookup"><span data-stu-id="2b5c7-133">id</span></span>|<span data-ttu-id="2b5c7-134">String</span><span class="sxs-lookup"><span data-stu-id="2b5c7-134">String</span></span>|<span data-ttu-id="2b5c7-135">Ключ объекта назначения группы, сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="2b5c7-135">Key of the device management script group assignment entity.</span></span>|
|<span data-ttu-id="2b5c7-136">target</span><span class="sxs-lookup"><span data-stu-id="2b5c7-136">target</span></span>|[<span data-ttu-id="2b5c7-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2b5c7-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2b5c7-138">Идентификатор группы Azure Active Directory мы ориентация сценария.</span><span class="sxs-lookup"><span data-stu-id="2b5c7-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="2b5c7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b5c7-139">Response</span></span>
<span data-ttu-id="2b5c7-140">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2b5c7-140">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b5c7-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2b5c7-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b5c7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b5c7-142">Request</span></span>
<span data-ttu-id="2b5c7-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b5c7-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2b5c7-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b5c7-144">Response</span></span>
<span data-ttu-id="2b5c7-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2b5c7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




