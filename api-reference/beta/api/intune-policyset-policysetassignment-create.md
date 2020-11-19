---
title: Создание Полицисетассигнмент
description: Создание нового объекта Полицисетассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 85a40859f986d07c36cc6e1d5950d3b1e23c00c7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49257886"
---
# <a name="create-policysetassignment"></a><span data-ttu-id="14b84-103">Создание Полицисетассигнмент</span><span class="sxs-lookup"><span data-stu-id="14b84-103">Create policySetAssignment</span></span>

<span data-ttu-id="14b84-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14b84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14b84-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14b84-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14b84-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14b84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14b84-107">Создание нового объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="14b84-107">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14b84-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="14b84-108">Prerequisites</span></span>
<span data-ttu-id="14b84-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14b84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14b84-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14b84-111">Permission type</span></span>|<span data-ttu-id="14b84-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14b84-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14b84-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14b84-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14b84-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14b84-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14b84-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14b84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14b84-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14b84-116">Not supported.</span></span>|
|<span data-ttu-id="14b84-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="14b84-117">Application</span></span>|<span data-ttu-id="14b84-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14b84-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14b84-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14b84-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="14b84-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="14b84-120">Request headers</span></span>
|<span data-ttu-id="14b84-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14b84-121">Header</span></span>|<span data-ttu-id="14b84-122">Значение</span><span class="sxs-lookup"><span data-stu-id="14b84-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14b84-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14b84-123">Authorization</span></span>|<span data-ttu-id="14b84-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14b84-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14b84-125">Accept</span><span class="sxs-lookup"><span data-stu-id="14b84-125">Accept</span></span>|<span data-ttu-id="14b84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14b84-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14b84-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14b84-127">Request body</span></span>
<span data-ttu-id="14b84-128">В тексте запроса добавьте представление объекта Полицисетассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14b84-128">In the request body, supply a JSON representation for the policySetAssignment object.</span></span>

<span data-ttu-id="14b84-129">В следующей таблице приведены свойства, необходимые при создании Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="14b84-129">The following table shows the properties that are required when you create the policySetAssignment.</span></span>

|<span data-ttu-id="14b84-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="14b84-130">Property</span></span>|<span data-ttu-id="14b84-131">Тип</span><span class="sxs-lookup"><span data-stu-id="14b84-131">Type</span></span>|<span data-ttu-id="14b84-132">Описание</span><span class="sxs-lookup"><span data-stu-id="14b84-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14b84-133">id</span><span class="sxs-lookup"><span data-stu-id="14b84-133">id</span></span>|<span data-ttu-id="14b84-134">String</span><span class="sxs-lookup"><span data-stu-id="14b84-134">String</span></span>|<span data-ttu-id="14b84-135">Ключ Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="14b84-135">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="14b84-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14b84-136">lastModifiedDateTime</span></span>|<span data-ttu-id="14b84-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14b84-137">DateTimeOffset</span></span>|<span data-ttu-id="14b84-138">Время последнего изменения Полицисетассигнмент.</span><span class="sxs-lookup"><span data-stu-id="14b84-138">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="14b84-139">target</span><span class="sxs-lookup"><span data-stu-id="14b84-139">target</span></span>|[<span data-ttu-id="14b84-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="14b84-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="14b84-141">Целевая группа Полицисетассигнмент</span><span class="sxs-lookup"><span data-stu-id="14b84-141">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="14b84-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="14b84-142">Response</span></span>
<span data-ttu-id="14b84-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="14b84-143">If successful, this method returns a `201 Created` response code and a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14b84-144">Пример</span><span class="sxs-lookup"><span data-stu-id="14b84-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="14b84-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="14b84-145">Request</span></span>
<span data-ttu-id="14b84-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14b84-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="14b84-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="14b84-147">Response</span></span>
<span data-ttu-id="14b84-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14b84-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 427

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




