---
title: Обновление Девицеманажементинтентассигнмент
description: Обновление свойств объекта Девицеманажементинтентассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a1fd6d161288bc3be0323478ea2d3ac79529397c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42471045"
---
# <a name="update-devicemanagementintentassignment"></a><span data-ttu-id="46862-103">Обновление Девицеманажементинтентассигнмент</span><span class="sxs-lookup"><span data-stu-id="46862-103">Update deviceManagementIntentAssignment</span></span>

<span data-ttu-id="46862-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="46862-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46862-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46862-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46862-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46862-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46862-107">Обновление свойств объекта [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="46862-107">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46862-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="46862-108">Prerequisites</span></span>
<span data-ttu-id="46862-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46862-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46862-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46862-111">Permission type</span></span>|<span data-ttu-id="46862-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46862-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46862-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46862-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46862-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46862-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46862-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46862-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46862-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46862-116">Not supported.</span></span>|
|<span data-ttu-id="46862-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46862-117">Application</span></span>|<span data-ttu-id="46862-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46862-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46862-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46862-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="46862-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="46862-120">Request headers</span></span>
|<span data-ttu-id="46862-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46862-121">Header</span></span>|<span data-ttu-id="46862-122">Значение</span><span class="sxs-lookup"><span data-stu-id="46862-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46862-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="46862-123">Authorization</span></span>|<span data-ttu-id="46862-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46862-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46862-125">Accept</span><span class="sxs-lookup"><span data-stu-id="46862-125">Accept</span></span>|<span data-ttu-id="46862-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46862-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46862-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46862-127">Request body</span></span>
<span data-ttu-id="46862-128">В тексте запроса добавьте представление объекта [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46862-128">In the request body, supply a JSON representation for the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

<span data-ttu-id="46862-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span><span class="sxs-lookup"><span data-stu-id="46862-129">The following table shows the properties that are required when you create the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>

|<span data-ttu-id="46862-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="46862-130">Property</span></span>|<span data-ttu-id="46862-131">Тип</span><span class="sxs-lookup"><span data-stu-id="46862-131">Type</span></span>|<span data-ttu-id="46862-132">Описание</span><span class="sxs-lookup"><span data-stu-id="46862-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46862-133">id</span><span class="sxs-lookup"><span data-stu-id="46862-133">id</span></span>|<span data-ttu-id="46862-134">String</span><span class="sxs-lookup"><span data-stu-id="46862-134">String</span></span>|<span data-ttu-id="46862-135">Идентификатор назначения</span><span class="sxs-lookup"><span data-stu-id="46862-135">The assignment ID</span></span>|
|<span data-ttu-id="46862-136">target</span><span class="sxs-lookup"><span data-stu-id="46862-136">target</span></span>|[<span data-ttu-id="46862-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="46862-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="46862-138">Цель назначения</span><span class="sxs-lookup"><span data-stu-id="46862-138">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="46862-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="46862-139">Response</span></span>
<span data-ttu-id="46862-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="46862-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46862-141">Пример</span><span class="sxs-lookup"><span data-stu-id="46862-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="46862-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="46862-142">Request</span></span>
<span data-ttu-id="46862-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46862-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="46862-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="46862-144">Response</span></span>
<span data-ttu-id="46862-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46862-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





