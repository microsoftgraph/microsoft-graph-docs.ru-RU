---
title: Создание объекта iosVppEBookAssignment
description: Создание объекта iosVppEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 56a560c45be3c1932636c988c11359125469b6b3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013586"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="774a0-103">Создание объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="774a0-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="774a0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="774a0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="774a0-105">Создание объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="774a0-105">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="774a0-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="774a0-106">Prerequisites</span></span>
<span data-ttu-id="774a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="774a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="774a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="774a0-109">Permission type</span></span>|<span data-ttu-id="774a0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="774a0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="774a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="774a0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="774a0-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="774a0-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="774a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="774a0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="774a0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="774a0-114">Not supported.</span></span>|
|<span data-ttu-id="774a0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="774a0-115">Application</span></span>|<span data-ttu-id="774a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="774a0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="774a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="774a0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="774a0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="774a0-118">Request headers</span></span>
|<span data-ttu-id="774a0-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="774a0-119">Header</span></span>|<span data-ttu-id="774a0-120">Значение</span><span class="sxs-lookup"><span data-stu-id="774a0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="774a0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="774a0-121">Authorization</span></span>|<span data-ttu-id="774a0-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="774a0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="774a0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="774a0-123">Accept</span></span>|<span data-ttu-id="774a0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="774a0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="774a0-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="774a0-125">Request body</span></span>
<span data-ttu-id="774a0-126">В тексте запроса добавьте представление объекта iosVppEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="774a0-126">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="774a0-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="774a0-127">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="774a0-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="774a0-128">Property</span></span>|<span data-ttu-id="774a0-129">Тип</span><span class="sxs-lookup"><span data-stu-id="774a0-129">Type</span></span>|<span data-ttu-id="774a0-130">Описание</span><span class="sxs-lookup"><span data-stu-id="774a0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="774a0-131">id</span><span class="sxs-lookup"><span data-stu-id="774a0-131">id</span></span>|<span data-ttu-id="774a0-132">String</span><span class="sxs-lookup"><span data-stu-id="774a0-132">String</span></span>|<span data-ttu-id="774a0-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="774a0-133">Key of the entity.</span></span> <span data-ttu-id="774a0-134">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="774a0-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="774a0-135">target</span><span class="sxs-lookup"><span data-stu-id="774a0-135">target</span></span>|[<span data-ttu-id="774a0-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="774a0-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="774a0-137">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="774a0-137">The assignment target for eBook.</span></span> <span data-ttu-id="774a0-138">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="774a0-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="774a0-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="774a0-139">installIntent</span></span>|[<span data-ttu-id="774a0-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="774a0-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="774a0-141">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="774a0-141">The install intent for eBook.</span></span> <span data-ttu-id="774a0-142">Наследуется от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="774a0-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="774a0-143">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="774a0-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="774a0-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="774a0-144">Response</span></span>
<span data-ttu-id="774a0-145">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="774a0-145">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="774a0-146">Пример</span><span class="sxs-lookup"><span data-stu-id="774a0-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="774a0-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="774a0-147">Request</span></span>
<span data-ttu-id="774a0-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="774a0-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="774a0-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="774a0-149">Response</span></span>
<span data-ttu-id="774a0-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="774a0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



