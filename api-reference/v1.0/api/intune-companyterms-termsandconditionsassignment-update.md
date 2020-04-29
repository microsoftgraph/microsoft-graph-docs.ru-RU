---
title: Обновление объекта termsAndConditionsAssignment
description: Удаление свойств объекта termsAndConditionsAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e82b23dbce77c101cfe661380ca4239225371119
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456350"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="d3166-103">Обновление объекта termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d3166-103">Update termsAndConditionsAssignment</span></span>

<span data-ttu-id="d3166-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3166-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3166-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3166-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3166-106">Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d3166-106">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3166-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d3166-107">Prerequisites</span></span>
<span data-ttu-id="d3166-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3166-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3166-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3166-110">Permission type</span></span>|<span data-ttu-id="d3166-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3166-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3166-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3166-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d3166-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3166-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d3166-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3166-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3166-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3166-115">Not supported.</span></span>|
|<span data-ttu-id="d3166-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3166-116">Application</span></span>|<span data-ttu-id="d3166-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3166-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3166-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3166-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d3166-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d3166-119">Request headers</span></span>
|<span data-ttu-id="d3166-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3166-120">Header</span></span>|<span data-ttu-id="d3166-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d3166-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3166-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3166-122">Authorization</span></span>|<span data-ttu-id="d3166-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3166-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3166-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d3166-124">Accept</span></span>|<span data-ttu-id="d3166-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d3166-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3166-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d3166-126">Request body</span></span>
<span data-ttu-id="d3166-127">В тексте запроса добавьте представление объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3166-127">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="d3166-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d3166-128">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="d3166-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3166-129">Property</span></span>|<span data-ttu-id="d3166-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d3166-130">Type</span></span>|<span data-ttu-id="d3166-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d3166-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3166-132">id</span><span class="sxs-lookup"><span data-stu-id="d3166-132">id</span></span>|<span data-ttu-id="d3166-133">String</span><span class="sxs-lookup"><span data-stu-id="d3166-133">String</span></span>|<span data-ttu-id="d3166-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="d3166-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d3166-135">target</span><span class="sxs-lookup"><span data-stu-id="d3166-135">target</span></span>|[<span data-ttu-id="d3166-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d3166-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d3166-137">Объект, для которого назначается политика соблюдения условий.</span><span class="sxs-lookup"><span data-stu-id="d3166-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="d3166-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3166-138">Response</span></span>
<span data-ttu-id="d3166-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3166-139">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3166-140">Пример</span><span class="sxs-lookup"><span data-stu-id="d3166-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3166-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3166-141">Request</span></span>
<span data-ttu-id="d3166-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3166-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d3166-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3166-143">Response</span></span>
<span data-ttu-id="d3166-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3166-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






