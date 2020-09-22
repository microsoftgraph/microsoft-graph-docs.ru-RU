---
title: Обновление объекта managedEBookAssignment
description: Обновление свойств объекта managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 25088846f815054501f1ee0b87265a17f34ea014
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48077823"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="bffa6-103">Обновление объекта managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="bffa6-103">Update managedEBookAssignment</span></span>

<span data-ttu-id="bffa6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bffa6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bffa6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bffa6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bffa6-106">Обновление свойств объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bffa6-106">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bffa6-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bffa6-107">Prerequisites</span></span>
<span data-ttu-id="bffa6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bffa6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bffa6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bffa6-110">Permission type</span></span>|<span data-ttu-id="bffa6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bffa6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bffa6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bffa6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bffa6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bffa6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bffa6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bffa6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bffa6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bffa6-115">Not supported.</span></span>|
|<span data-ttu-id="bffa6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bffa6-116">Application</span></span>|<span data-ttu-id="bffa6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bffa6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bffa6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bffa6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="bffa6-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bffa6-119">Request headers</span></span>
|<span data-ttu-id="bffa6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bffa6-120">Header</span></span>|<span data-ttu-id="bffa6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bffa6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bffa6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bffa6-122">Authorization</span></span>|<span data-ttu-id="bffa6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bffa6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bffa6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bffa6-124">Accept</span></span>|<span data-ttu-id="bffa6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bffa6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bffa6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bffa6-126">Request body</span></span>
<span data-ttu-id="bffa6-127">В тексте запроса добавьте представление объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bffa6-127">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="bffa6-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bffa6-128">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="bffa6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bffa6-129">Property</span></span>|<span data-ttu-id="bffa6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bffa6-130">Type</span></span>|<span data-ttu-id="bffa6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bffa6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bffa6-132">id</span><span class="sxs-lookup"><span data-stu-id="bffa6-132">id</span></span>|<span data-ttu-id="bffa6-133">Строка</span><span class="sxs-lookup"><span data-stu-id="bffa6-133">String</span></span>|<span data-ttu-id="bffa6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bffa6-134">Key of the entity.</span></span>|
|<span data-ttu-id="bffa6-135">target</span><span class="sxs-lookup"><span data-stu-id="bffa6-135">target</span></span>|[<span data-ttu-id="bffa6-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bffa6-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bffa6-137">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="bffa6-137">The assignment target for eBook.</span></span>|
|<span data-ttu-id="bffa6-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="bffa6-138">installIntent</span></span>|[<span data-ttu-id="bffa6-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="bffa6-139">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="bffa6-140">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="bffa6-140">The install intent for eBook.</span></span> <span data-ttu-id="bffa6-141">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="bffa6-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="bffa6-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="bffa6-142">Response</span></span>
<span data-ttu-id="bffa6-143">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bffa6-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bffa6-144">Пример</span><span class="sxs-lookup"><span data-stu-id="bffa6-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="bffa6-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="bffa6-145">Request</span></span>
<span data-ttu-id="bffa6-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bffa6-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="bffa6-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="bffa6-147">Response</span></span>
<span data-ttu-id="bffa6-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bffa6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









