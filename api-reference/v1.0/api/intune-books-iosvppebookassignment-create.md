---
title: Создание объекта iosVppEBookAssignment
description: Создание объекта iosVppEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 38014d5ad851f44555dd637f62ae4923c12ee4bb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758444"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="cac9c-103">Создание объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="cac9c-103">Create iosVppEBookAssignment</span></span>

<span data-ttu-id="cac9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cac9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cac9c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cac9c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cac9c-106">Создание объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cac9c-106">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cac9c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cac9c-107">Prerequisites</span></span>
<span data-ttu-id="cac9c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cac9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cac9c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cac9c-110">Permission type</span></span>|<span data-ttu-id="cac9c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cac9c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cac9c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cac9c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cac9c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cac9c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cac9c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cac9c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cac9c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cac9c-115">Not supported.</span></span>|
|<span data-ttu-id="cac9c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="cac9c-116">Application</span></span>|<span data-ttu-id="cac9c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cac9c-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cac9c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cac9c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="cac9c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cac9c-119">Request headers</span></span>
|<span data-ttu-id="cac9c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cac9c-120">Header</span></span>|<span data-ttu-id="cac9c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cac9c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cac9c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cac9c-122">Authorization</span></span>|<span data-ttu-id="cac9c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cac9c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cac9c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cac9c-124">Accept</span></span>|<span data-ttu-id="cac9c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cac9c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cac9c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cac9c-126">Request body</span></span>
<span data-ttu-id="cac9c-127">В тексте запроса добавьте представление объекта iosVppEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cac9c-127">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="cac9c-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="cac9c-128">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="cac9c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cac9c-129">Property</span></span>|<span data-ttu-id="cac9c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cac9c-130">Type</span></span>|<span data-ttu-id="cac9c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cac9c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cac9c-132">id</span><span class="sxs-lookup"><span data-stu-id="cac9c-132">id</span></span>|<span data-ttu-id="cac9c-133">String</span><span class="sxs-lookup"><span data-stu-id="cac9c-133">String</span></span>|<span data-ttu-id="cac9c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cac9c-134">Key of the entity.</span></span> <span data-ttu-id="cac9c-135">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cac9c-135">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="cac9c-136">target</span><span class="sxs-lookup"><span data-stu-id="cac9c-136">target</span></span>|[<span data-ttu-id="cac9c-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cac9c-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cac9c-138">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="cac9c-138">The assignment target for eBook.</span></span> <span data-ttu-id="cac9c-139">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cac9c-139">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="cac9c-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="cac9c-140">installIntent</span></span>|[<span data-ttu-id="cac9c-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="cac9c-141">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="cac9c-142">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="cac9c-142">The install intent for eBook.</span></span> <span data-ttu-id="cac9c-143">Унаследованный от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cac9c-143">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="cac9c-144">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="cac9c-144">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="cac9c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="cac9c-145">Response</span></span>
<span data-ttu-id="cac9c-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cac9c-146">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cac9c-147">Пример</span><span class="sxs-lookup"><span data-stu-id="cac9c-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="cac9c-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="cac9c-148">Request</span></span>
<span data-ttu-id="cac9c-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cac9c-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="cac9c-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="cac9c-150">Response</span></span>
<span data-ttu-id="cac9c-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cac9c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




