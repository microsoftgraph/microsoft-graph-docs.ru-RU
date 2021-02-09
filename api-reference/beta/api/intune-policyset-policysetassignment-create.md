---
title: Создание policySetAssignment
description: Создание объекта policySetAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3c2616cecf5cd66ec008dc4754670e916af1718b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153762"
---
# <a name="create-policysetassignment"></a><span data-ttu-id="9215d-103">Создание policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="9215d-103">Create policySetAssignment</span></span>

<span data-ttu-id="9215d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9215d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9215d-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9215d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9215d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9215d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9215d-107">Создание объекта [policySetAssignment.](../resources/intune-policyset-policysetassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9215d-107">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9215d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9215d-108">Prerequisites</span></span>
<span data-ttu-id="9215d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9215d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9215d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9215d-111">Permission type</span></span>|<span data-ttu-id="9215d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9215d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9215d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9215d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9215d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9215d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9215d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9215d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9215d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9215d-116">Not supported.</span></span>|
|<span data-ttu-id="9215d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9215d-117">Application</span></span>|<span data-ttu-id="9215d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9215d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9215d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9215d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9215d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9215d-120">Request headers</span></span>
|<span data-ttu-id="9215d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9215d-121">Header</span></span>|<span data-ttu-id="9215d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9215d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9215d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9215d-123">Authorization</span></span>|<span data-ttu-id="9215d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9215d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9215d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9215d-125">Accept</span></span>|<span data-ttu-id="9215d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9215d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9215d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9215d-127">Request body</span></span>
<span data-ttu-id="9215d-128">В теле запроса укажу представление объекта policySetAssignment в JSON.</span><span class="sxs-lookup"><span data-stu-id="9215d-128">In the request body, supply a JSON representation for the policySetAssignment object.</span></span>

<span data-ttu-id="9215d-129">В следующей таблице показаны свойства, необходимые при создании политикиSetAssignment.</span><span class="sxs-lookup"><span data-stu-id="9215d-129">The following table shows the properties that are required when you create the policySetAssignment.</span></span>

|<span data-ttu-id="9215d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9215d-130">Property</span></span>|<span data-ttu-id="9215d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9215d-131">Type</span></span>|<span data-ttu-id="9215d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9215d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9215d-133">id</span><span class="sxs-lookup"><span data-stu-id="9215d-133">id</span></span>|<span data-ttu-id="9215d-134">String</span><span class="sxs-lookup"><span data-stu-id="9215d-134">String</span></span>|<span data-ttu-id="9215d-135">Ключ policySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="9215d-135">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="9215d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9215d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9215d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9215d-137">DateTimeOffset</span></span>|<span data-ttu-id="9215d-138">Время последнего изменения policySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="9215d-138">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="9215d-139">target</span><span class="sxs-lookup"><span data-stu-id="9215d-139">target</span></span>|[<span data-ttu-id="9215d-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9215d-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9215d-141">Целевая группа PolicySetAssignment</span><span class="sxs-lookup"><span data-stu-id="9215d-141">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="9215d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9215d-142">Response</span></span>
<span data-ttu-id="9215d-143">В случае успешного выполнения этот метод возвращает код отклика и объект `201 Created` [policySetAssignment](../resources/intune-policyset-policysetassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9215d-143">If successful, this method returns a `201 Created` response code and a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9215d-144">Пример</span><span class="sxs-lookup"><span data-stu-id="9215d-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="9215d-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="9215d-145">Request</span></span>
<span data-ttu-id="9215d-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9215d-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments
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

### <a name="response"></a><span data-ttu-id="9215d-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="9215d-147">Response</span></span>
<span data-ttu-id="9215d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9215d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




