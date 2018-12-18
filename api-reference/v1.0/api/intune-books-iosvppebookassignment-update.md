---
title: Обновление объекта iosVppEBookAssignment
description: Обновление свойств объекта iosVppEBookAssignment.
author: tfitzmac
ms.openlocfilehash: 8a4970b41cae2ab164a1164970d15d0a8afec344
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330536"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="d66c1-103">Обновление объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="d66c1-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="d66c1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d66c1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d66c1-105">Обновление свойств объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d66c1-105">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d66c1-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d66c1-106">Prerequisites</span></span>
<span data-ttu-id="d66c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d66c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d66c1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d66c1-109">Permission type</span></span>|<span data-ttu-id="d66c1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d66c1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d66c1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d66c1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d66c1-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d66c1-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d66c1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d66c1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d66c1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d66c1-114">Not supported.</span></span>|
|<span data-ttu-id="d66c1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d66c1-115">Application</span></span>|<span data-ttu-id="d66c1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d66c1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d66c1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d66c1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d66c1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d66c1-118">Request headers</span></span>
|<span data-ttu-id="d66c1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d66c1-119">Header</span></span>|<span data-ttu-id="d66c1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d66c1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d66c1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d66c1-121">Authorization</span></span>|<span data-ttu-id="d66c1-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d66c1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d66c1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d66c1-123">Accept</span></span>|<span data-ttu-id="d66c1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d66c1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d66c1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d66c1-125">Request body</span></span>
<span data-ttu-id="d66c1-126">В тексте запроса добавьте представление объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d66c1-126">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="d66c1-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d66c1-127">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="d66c1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d66c1-128">Property</span></span>|<span data-ttu-id="d66c1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d66c1-129">Type</span></span>|<span data-ttu-id="d66c1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d66c1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d66c1-131">id</span><span class="sxs-lookup"><span data-stu-id="d66c1-131">id</span></span>|<span data-ttu-id="d66c1-132">Строка</span><span class="sxs-lookup"><span data-stu-id="d66c1-132">String</span></span>|<span data-ttu-id="d66c1-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d66c1-133">Key of the entity.</span></span> <span data-ttu-id="d66c1-134">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d66c1-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="d66c1-135">target</span><span class="sxs-lookup"><span data-stu-id="d66c1-135">target</span></span>|[<span data-ttu-id="d66c1-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d66c1-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d66c1-137">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="d66c1-137">The assignment target for eBook.</span></span> <span data-ttu-id="d66c1-138">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d66c1-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="d66c1-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="d66c1-139">installIntent</span></span>|[<span data-ttu-id="d66c1-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="d66c1-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="d66c1-141">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="d66c1-141">The install intent for eBook.</span></span> <span data-ttu-id="d66c1-142">Наследуется от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d66c1-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="d66c1-143">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="d66c1-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="d66c1-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d66c1-144">Response</span></span>
<span data-ttu-id="d66c1-145">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d66c1-145">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d66c1-146">Пример</span><span class="sxs-lookup"><span data-stu-id="d66c1-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="d66c1-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="d66c1-147">Request</span></span>
<span data-ttu-id="d66c1-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d66c1-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="d66c1-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="d66c1-149">Response</span></span>
<span data-ttu-id="d66c1-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d66c1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



