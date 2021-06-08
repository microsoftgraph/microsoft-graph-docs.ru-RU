---
title: Создание объекта managedEBookAssignment
description: Создание объекта managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 881c22ada3a6a4484628a8f5606029cc7f6c4ece
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757264"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="7f15d-103">Создание объекта managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="7f15d-103">Create managedEBookAssignment</span></span>

<span data-ttu-id="7f15d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f15d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f15d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f15d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f15d-106">Создание объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7f15d-106">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f15d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7f15d-107">Prerequisites</span></span>
<span data-ttu-id="7f15d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f15d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f15d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f15d-110">Permission type</span></span>|<span data-ttu-id="7f15d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f15d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f15d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f15d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f15d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f15d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7f15d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f15d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f15d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f15d-115">Not supported.</span></span>|
|<span data-ttu-id="7f15d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7f15d-116">Application</span></span>|<span data-ttu-id="7f15d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f15d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f15d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f15d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7f15d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7f15d-119">Request headers</span></span>
|<span data-ttu-id="7f15d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f15d-120">Header</span></span>|<span data-ttu-id="7f15d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7f15d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f15d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f15d-122">Authorization</span></span>|<span data-ttu-id="7f15d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f15d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f15d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7f15d-124">Accept</span></span>|<span data-ttu-id="7f15d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7f15d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f15d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f15d-126">Request body</span></span>
<span data-ttu-id="7f15d-127">В тексте запроса добавьте представление объекта managedEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f15d-127">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="7f15d-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="7f15d-128">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="7f15d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f15d-129">Property</span></span>|<span data-ttu-id="7f15d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7f15d-130">Type</span></span>|<span data-ttu-id="7f15d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7f15d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f15d-132">id</span><span class="sxs-lookup"><span data-stu-id="7f15d-132">id</span></span>|<span data-ttu-id="7f15d-133">String</span><span class="sxs-lookup"><span data-stu-id="7f15d-133">String</span></span>|<span data-ttu-id="7f15d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7f15d-134">Key of the entity.</span></span>|
|<span data-ttu-id="7f15d-135">target</span><span class="sxs-lookup"><span data-stu-id="7f15d-135">target</span></span>|[<span data-ttu-id="7f15d-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7f15d-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7f15d-137">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="7f15d-137">The assignment target for eBook.</span></span>|
|<span data-ttu-id="7f15d-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="7f15d-138">installIntent</span></span>|[<span data-ttu-id="7f15d-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="7f15d-139">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="7f15d-140">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="7f15d-140">The install intent for eBook.</span></span> <span data-ttu-id="7f15d-141">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="7f15d-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="7f15d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f15d-142">Response</span></span>
<span data-ttu-id="7f15d-143">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f15d-143">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f15d-144">Пример</span><span class="sxs-lookup"><span data-stu-id="7f15d-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f15d-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f15d-145">Request</span></span>
<span data-ttu-id="7f15d-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f15d-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 188

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="7f15d-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f15d-147">Response</span></span>
<span data-ttu-id="7f15d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f15d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 237

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "installIntent": "required"
}
```




