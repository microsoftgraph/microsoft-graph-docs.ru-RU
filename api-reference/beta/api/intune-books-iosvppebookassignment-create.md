---
title: Создание объекта iosVppEBookAssignment
description: Создание объекта iosVppEBookAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b8170738d48811d8d4b9a1e672d6284fcb115f76
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760475"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="ef27e-103">Создание объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="ef27e-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="ef27e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef27e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef27e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef27e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef27e-106">Создание объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ef27e-106">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef27e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ef27e-107">Prerequisites</span></span>
<span data-ttu-id="ef27e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef27e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef27e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef27e-110">Permission type</span></span>|<span data-ttu-id="ef27e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef27e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef27e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef27e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef27e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef27e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ef27e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef27e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef27e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef27e-115">Not supported.</span></span>|
|<span data-ttu-id="ef27e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ef27e-116">Application</span></span>|<span data-ttu-id="ef27e-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef27e-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef27e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef27e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ef27e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ef27e-119">Request headers</span></span>
|<span data-ttu-id="ef27e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef27e-120">Header</span></span>|<span data-ttu-id="ef27e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ef27e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef27e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef27e-122">Authorization</span></span>|<span data-ttu-id="ef27e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef27e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef27e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ef27e-124">Accept</span></span>|<span data-ttu-id="ef27e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef27e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef27e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef27e-126">Request body</span></span>
<span data-ttu-id="ef27e-127">В тексте запроса добавьте представление объекта iosVppEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef27e-127">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="ef27e-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="ef27e-128">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="ef27e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef27e-129">Property</span></span>|<span data-ttu-id="ef27e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ef27e-130">Type</span></span>|<span data-ttu-id="ef27e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ef27e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef27e-132">id</span><span class="sxs-lookup"><span data-stu-id="ef27e-132">id</span></span>|<span data-ttu-id="ef27e-133">String</span><span class="sxs-lookup"><span data-stu-id="ef27e-133">String</span></span>|<span data-ttu-id="ef27e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ef27e-134">Key of the entity.</span></span> <span data-ttu-id="ef27e-135">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ef27e-135">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="ef27e-136">target</span><span class="sxs-lookup"><span data-stu-id="ef27e-136">target</span></span>|[<span data-ttu-id="ef27e-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ef27e-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ef27e-138">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ef27e-138">The assignment target for eBook.</span></span> <span data-ttu-id="ef27e-139">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ef27e-139">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="ef27e-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="ef27e-140">installIntent</span></span>|[<span data-ttu-id="ef27e-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="ef27e-141">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="ef27e-142">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ef27e-142">The install intent for eBook.</span></span> <span data-ttu-id="ef27e-143">Наследуется от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ef27e-143">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="ef27e-144">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="ef27e-144">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="ef27e-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef27e-145">Response</span></span>
<span data-ttu-id="ef27e-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ef27e-146">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef27e-147">Пример</span><span class="sxs-lookup"><span data-stu-id="ef27e-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef27e-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef27e-148">Request</span></span>
<span data-ttu-id="ef27e-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef27e-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="ef27e-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef27e-150">Response</span></span>
<span data-ttu-id="ef27e-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef27e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




