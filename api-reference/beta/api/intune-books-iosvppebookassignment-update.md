---
title: Обновление объекта iosVppEBookAssignment
description: Обновление свойств объекта iosVppEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eded12d6b291cea5247aabac5875cd747cc235c6
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793222"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="c9200-103">Обновление объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="c9200-103">Update iosVppEBookAssignment</span></span>

<span data-ttu-id="c9200-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9200-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9200-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9200-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9200-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9200-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9200-107">Обновление свойств объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c9200-107">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9200-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c9200-108">Prerequisites</span></span>
<span data-ttu-id="c9200-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9200-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9200-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9200-111">Permission type</span></span>|<span data-ttu-id="c9200-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9200-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9200-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9200-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9200-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9200-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c9200-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9200-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9200-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9200-116">Not supported.</span></span>|
|<span data-ttu-id="c9200-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9200-117">Application</span></span>|<span data-ttu-id="c9200-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9200-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9200-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9200-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c9200-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c9200-120">Request headers</span></span>
|<span data-ttu-id="c9200-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9200-121">Header</span></span>|<span data-ttu-id="c9200-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c9200-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9200-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9200-123">Authorization</span></span>|<span data-ttu-id="c9200-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9200-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9200-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c9200-125">Accept</span></span>|<span data-ttu-id="c9200-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9200-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9200-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9200-127">Request body</span></span>
<span data-ttu-id="c9200-128">В тексте запроса добавьте представление объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9200-128">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="c9200-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c9200-129">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="c9200-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9200-130">Property</span></span>|<span data-ttu-id="c9200-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c9200-131">Type</span></span>|<span data-ttu-id="c9200-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c9200-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9200-133">id</span><span class="sxs-lookup"><span data-stu-id="c9200-133">id</span></span>|<span data-ttu-id="c9200-134">String</span><span class="sxs-lookup"><span data-stu-id="c9200-134">String</span></span>|<span data-ttu-id="c9200-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c9200-135">Key of the entity.</span></span> <span data-ttu-id="c9200-136">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c9200-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="c9200-137">target</span><span class="sxs-lookup"><span data-stu-id="c9200-137">target</span></span>|[<span data-ttu-id="c9200-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c9200-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c9200-139">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="c9200-139">The assignment target for eBook.</span></span> <span data-ttu-id="c9200-140">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c9200-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="c9200-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="c9200-141">installIntent</span></span>|[<span data-ttu-id="c9200-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="c9200-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="c9200-143">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="c9200-143">The install intent for eBook.</span></span> <span data-ttu-id="c9200-144">Наследуется от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c9200-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="c9200-145">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="c9200-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="c9200-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9200-146">Response</span></span>
<span data-ttu-id="c9200-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9200-147">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9200-148">Пример</span><span class="sxs-lookup"><span data-stu-id="c9200-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9200-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9200-149">Request</span></span>
<span data-ttu-id="c9200-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9200-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="c9200-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9200-151">Response</span></span>
<span data-ttu-id="c9200-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9200-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



