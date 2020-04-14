---
title: Обновление объекта termsAndConditionsAssignment
description: Удаление свойств объекта termsAndConditionsAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 83a718a635a607113bfda037e50e8c944bcb3306
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436406"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="7b67f-103">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="7b67f-103">Update termsAndConditionsAssignment</span></span>

<span data-ttu-id="7b67f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b67f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b67f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b67f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b67f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b67f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b67f-107">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7b67f-107">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b67f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7b67f-108">Prerequisites</span></span>
<span data-ttu-id="7b67f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b67f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b67f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b67f-111">Permission type</span></span>|<span data-ttu-id="7b67f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b67f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b67f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b67f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b67f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b67f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7b67f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b67f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b67f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b67f-116">Not supported.</span></span>|
|<span data-ttu-id="7b67f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7b67f-117">Application</span></span>|<span data-ttu-id="7b67f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b67f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b67f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b67f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7b67f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7b67f-120">Request headers</span></span>
|<span data-ttu-id="7b67f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b67f-121">Header</span></span>|<span data-ttu-id="7b67f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7b67f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b67f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b67f-123">Authorization</span></span>|<span data-ttu-id="7b67f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b67f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b67f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7b67f-125">Accept</span></span>|<span data-ttu-id="7b67f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b67f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b67f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b67f-127">Request body</span></span>
<span data-ttu-id="7b67f-128">В тексте запроса добавьте представление объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b67f-128">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="7b67f-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7b67f-129">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="7b67f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b67f-130">Property</span></span>|<span data-ttu-id="7b67f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7b67f-131">Type</span></span>|<span data-ttu-id="7b67f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7b67f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b67f-133">id</span><span class="sxs-lookup"><span data-stu-id="7b67f-133">id</span></span>|<span data-ttu-id="7b67f-134">String</span><span class="sxs-lookup"><span data-stu-id="7b67f-134">String</span></span>|<span data-ttu-id="7b67f-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="7b67f-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="7b67f-136">target</span><span class="sxs-lookup"><span data-stu-id="7b67f-136">target</span></span>|[<span data-ttu-id="7b67f-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7b67f-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7b67f-138">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="7b67f-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="7b67f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b67f-139">Response</span></span>
<span data-ttu-id="7b67f-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7b67f-140">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b67f-141">Пример</span><span class="sxs-lookup"><span data-stu-id="7b67f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b67f-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b67f-142">Request</span></span>
<span data-ttu-id="7b67f-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b67f-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="7b67f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b67f-144">Response</span></span>
<span data-ttu-id="7b67f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b67f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 217

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



