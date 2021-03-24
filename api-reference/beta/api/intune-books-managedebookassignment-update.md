---
title: Обновление объекта managedEBookAssignment
description: Обновление свойств объекта managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d1adfc73c4986605a1a70ed2b5f3ca0dfcf1fd5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133075"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="a2391-103">Обновление объекта managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="a2391-103">Update managedEBookAssignment</span></span>

<span data-ttu-id="a2391-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2391-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2391-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2391-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2391-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2391-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2391-107">Обновление свойств объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a2391-107">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2391-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a2391-108">Prerequisites</span></span>
<span data-ttu-id="a2391-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2391-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2391-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2391-111">Permission type</span></span>|<span data-ttu-id="a2391-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2391-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2391-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2391-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2391-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2391-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a2391-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2391-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2391-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2391-116">Not supported.</span></span>|
|<span data-ttu-id="a2391-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a2391-117">Application</span></span>|<span data-ttu-id="a2391-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2391-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2391-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2391-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="a2391-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a2391-120">Request headers</span></span>
|<span data-ttu-id="a2391-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2391-121">Header</span></span>|<span data-ttu-id="a2391-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a2391-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2391-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2391-123">Authorization</span></span>|<span data-ttu-id="a2391-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2391-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2391-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2391-125">Accept</span></span>|<span data-ttu-id="a2391-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2391-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2391-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2391-127">Request body</span></span>
<span data-ttu-id="a2391-128">В тексте запроса добавьте представление объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2391-128">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="a2391-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a2391-129">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="a2391-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2391-130">Property</span></span>|<span data-ttu-id="a2391-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a2391-131">Type</span></span>|<span data-ttu-id="a2391-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a2391-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2391-133">id</span><span class="sxs-lookup"><span data-stu-id="a2391-133">id</span></span>|<span data-ttu-id="a2391-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a2391-134">String</span></span>|<span data-ttu-id="a2391-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a2391-135">Key of the entity.</span></span>|
|<span data-ttu-id="a2391-136">target</span><span class="sxs-lookup"><span data-stu-id="a2391-136">target</span></span>|[<span data-ttu-id="a2391-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a2391-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a2391-138">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="a2391-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="a2391-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="a2391-139">installIntent</span></span>|[<span data-ttu-id="a2391-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="a2391-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="a2391-141">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="a2391-141">The install intent for eBook.</span></span> <span data-ttu-id="a2391-142">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="a2391-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="a2391-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2391-143">Response</span></span>
<span data-ttu-id="a2391-144">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2391-144">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2391-145">Пример</span><span class="sxs-lookup"><span data-stu-id="a2391-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2391-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2391-146">Request</span></span>
<span data-ttu-id="a2391-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2391-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 355

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="a2391-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2391-148">Response</span></span>
<span data-ttu-id="a2391-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2391-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 404

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "installIntent": "required"
}
```




