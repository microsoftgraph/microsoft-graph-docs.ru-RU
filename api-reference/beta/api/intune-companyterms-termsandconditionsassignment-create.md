---
title: Создание объекта termsAndConditionsAssignment
description: Создание объекта termsAndConditionsAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8306764b2d413def47a46a4e3978121dad4f9cb7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793180"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="d476b-103">Создание объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d476b-103">Create termsAndConditionsAssignment</span></span>

<span data-ttu-id="d476b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d476b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d476b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d476b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d476b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d476b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d476b-107">Создание объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d476b-107">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d476b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d476b-108">Prerequisites</span></span>
<span data-ttu-id="d476b-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d476b-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d476b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d476b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d476b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d476b-111">Permission type</span></span>|<span data-ttu-id="d476b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d476b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d476b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d476b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d476b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d476b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d476b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d476b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d476b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d476b-116">Not supported.</span></span>|
|<span data-ttu-id="d476b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d476b-117">Application</span></span>|<span data-ttu-id="d476b-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d476b-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d476b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d476b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d476b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d476b-120">Request headers</span></span>
|<span data-ttu-id="d476b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d476b-121">Header</span></span>|<span data-ttu-id="d476b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d476b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d476b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d476b-123">Authorization</span></span>|<span data-ttu-id="d476b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d476b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d476b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d476b-125">Accept</span></span>|<span data-ttu-id="d476b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d476b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d476b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d476b-127">Request body</span></span>
<span data-ttu-id="d476b-128">В тексте запроса добавьте представление объекта termsAndConditionsAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d476b-128">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="d476b-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта termsAndConditionsAssignment.</span><span class="sxs-lookup"><span data-stu-id="d476b-129">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="d476b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d476b-130">Property</span></span>|<span data-ttu-id="d476b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d476b-131">Type</span></span>|<span data-ttu-id="d476b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d476b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d476b-133">id</span><span class="sxs-lookup"><span data-stu-id="d476b-133">id</span></span>|<span data-ttu-id="d476b-134">String</span><span class="sxs-lookup"><span data-stu-id="d476b-134">String</span></span>|<span data-ttu-id="d476b-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="d476b-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d476b-136">target</span><span class="sxs-lookup"><span data-stu-id="d476b-136">target</span></span>|[<span data-ttu-id="d476b-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d476b-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d476b-138">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="d476b-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="d476b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d476b-139">Response</span></span>
<span data-ttu-id="d476b-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d476b-140">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d476b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d476b-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d476b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d476b-142">Request</span></span>
<span data-ttu-id="d476b-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d476b-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
Content-type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="d476b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d476b-144">Response</span></span>
<span data-ttu-id="d476b-145">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="d476b-145">Here is an example of the response.</span></span> <span data-ttu-id="d476b-146">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="d476b-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d476b-147">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="d476b-147">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 372

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



