---
title: Создание deviceManagementIntentAssignment
description: Создание объекта deviceManagementIntentAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e8a9ba1dd1fbaacd1f6b12bb280cc1c5d984ad3
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155162"
---
# <a name="create-devicemanagementintentassignment"></a><span data-ttu-id="c5000-103">Создание deviceManagementIntentAssignment</span><span class="sxs-lookup"><span data-stu-id="c5000-103">Create deviceManagementIntentAssignment</span></span>

<span data-ttu-id="c5000-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5000-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5000-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5000-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5000-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5000-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5000-107">Создание объекта [deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c5000-107">Create a new [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5000-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c5000-108">Prerequisites</span></span>
<span data-ttu-id="c5000-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5000-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5000-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5000-111">Permission type</span></span>|<span data-ttu-id="c5000-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5000-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5000-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5000-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5000-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5000-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5000-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5000-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5000-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5000-116">Not supported.</span></span>|
|<span data-ttu-id="c5000-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5000-117">Application</span></span>|<span data-ttu-id="c5000-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5000-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5000-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5000-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c5000-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c5000-120">Request headers</span></span>
|<span data-ttu-id="c5000-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5000-121">Header</span></span>|<span data-ttu-id="c5000-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c5000-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5000-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5000-123">Authorization</span></span>|<span data-ttu-id="c5000-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5000-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5000-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5000-125">Accept</span></span>|<span data-ttu-id="c5000-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5000-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5000-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5000-127">Request body</span></span>
<span data-ttu-id="c5000-128">В теле запроса упростите представление объекта deviceManagementIntentAssignment в JSON.</span><span class="sxs-lookup"><span data-stu-id="c5000-128">In the request body, supply a JSON representation for the deviceManagementIntentAssignment object.</span></span>

<span data-ttu-id="c5000-129">В следующей таблице показаны свойства, необходимые при создании объекта deviceManagementIntentAssignment.</span><span class="sxs-lookup"><span data-stu-id="c5000-129">The following table shows the properties that are required when you create the deviceManagementIntentAssignment.</span></span>

|<span data-ttu-id="c5000-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5000-130">Property</span></span>|<span data-ttu-id="c5000-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c5000-131">Type</span></span>|<span data-ttu-id="c5000-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c5000-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5000-133">id</span><span class="sxs-lookup"><span data-stu-id="c5000-133">id</span></span>|<span data-ttu-id="c5000-134">String</span><span class="sxs-lookup"><span data-stu-id="c5000-134">String</span></span>|<span data-ttu-id="c5000-135">ИД назначения</span><span class="sxs-lookup"><span data-stu-id="c5000-135">The assignment ID</span></span>|
|<span data-ttu-id="c5000-136">target</span><span class="sxs-lookup"><span data-stu-id="c5000-136">target</span></span>|[<span data-ttu-id="c5000-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c5000-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c5000-138">Целевой объект назначения</span><span class="sxs-lookup"><span data-stu-id="c5000-138">The assignment target</span></span>|



## <a name="response"></a><span data-ttu-id="c5000-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5000-139">Response</span></span>
<span data-ttu-id="c5000-140">В случае успешного выполнения этот метод возвращает код отклика и объект `201 Created` [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c5000-140">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5000-141">Пример</span><span class="sxs-lookup"><span data-stu-id="c5000-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5000-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5000-142">Request</span></span>
<span data-ttu-id="c5000-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5000-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/assignments
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

### <a name="response"></a><span data-ttu-id="c5000-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5000-144">Response</span></span>
<span data-ttu-id="c5000-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5000-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




