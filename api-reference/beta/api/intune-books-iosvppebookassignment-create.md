---
title: Создание объекта iosVppEBookAssignment
description: Создание объекта iosVppEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a333b000b4e83a5afb50f0402b82dfa2f68778f7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793243"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="efadc-103">Создание объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="efadc-103">Create iosVppEBookAssignment</span></span>

<span data-ttu-id="efadc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efadc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efadc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efadc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efadc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="efadc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efadc-107">Создание объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="efadc-107">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efadc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="efadc-108">Prerequisites</span></span>
<span data-ttu-id="efadc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efadc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efadc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efadc-111">Permission type</span></span>|<span data-ttu-id="efadc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="efadc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efadc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efadc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="efadc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efadc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="efadc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efadc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efadc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efadc-116">Not supported.</span></span>|
|<span data-ttu-id="efadc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efadc-117">Application</span></span>|<span data-ttu-id="efadc-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efadc-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efadc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efadc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="efadc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="efadc-120">Request headers</span></span>
|<span data-ttu-id="efadc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="efadc-121">Header</span></span>|<span data-ttu-id="efadc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="efadc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efadc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efadc-123">Authorization</span></span>|<span data-ttu-id="efadc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="efadc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efadc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="efadc-125">Accept</span></span>|<span data-ttu-id="efadc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="efadc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efadc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="efadc-127">Request body</span></span>
<span data-ttu-id="efadc-128">В тексте запроса добавьте представление объекта iosVppEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efadc-128">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="efadc-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="efadc-129">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="efadc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="efadc-130">Property</span></span>|<span data-ttu-id="efadc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="efadc-131">Type</span></span>|<span data-ttu-id="efadc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="efadc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efadc-133">id</span><span class="sxs-lookup"><span data-stu-id="efadc-133">id</span></span>|<span data-ttu-id="efadc-134">String</span><span class="sxs-lookup"><span data-stu-id="efadc-134">String</span></span>|<span data-ttu-id="efadc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="efadc-135">Key of the entity.</span></span> <span data-ttu-id="efadc-136">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="efadc-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="efadc-137">target</span><span class="sxs-lookup"><span data-stu-id="efadc-137">target</span></span>|[<span data-ttu-id="efadc-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="efadc-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="efadc-139">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="efadc-139">The assignment target for eBook.</span></span> <span data-ttu-id="efadc-140">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="efadc-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="efadc-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="efadc-141">installIntent</span></span>|[<span data-ttu-id="efadc-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="efadc-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="efadc-143">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="efadc-143">The install intent for eBook.</span></span> <span data-ttu-id="efadc-144">Наследуется от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="efadc-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="efadc-145">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="efadc-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="efadc-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="efadc-146">Response</span></span>
<span data-ttu-id="efadc-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="efadc-147">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efadc-148">Пример</span><span class="sxs-lookup"><span data-stu-id="efadc-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="efadc-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="efadc-149">Request</span></span>
<span data-ttu-id="efadc-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efadc-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="efadc-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="efadc-151">Response</span></span>
<span data-ttu-id="efadc-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efadc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



