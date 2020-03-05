---
title: Обновление объекта iosVppEBookAssignment
description: Обновление свойств объекта iosVppEBookAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 84dbd1fe337fab2ac4fb8084460429bdcff2ba9b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444548"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="093b0-103">Обновление объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="093b0-103">Update iosVppEBookAssignment</span></span>

<span data-ttu-id="093b0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="093b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="093b0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="093b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="093b0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="093b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="093b0-107">Обновление свойств объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="093b0-107">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="093b0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="093b0-108">Prerequisites</span></span>
<span data-ttu-id="093b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="093b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="093b0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="093b0-111">Permission type</span></span>|<span data-ttu-id="093b0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="093b0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="093b0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="093b0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="093b0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="093b0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="093b0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="093b0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="093b0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="093b0-116">Not supported.</span></span>|
|<span data-ttu-id="093b0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="093b0-117">Application</span></span>|<span data-ttu-id="093b0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="093b0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="093b0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="093b0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="093b0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="093b0-120">Request headers</span></span>
|<span data-ttu-id="093b0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="093b0-121">Header</span></span>|<span data-ttu-id="093b0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="093b0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="093b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="093b0-123">Authorization</span></span>|<span data-ttu-id="093b0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="093b0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="093b0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="093b0-125">Accept</span></span>|<span data-ttu-id="093b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="093b0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="093b0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="093b0-127">Request body</span></span>
<span data-ttu-id="093b0-128">В тексте запроса добавьте представление объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="093b0-128">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="093b0-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="093b0-129">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="093b0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="093b0-130">Property</span></span>|<span data-ttu-id="093b0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="093b0-131">Type</span></span>|<span data-ttu-id="093b0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="093b0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="093b0-133">id</span><span class="sxs-lookup"><span data-stu-id="093b0-133">id</span></span>|<span data-ttu-id="093b0-134">String</span><span class="sxs-lookup"><span data-stu-id="093b0-134">String</span></span>|<span data-ttu-id="093b0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="093b0-135">Key of the entity.</span></span> <span data-ttu-id="093b0-136">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="093b0-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="093b0-137">target</span><span class="sxs-lookup"><span data-stu-id="093b0-137">target</span></span>|[<span data-ttu-id="093b0-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="093b0-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="093b0-139">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="093b0-139">The assignment target for eBook.</span></span> <span data-ttu-id="093b0-140">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="093b0-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="093b0-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="093b0-141">installIntent</span></span>|[<span data-ttu-id="093b0-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="093b0-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="093b0-143">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="093b0-143">The install intent for eBook.</span></span> <span data-ttu-id="093b0-144">Наследуется от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="093b0-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="093b0-145">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="093b0-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="093b0-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="093b0-146">Response</span></span>
<span data-ttu-id="093b0-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="093b0-147">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="093b0-148">Пример</span><span class="sxs-lookup"><span data-stu-id="093b0-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="093b0-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="093b0-149">Request</span></span>
<span data-ttu-id="093b0-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="093b0-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="093b0-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="093b0-151">Response</span></span>
<span data-ttu-id="093b0-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="093b0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "48f05789-5789-48f0-8957-f0488957f048",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```





