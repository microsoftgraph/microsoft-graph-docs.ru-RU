---
title: Создание объекта managedEBookAssignment
description: Создание объекта managedEBookAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a6ee0c8e3e7538c761754b94b3b2f38bc277c65f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444527"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="13be7-103">Создание объекта managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="13be7-103">Create managedEBookAssignment</span></span>

<span data-ttu-id="13be7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="13be7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13be7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13be7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13be7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13be7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13be7-107">Создание объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="13be7-107">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13be7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="13be7-108">Prerequisites</span></span>
<span data-ttu-id="13be7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13be7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13be7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13be7-111">Permission type</span></span>|<span data-ttu-id="13be7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13be7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13be7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13be7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13be7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13be7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="13be7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13be7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13be7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13be7-116">Not supported.</span></span>|
|<span data-ttu-id="13be7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13be7-117">Application</span></span>|<span data-ttu-id="13be7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13be7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13be7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13be7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="13be7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="13be7-120">Request headers</span></span>
|<span data-ttu-id="13be7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13be7-121">Header</span></span>|<span data-ttu-id="13be7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="13be7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13be7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="13be7-123">Authorization</span></span>|<span data-ttu-id="13be7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13be7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13be7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="13be7-125">Accept</span></span>|<span data-ttu-id="13be7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13be7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13be7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13be7-127">Request body</span></span>
<span data-ttu-id="13be7-128">В тексте запроса добавьте представление объекта managedEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13be7-128">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="13be7-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="13be7-129">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="13be7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="13be7-130">Property</span></span>|<span data-ttu-id="13be7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="13be7-131">Type</span></span>|<span data-ttu-id="13be7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="13be7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13be7-133">id</span><span class="sxs-lookup"><span data-stu-id="13be7-133">id</span></span>|<span data-ttu-id="13be7-134">String</span><span class="sxs-lookup"><span data-stu-id="13be7-134">String</span></span>|<span data-ttu-id="13be7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="13be7-135">Key of the entity.</span></span>|
|<span data-ttu-id="13be7-136">target</span><span class="sxs-lookup"><span data-stu-id="13be7-136">target</span></span>|[<span data-ttu-id="13be7-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="13be7-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="13be7-138">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="13be7-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="13be7-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="13be7-139">installIntent</span></span>|[<span data-ttu-id="13be7-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="13be7-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="13be7-141">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="13be7-141">The install intent for eBook.</span></span> <span data-ttu-id="13be7-142">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="13be7-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="13be7-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="13be7-143">Response</span></span>
<span data-ttu-id="13be7-144">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13be7-144">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13be7-145">Пример</span><span class="sxs-lookup"><span data-stu-id="13be7-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="13be7-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="13be7-146">Request</span></span>
<span data-ttu-id="13be7-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13be7-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="13be7-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="13be7-148">Response</span></span>
<span data-ttu-id="13be7-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13be7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





