---
title: Создание объекта iosVppEBookAssignment
description: Создание объекта iosVppEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 81a88452e5c8fb930230fa6c7c961ffabcbf7302
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49245293"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="d0f04-103">Создание объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="d0f04-103">Create iosVppEBookAssignment</span></span>

<span data-ttu-id="d0f04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0f04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0f04-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0f04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0f04-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0f04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0f04-107">Создание объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d0f04-107">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0f04-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d0f04-108">Prerequisites</span></span>
<span data-ttu-id="d0f04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0f04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0f04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0f04-111">Permission type</span></span>|<span data-ttu-id="d0f04-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0f04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0f04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0f04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d0f04-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0f04-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d0f04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0f04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0f04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0f04-116">Not supported.</span></span>|
|<span data-ttu-id="d0f04-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d0f04-117">Application</span></span>|<span data-ttu-id="d0f04-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0f04-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0f04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0f04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d0f04-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d0f04-120">Request headers</span></span>
|<span data-ttu-id="d0f04-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0f04-121">Header</span></span>|<span data-ttu-id="d0f04-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d0f04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0f04-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0f04-123">Authorization</span></span>|<span data-ttu-id="d0f04-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0f04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0f04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d0f04-125">Accept</span></span>|<span data-ttu-id="d0f04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0f04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0f04-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0f04-127">Request body</span></span>
<span data-ttu-id="d0f04-128">В тексте запроса добавьте представление объекта iosVppEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0f04-128">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="d0f04-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="d0f04-129">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="d0f04-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0f04-130">Property</span></span>|<span data-ttu-id="d0f04-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d0f04-131">Type</span></span>|<span data-ttu-id="d0f04-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d0f04-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0f04-133">id</span><span class="sxs-lookup"><span data-stu-id="d0f04-133">id</span></span>|<span data-ttu-id="d0f04-134">String</span><span class="sxs-lookup"><span data-stu-id="d0f04-134">String</span></span>|<span data-ttu-id="d0f04-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d0f04-135">Key of the entity.</span></span> <span data-ttu-id="d0f04-136">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d0f04-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="d0f04-137">target</span><span class="sxs-lookup"><span data-stu-id="d0f04-137">target</span></span>|[<span data-ttu-id="d0f04-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d0f04-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d0f04-139">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="d0f04-139">The assignment target for eBook.</span></span> <span data-ttu-id="d0f04-140">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d0f04-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="d0f04-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="d0f04-141">installIntent</span></span>|[<span data-ttu-id="d0f04-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="d0f04-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="d0f04-143">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="d0f04-143">The install intent for eBook.</span></span> <span data-ttu-id="d0f04-144">Наследуется от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d0f04-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="d0f04-145">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="d0f04-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="d0f04-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0f04-146">Response</span></span>
<span data-ttu-id="d0f04-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d0f04-147">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0f04-148">Пример</span><span class="sxs-lookup"><span data-stu-id="d0f04-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0f04-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0f04-149">Request</span></span>
<span data-ttu-id="d0f04-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0f04-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d0f04-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0f04-151">Response</span></span>
<span data-ttu-id="d0f04-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0f04-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




