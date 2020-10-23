---
title: Создание объекта managedEBookAssignment
description: Создание объекта managedEBookAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f4e158b901440683c7a5f3b6ff8c3e965110f087
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731446"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="75fdc-103">Создание объекта managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="75fdc-103">Create managedEBookAssignment</span></span>

<span data-ttu-id="75fdc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75fdc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75fdc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75fdc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75fdc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75fdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75fdc-107">Создание объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="75fdc-107">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75fdc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="75fdc-108">Prerequisites</span></span>
<span data-ttu-id="75fdc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75fdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75fdc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75fdc-111">Permission type</span></span>|<span data-ttu-id="75fdc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75fdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75fdc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75fdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75fdc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75fdc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="75fdc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75fdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75fdc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75fdc-116">Not supported.</span></span>|
|<span data-ttu-id="75fdc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75fdc-117">Application</span></span>|<span data-ttu-id="75fdc-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75fdc-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75fdc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75fdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="75fdc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="75fdc-120">Request headers</span></span>
|<span data-ttu-id="75fdc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75fdc-121">Header</span></span>|<span data-ttu-id="75fdc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="75fdc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75fdc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75fdc-123">Authorization</span></span>|<span data-ttu-id="75fdc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75fdc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75fdc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="75fdc-125">Accept</span></span>|<span data-ttu-id="75fdc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75fdc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75fdc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="75fdc-127">Request body</span></span>
<span data-ttu-id="75fdc-128">В тексте запроса добавьте представление объекта managedEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75fdc-128">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="75fdc-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="75fdc-129">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="75fdc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="75fdc-130">Property</span></span>|<span data-ttu-id="75fdc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="75fdc-131">Type</span></span>|<span data-ttu-id="75fdc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="75fdc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75fdc-133">id</span><span class="sxs-lookup"><span data-stu-id="75fdc-133">id</span></span>|<span data-ttu-id="75fdc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="75fdc-134">String</span></span>|<span data-ttu-id="75fdc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="75fdc-135">Key of the entity.</span></span>|
|<span data-ttu-id="75fdc-136">target</span><span class="sxs-lookup"><span data-stu-id="75fdc-136">target</span></span>|[<span data-ttu-id="75fdc-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="75fdc-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="75fdc-138">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="75fdc-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="75fdc-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="75fdc-139">installIntent</span></span>|[<span data-ttu-id="75fdc-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="75fdc-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="75fdc-141">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="75fdc-141">The install intent for eBook.</span></span> <span data-ttu-id="75fdc-142">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="75fdc-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="75fdc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="75fdc-143">Response</span></span>
<span data-ttu-id="75fdc-144">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75fdc-144">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75fdc-145">Пример</span><span class="sxs-lookup"><span data-stu-id="75fdc-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="75fdc-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="75fdc-146">Request</span></span>
<span data-ttu-id="75fdc-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75fdc-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 355

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="75fdc-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="75fdc-148">Response</span></span>
<span data-ttu-id="75fdc-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75fdc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 404

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "installIntent": "required"
}
```





