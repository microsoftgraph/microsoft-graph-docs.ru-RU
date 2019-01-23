---
title: Обновление объекта iosVppEBookAssignment
description: Обновление свойств объекта iosVppEBookAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0ad070245ee687d08e4b636d7ef6301c42f1a586
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405816"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="ccbd1-103">Обновление объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="ccbd1-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="ccbd1-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ccbd1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ccbd1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccbd1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ccbd1-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ccbd1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccbd1-107">Обновление свойств объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ccbd1-107">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccbd1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ccbd1-108">Prerequisites</span></span>
<span data-ttu-id="ccbd1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ccbd1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ccbd1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccbd1-111">Permission type</span></span>|<span data-ttu-id="ccbd1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccbd1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccbd1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccbd1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ccbd1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccbd1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ccbd1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccbd1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccbd1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccbd1-116">Not supported.</span></span>|
|<span data-ttu-id="ccbd1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccbd1-117">Application</span></span>|<span data-ttu-id="ccbd1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccbd1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccbd1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccbd1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ccbd1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccbd1-120">Request headers</span></span>
|<span data-ttu-id="ccbd1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ccbd1-121">Header</span></span>|<span data-ttu-id="ccbd1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ccbd1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccbd1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccbd1-123">Authorization</span></span>|<span data-ttu-id="ccbd1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ccbd1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccbd1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ccbd1-125">Accept</span></span>|<span data-ttu-id="ccbd1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ccbd1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccbd1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ccbd1-127">Request body</span></span>
<span data-ttu-id="ccbd1-128">В тексте запроса добавьте представление объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccbd1-128">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="ccbd1-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ccbd1-129">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="ccbd1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccbd1-130">Property</span></span>|<span data-ttu-id="ccbd1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ccbd1-131">Type</span></span>|<span data-ttu-id="ccbd1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ccbd1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccbd1-133">id</span><span class="sxs-lookup"><span data-stu-id="ccbd1-133">id</span></span>|<span data-ttu-id="ccbd1-134">String</span><span class="sxs-lookup"><span data-stu-id="ccbd1-134">String</span></span>|<span data-ttu-id="ccbd1-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ccbd1-135">Key of the entity.</span></span> <span data-ttu-id="ccbd1-136">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ccbd1-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="ccbd1-137">target</span><span class="sxs-lookup"><span data-stu-id="ccbd1-137">target</span></span>|[<span data-ttu-id="ccbd1-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ccbd1-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ccbd1-139">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ccbd1-139">The assignment target for eBook.</span></span> <span data-ttu-id="ccbd1-140">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ccbd1-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="ccbd1-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="ccbd1-141">installIntent</span></span>|[<span data-ttu-id="ccbd1-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="ccbd1-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="ccbd1-143">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ccbd1-143">The install intent for eBook.</span></span> <span data-ttu-id="ccbd1-144">Наследуется от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ccbd1-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="ccbd1-145">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="ccbd1-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="ccbd1-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccbd1-146">Response</span></span>
<span data-ttu-id="ccbd1-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ccbd1-147">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccbd1-148">Пример</span><span class="sxs-lookup"><span data-stu-id="ccbd1-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccbd1-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccbd1-149">Request</span></span>
<span data-ttu-id="ccbd1-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccbd1-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="ccbd1-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccbd1-151">Response</span></span>
<span data-ttu-id="ccbd1-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ccbd1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




