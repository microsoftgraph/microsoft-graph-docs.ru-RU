---
title: Обновление Девицеманажементинтентассигнмент
description: Обновление свойств объекта Девицеманажементинтентассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 99d4d5e36338e94d488925eab6612bf53a1739d7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313190"
---
# <a name="update-devicemanagementintentassignment"></a><span data-ttu-id="889b7-103">Обновление Девицеманажементинтентассигнмент</span><span class="sxs-lookup"><span data-stu-id="889b7-103">Update deviceManagementIntentAssignment</span></span>

> <span data-ttu-id="889b7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="889b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="889b7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="889b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="889b7-106">Обновление свойств объекта [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="889b7-106">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="889b7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="889b7-107">Prerequisites</span></span>
<span data-ttu-id="889b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="889b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="889b7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="889b7-110">Permission type</span></span>|<span data-ttu-id="889b7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="889b7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="889b7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="889b7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="889b7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="889b7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="889b7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="889b7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="889b7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="889b7-115">Not supported.</span></span>|
|<span data-ttu-id="889b7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="889b7-116">Application</span></span>|<span data-ttu-id="889b7-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="889b7-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="889b7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="889b7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="889b7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="889b7-119">Request headers</span></span>
|<span data-ttu-id="889b7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="889b7-120">Header</span></span>|<span data-ttu-id="889b7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="889b7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="889b7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="889b7-122">Authorization</span></span>|<span data-ttu-id="889b7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="889b7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="889b7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="889b7-124">Accept</span></span>|<span data-ttu-id="889b7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="889b7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="889b7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="889b7-126">Request body</span></span>
<span data-ttu-id="889b7-127">В тексте запроса добавьте представление объекта [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="889b7-127">In the request body, supply a JSON representation for the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

<span data-ttu-id="889b7-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span><span class="sxs-lookup"><span data-stu-id="889b7-128">The following table shows the properties that are required when you create the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>

|<span data-ttu-id="889b7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="889b7-129">Property</span></span>|<span data-ttu-id="889b7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="889b7-130">Type</span></span>|<span data-ttu-id="889b7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="889b7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="889b7-132">id</span><span class="sxs-lookup"><span data-stu-id="889b7-132">id</span></span>|<span data-ttu-id="889b7-133">String</span><span class="sxs-lookup"><span data-stu-id="889b7-133">String</span></span>|<span data-ttu-id="889b7-134">Идентификатор назначения</span><span class="sxs-lookup"><span data-stu-id="889b7-134">The assignment ID</span></span>|
|<span data-ttu-id="889b7-135">target</span><span class="sxs-lookup"><span data-stu-id="889b7-135">target</span></span>|[<span data-ttu-id="889b7-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="889b7-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="889b7-137">Цель назначения</span><span class="sxs-lookup"><span data-stu-id="889b7-137">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="889b7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="889b7-138">Response</span></span>
<span data-ttu-id="889b7-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентассигнмент](../resources/intune-deviceintent-devicemanagementintentassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="889b7-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="889b7-140">Пример</span><span class="sxs-lookup"><span data-stu-id="889b7-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="889b7-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="889b7-141">Request</span></span>
<span data-ttu-id="889b7-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="889b7-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="889b7-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="889b7-143">Response</span></span>
<span data-ttu-id="889b7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="889b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






