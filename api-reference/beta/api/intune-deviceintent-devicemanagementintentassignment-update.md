---
title: Обновление deviceManagementIntentAssignment
description: Обновление свойств объекта deviceManagementIntentAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ef385cc0854e6941eb9e07d4149ebe0b9a8c57e1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159705"
---
# <a name="update-devicemanagementintentassignment"></a><span data-ttu-id="a491a-103">Обновление deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="a491a-103">Update deviceManagementIntentAssignment</span></span>

<span data-ttu-id="a491a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a491a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a491a-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a491a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a491a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a491a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a491a-107">Обновление свойств объекта [deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a491a-107">Update the properties of a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a491a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a491a-108">Prerequisites</span></span>
<span data-ttu-id="a491a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a491a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a491a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a491a-111">Permission type</span></span>|<span data-ttu-id="a491a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a491a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a491a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a491a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a491a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a491a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a491a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a491a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a491a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a491a-116">Not supported.</span></span>|
|<span data-ttu-id="a491a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a491a-117">Application</span></span>|<span data-ttu-id="a491a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a491a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a491a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a491a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="a491a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a491a-120">Request headers</span></span>
|<span data-ttu-id="a491a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a491a-121">Header</span></span>|<span data-ttu-id="a491a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a491a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a491a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a491a-123">Authorization</span></span>|<span data-ttu-id="a491a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a491a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a491a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a491a-125">Accept</span></span>|<span data-ttu-id="a491a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a491a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a491a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a491a-127">Request body</span></span>
<span data-ttu-id="a491a-128">В теле запроса упростите представление объекта [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="a491a-128">In the request body, supply a JSON representation for the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

<span data-ttu-id="a491a-129">В следующей таблице показаны свойства, необходимые при создании [объекта deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a491a-129">The following table shows the properties that are required when you create the [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).</span></span>

|<span data-ttu-id="a491a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a491a-130">Property</span></span>|<span data-ttu-id="a491a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a491a-131">Type</span></span>|<span data-ttu-id="a491a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a491a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a491a-133">id</span><span class="sxs-lookup"><span data-stu-id="a491a-133">id</span></span>|<span data-ttu-id="a491a-134">String</span><span class="sxs-lookup"><span data-stu-id="a491a-134">String</span></span>|<span data-ttu-id="a491a-135">ИД назначения</span><span class="sxs-lookup"><span data-stu-id="a491a-135">The assignment ID</span></span>|
|<span data-ttu-id="a491a-136">target</span><span class="sxs-lookup"><span data-stu-id="a491a-136">target</span></span>|[<span data-ttu-id="a491a-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a491a-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a491a-138">Целевой объект назначения</span><span class="sxs-lookup"><span data-stu-id="a491a-138">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="a491a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a491a-139">Response</span></span>
<span data-ttu-id="a491a-140">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a491a-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a491a-141">Пример</span><span class="sxs-lookup"><span data-stu-id="a491a-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="a491a-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="a491a-142">Request</span></span>
<span data-ttu-id="a491a-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a491a-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments/{deviceManagementIntentAssignmentId}
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="a491a-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a491a-144">Response</span></span>
<span data-ttu-id="a491a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a491a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "id": "bedc5365-5365-bedc-6553-dcbe6553dcbe",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```




