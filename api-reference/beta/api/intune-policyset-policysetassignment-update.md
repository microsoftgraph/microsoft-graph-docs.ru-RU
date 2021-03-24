---
title: Обновление политикиSetAssignment
description: Обновление свойств объекта policySetAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 374b233731a09e7d0bb5ef4b9d1ba26b3147f63e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134587"
---
# <a name="update-policysetassignment"></a><span data-ttu-id="cecb6-103">Обновление политикиSetAssignment</span><span class="sxs-lookup"><span data-stu-id="cecb6-103">Update policySetAssignment</span></span>

<span data-ttu-id="cecb6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cecb6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cecb6-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cecb6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cecb6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cecb6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cecb6-107">Обновление свойств объекта [policySetAssignment.](../resources/intune-policyset-policysetassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cecb6-107">Update the properties of a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cecb6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cecb6-108">Prerequisites</span></span>
<span data-ttu-id="cecb6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cecb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cecb6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cecb6-111">Permission type</span></span>|<span data-ttu-id="cecb6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cecb6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cecb6-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cecb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cecb6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cecb6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cecb6-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cecb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cecb6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cecb6-116">Not supported.</span></span>|
|<span data-ttu-id="cecb6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cecb6-117">Application</span></span>|<span data-ttu-id="cecb6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cecb6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cecb6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cecb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/assignments/{policySetAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="cecb6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cecb6-120">Request headers</span></span>
|<span data-ttu-id="cecb6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cecb6-121">Header</span></span>|<span data-ttu-id="cecb6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cecb6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cecb6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cecb6-123">Authorization</span></span>|<span data-ttu-id="cecb6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cecb6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cecb6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cecb6-125">Accept</span></span>|<span data-ttu-id="cecb6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cecb6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cecb6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cecb6-127">Request body</span></span>
<span data-ttu-id="cecb6-128">В теле запроса поставляем представление JSON для объекта [policySetAssignment.](../resources/intune-policyset-policysetassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cecb6-128">In the request body, supply a JSON representation for the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

<span data-ttu-id="cecb6-129">В следующей таблице показаны свойства, необходимые при создании [политикиSetAssignment.](../resources/intune-policyset-policysetassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cecb6-129">The following table shows the properties that are required when you create the [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span></span>

|<span data-ttu-id="cecb6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cecb6-130">Property</span></span>|<span data-ttu-id="cecb6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cecb6-131">Type</span></span>|<span data-ttu-id="cecb6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cecb6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cecb6-133">id</span><span class="sxs-lookup"><span data-stu-id="cecb6-133">id</span></span>|<span data-ttu-id="cecb6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="cecb6-134">String</span></span>|<span data-ttu-id="cecb6-135">Клавиша PolicySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="cecb6-135">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="cecb6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cecb6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cecb6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cecb6-137">DateTimeOffset</span></span>|<span data-ttu-id="cecb6-138">Последнее измененное время policySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="cecb6-138">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="cecb6-139">target</span><span class="sxs-lookup"><span data-stu-id="cecb6-139">target</span></span>|[<span data-ttu-id="cecb6-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cecb6-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cecb6-141">Целевая группа PolicySetAssignment</span><span class="sxs-lookup"><span data-stu-id="cecb6-141">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="cecb6-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="cecb6-142">Response</span></span>
<span data-ttu-id="cecb6-143">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [policySetAssignment](../resources/intune-policyset-policysetassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cecb6-143">If successful, this method returns a `200 OK` response code and an updated [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cecb6-144">Пример</span><span class="sxs-lookup"><span data-stu-id="cecb6-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="cecb6-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="cecb6-145">Request</span></span>
<span data-ttu-id="cecb6-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cecb6-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments/{policySetAssignmentId}
Content-type: application/json
Content-length: 378

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="cecb6-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="cecb6-147">Response</span></span>
<span data-ttu-id="cecb6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cecb6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 491

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```




