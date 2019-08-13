---
title: Обновление объекта managedEBookAssignment
description: Обновление свойств объекта managedEBookAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 708a7aa3266e67d62ce540c3f5e2f22b8154912b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335944"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="066f2-103">Обновление объекта managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="066f2-103">Update managedEBookAssignment</span></span>

> <span data-ttu-id="066f2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="066f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="066f2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="066f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="066f2-106">Обновление свойств объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="066f2-106">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="066f2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="066f2-107">Prerequisites</span></span>
<span data-ttu-id="066f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="066f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="066f2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="066f2-110">Permission type</span></span>|<span data-ttu-id="066f2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="066f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="066f2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="066f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="066f2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="066f2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="066f2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="066f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="066f2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="066f2-115">Not supported.</span></span>|
|<span data-ttu-id="066f2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="066f2-116">Application</span></span>|<span data-ttu-id="066f2-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="066f2-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="066f2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="066f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="066f2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="066f2-119">Request headers</span></span>
|<span data-ttu-id="066f2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="066f2-120">Header</span></span>|<span data-ttu-id="066f2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="066f2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="066f2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="066f2-122">Authorization</span></span>|<span data-ttu-id="066f2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="066f2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="066f2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="066f2-124">Accept</span></span>|<span data-ttu-id="066f2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="066f2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="066f2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="066f2-126">Request body</span></span>
<span data-ttu-id="066f2-127">В тексте запроса добавьте представление объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="066f2-127">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="066f2-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="066f2-128">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="066f2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="066f2-129">Property</span></span>|<span data-ttu-id="066f2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="066f2-130">Type</span></span>|<span data-ttu-id="066f2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="066f2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="066f2-132">id</span><span class="sxs-lookup"><span data-stu-id="066f2-132">id</span></span>|<span data-ttu-id="066f2-133">String</span><span class="sxs-lookup"><span data-stu-id="066f2-133">String</span></span>|<span data-ttu-id="066f2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="066f2-134">Key of the entity.</span></span>|
|<span data-ttu-id="066f2-135">target</span><span class="sxs-lookup"><span data-stu-id="066f2-135">target</span></span>|[<span data-ttu-id="066f2-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="066f2-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="066f2-137">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="066f2-137">The assignment target for eBook.</span></span>|
|<span data-ttu-id="066f2-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="066f2-138">installIntent</span></span>|[<span data-ttu-id="066f2-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="066f2-139">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="066f2-140">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="066f2-140">The install intent for eBook.</span></span> <span data-ttu-id="066f2-141">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="066f2-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="066f2-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="066f2-142">Response</span></span>
<span data-ttu-id="066f2-143">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="066f2-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="066f2-144">Пример</span><span class="sxs-lookup"><span data-stu-id="066f2-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="066f2-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="066f2-145">Request</span></span>
<span data-ttu-id="066f2-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="066f2-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 194

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="066f2-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="066f2-147">Response</span></span>
<span data-ttu-id="066f2-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="066f2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```






