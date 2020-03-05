---
title: Создание Девицеманажементинтентассигнмент
description: Создание нового объекта Девицеманажементинтентассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 096d949bbef788e4a17eebed0cb1052460c4cc37
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42471122"
---
# <a name="create-devicemanagementintentassignment"></a><span data-ttu-id="dd5cf-103">Создание Девицеманажементинтентассигнмент</span><span class="sxs-lookup"><span data-stu-id="dd5cf-103">Create deviceManagementIntentAssignment</span></span>

<span data-ttu-id="dd5cf-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dd5cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd5cf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd5cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd5cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd5cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd5cf-107">Создание нового объекта [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="dd5cf-107">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd5cf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dd5cf-108">Prerequisites</span></span>
<span data-ttu-id="dd5cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd5cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd5cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd5cf-111">Permission type</span></span>|<span data-ttu-id="dd5cf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd5cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd5cf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd5cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd5cf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd5cf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd5cf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd5cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd5cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd5cf-116">Not supported.</span></span>|
|<span data-ttu-id="dd5cf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd5cf-117">Application</span></span>|<span data-ttu-id="dd5cf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd5cf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd5cf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd5cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="dd5cf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dd5cf-120">Request headers</span></span>
|<span data-ttu-id="dd5cf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd5cf-121">Header</span></span>|<span data-ttu-id="dd5cf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dd5cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd5cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd5cf-123">Authorization</span></span>|<span data-ttu-id="dd5cf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd5cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd5cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dd5cf-125">Accept</span></span>|<span data-ttu-id="dd5cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd5cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd5cf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd5cf-127">Request body</span></span>
<span data-ttu-id="dd5cf-128">В тексте запроса добавьте представление объекта Девицеманажементинтентассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd5cf-128">In the request body, supply a JSON representation for the deviceManagementIntentAssignment object.</span></span>

<span data-ttu-id="dd5cf-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтентассигнмент.</span><span class="sxs-lookup"><span data-stu-id="dd5cf-129">The following table shows the properties that are required when you create the deviceManagementIntentAssignment.</span></span>

|<span data-ttu-id="dd5cf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd5cf-130">Property</span></span>|<span data-ttu-id="dd5cf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dd5cf-131">Type</span></span>|<span data-ttu-id="dd5cf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dd5cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd5cf-133">id</span><span class="sxs-lookup"><span data-stu-id="dd5cf-133">id</span></span>|<span data-ttu-id="dd5cf-134">String</span><span class="sxs-lookup"><span data-stu-id="dd5cf-134">String</span></span>|<span data-ttu-id="dd5cf-135">Идентификатор назначения</span><span class="sxs-lookup"><span data-stu-id="dd5cf-135">The assignment ID</span></span>|
|<span data-ttu-id="dd5cf-136">target</span><span class="sxs-lookup"><span data-stu-id="dd5cf-136">target</span></span>|[<span data-ttu-id="dd5cf-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="dd5cf-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="dd5cf-138">Цель назначения</span><span class="sxs-lookup"><span data-stu-id="dd5cf-138">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="dd5cf-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd5cf-139">Response</span></span>
<span data-ttu-id="dd5cf-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd5cf-140">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd5cf-141">Пример</span><span class="sxs-lookup"><span data-stu-id="dd5cf-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd5cf-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd5cf-142">Request</span></span>
<span data-ttu-id="dd5cf-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd5cf-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="dd5cf-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd5cf-144">Response</span></span>
<span data-ttu-id="dd5cf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd5cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





