---
title: Обновление объекта managedEBookAssignment
description: Обновление свойств объекта managedEBookAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14a351ffce07f18e82fefd59bd822523f03b7250
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444576"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="535ce-103">Обновление объекта managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="535ce-103">Update managedEBookAssignment</span></span>

<span data-ttu-id="535ce-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="535ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="535ce-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="535ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="535ce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="535ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="535ce-107">Обновление свойств объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="535ce-107">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="535ce-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="535ce-108">Prerequisites</span></span>
<span data-ttu-id="535ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="535ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="535ce-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="535ce-111">Permission type</span></span>|<span data-ttu-id="535ce-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="535ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="535ce-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="535ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="535ce-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="535ce-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="535ce-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="535ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="535ce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="535ce-116">Not supported.</span></span>|
|<span data-ttu-id="535ce-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="535ce-117">Application</span></span>|<span data-ttu-id="535ce-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="535ce-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="535ce-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="535ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="535ce-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="535ce-120">Request headers</span></span>
|<span data-ttu-id="535ce-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="535ce-121">Header</span></span>|<span data-ttu-id="535ce-122">Значение</span><span class="sxs-lookup"><span data-stu-id="535ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="535ce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="535ce-123">Authorization</span></span>|<span data-ttu-id="535ce-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="535ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="535ce-125">Accept</span><span class="sxs-lookup"><span data-stu-id="535ce-125">Accept</span></span>|<span data-ttu-id="535ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="535ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="535ce-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="535ce-127">Request body</span></span>
<span data-ttu-id="535ce-128">В тексте запроса добавьте представление объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="535ce-128">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="535ce-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="535ce-129">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="535ce-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="535ce-130">Property</span></span>|<span data-ttu-id="535ce-131">Тип</span><span class="sxs-lookup"><span data-stu-id="535ce-131">Type</span></span>|<span data-ttu-id="535ce-132">Описание</span><span class="sxs-lookup"><span data-stu-id="535ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="535ce-133">id</span><span class="sxs-lookup"><span data-stu-id="535ce-133">id</span></span>|<span data-ttu-id="535ce-134">String</span><span class="sxs-lookup"><span data-stu-id="535ce-134">String</span></span>|<span data-ttu-id="535ce-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="535ce-135">Key of the entity.</span></span>|
|<span data-ttu-id="535ce-136">target</span><span class="sxs-lookup"><span data-stu-id="535ce-136">target</span></span>|[<span data-ttu-id="535ce-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="535ce-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="535ce-138">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="535ce-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="535ce-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="535ce-139">installIntent</span></span>|[<span data-ttu-id="535ce-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="535ce-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="535ce-141">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="535ce-141">The install intent for eBook.</span></span> <span data-ttu-id="535ce-142">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="535ce-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="535ce-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="535ce-143">Response</span></span>
<span data-ttu-id="535ce-144">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="535ce-144">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="535ce-145">Пример</span><span class="sxs-lookup"><span data-stu-id="535ce-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="535ce-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="535ce-146">Request</span></span>
<span data-ttu-id="535ce-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="535ce-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="535ce-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="535ce-148">Response</span></span>
<span data-ttu-id="535ce-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="535ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





