---
title: Создание объекта iosVppEBookAssignment
description: Создание объекта iosVppEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f6aa4201d5801f3e235fa28a44d0e38f69fd1bd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133194"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="0159c-103">Создание объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="0159c-103">Create iosVppEBookAssignment</span></span>

<span data-ttu-id="0159c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0159c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0159c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0159c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0159c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0159c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0159c-107">Создание объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0159c-107">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0159c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0159c-108">Prerequisites</span></span>
<span data-ttu-id="0159c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0159c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0159c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0159c-111">Permission type</span></span>|<span data-ttu-id="0159c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0159c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0159c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0159c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0159c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0159c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0159c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0159c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0159c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0159c-116">Not supported.</span></span>|
|<span data-ttu-id="0159c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0159c-117">Application</span></span>|<span data-ttu-id="0159c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0159c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0159c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0159c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0159c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0159c-120">Request headers</span></span>
|<span data-ttu-id="0159c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0159c-121">Header</span></span>|<span data-ttu-id="0159c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0159c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0159c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0159c-123">Authorization</span></span>|<span data-ttu-id="0159c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0159c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0159c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0159c-125">Accept</span></span>|<span data-ttu-id="0159c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0159c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0159c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0159c-127">Request body</span></span>
<span data-ttu-id="0159c-128">В тексте запроса добавьте представление объекта iosVppEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0159c-128">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="0159c-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="0159c-129">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="0159c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0159c-130">Property</span></span>|<span data-ttu-id="0159c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0159c-131">Type</span></span>|<span data-ttu-id="0159c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0159c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0159c-133">id</span><span class="sxs-lookup"><span data-stu-id="0159c-133">id</span></span>|<span data-ttu-id="0159c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0159c-134">String</span></span>|<span data-ttu-id="0159c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0159c-135">Key of the entity.</span></span> <span data-ttu-id="0159c-136">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0159c-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="0159c-137">target</span><span class="sxs-lookup"><span data-stu-id="0159c-137">target</span></span>|[<span data-ttu-id="0159c-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0159c-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0159c-139">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="0159c-139">The assignment target for eBook.</span></span> <span data-ttu-id="0159c-140">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0159c-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="0159c-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="0159c-141">installIntent</span></span>|[<span data-ttu-id="0159c-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="0159c-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="0159c-143">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="0159c-143">The install intent for eBook.</span></span> <span data-ttu-id="0159c-144">Унаследованный от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0159c-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="0159c-145">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="0159c-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="0159c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="0159c-146">Response</span></span>
<span data-ttu-id="0159c-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0159c-147">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0159c-148">Пример</span><span class="sxs-lookup"><span data-stu-id="0159c-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="0159c-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="0159c-149">Request</span></span>
<span data-ttu-id="0159c-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0159c-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="0159c-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="0159c-151">Response</span></span>
<span data-ttu-id="0159c-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0159c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "48f05789-5789-48f0-8957-f0488957f048",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "installIntent": "required"
}
```




