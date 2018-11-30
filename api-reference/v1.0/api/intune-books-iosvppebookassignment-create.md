---
title: Создание объекта iosVppEBookAssignment
description: Создание объекта iosVppEBookAssignment.
ms.openlocfilehash: 2b8dd451ae44267c792bf548ecdca27b2fb6d55e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024692"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="7377e-103">Создание объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="7377e-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="7377e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7377e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7377e-105">Создание объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7377e-105">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7377e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7377e-106">Prerequisites</span></span>
<span data-ttu-id="7377e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7377e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7377e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7377e-109">Permission type</span></span>|<span data-ttu-id="7377e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7377e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7377e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7377e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7377e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7377e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7377e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7377e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7377e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7377e-114">Not supported.</span></span>|
|<span data-ttu-id="7377e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7377e-115">Application</span></span>|<span data-ttu-id="7377e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7377e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7377e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7377e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7377e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7377e-118">Request headers</span></span>
|<span data-ttu-id="7377e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7377e-119">Header</span></span>|<span data-ttu-id="7377e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7377e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7377e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7377e-121">Authorization</span></span>|<span data-ttu-id="7377e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7377e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7377e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7377e-123">Accept</span></span>|<span data-ttu-id="7377e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7377e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7377e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7377e-125">Request body</span></span>
<span data-ttu-id="7377e-126">В тексте запроса добавьте представление объекта iosVppEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7377e-126">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="7377e-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="7377e-127">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="7377e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7377e-128">Property</span></span>|<span data-ttu-id="7377e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7377e-129">Type</span></span>|<span data-ttu-id="7377e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7377e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7377e-131">id</span><span class="sxs-lookup"><span data-stu-id="7377e-131">id</span></span>|<span data-ttu-id="7377e-132">String</span><span class="sxs-lookup"><span data-stu-id="7377e-132">String</span></span>|<span data-ttu-id="7377e-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7377e-133">Key of the entity.</span></span> <span data-ttu-id="7377e-134">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7377e-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="7377e-135">target</span><span class="sxs-lookup"><span data-stu-id="7377e-135">target</span></span>|[<span data-ttu-id="7377e-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7377e-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7377e-137">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="7377e-137">The assignment target for eBook.</span></span> <span data-ttu-id="7377e-138">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7377e-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="7377e-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="7377e-139">installIntent</span></span>|[<span data-ttu-id="7377e-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="7377e-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="7377e-141">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="7377e-141">The install intent for eBook.</span></span> <span data-ttu-id="7377e-142">Наследуется от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="7377e-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="7377e-143">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="7377e-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="7377e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7377e-144">Response</span></span>
<span data-ttu-id="7377e-145">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7377e-145">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7377e-146">Пример</span><span class="sxs-lookup"><span data-stu-id="7377e-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="7377e-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="7377e-147">Request</span></span>
<span data-ttu-id="7377e-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7377e-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7377e-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="7377e-149">Response</span></span>
<span data-ttu-id="7377e-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7377e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



