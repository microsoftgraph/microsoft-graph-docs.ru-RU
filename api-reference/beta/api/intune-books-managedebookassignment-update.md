---
title: Обновление объекта managedEBookAssignment
description: Обновление свойств объекта managedEBookAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0cf6aef49315eba7f6c67af34147a577a43a5a80
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413796"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="72eee-103">Обновление объекта managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="72eee-103">Update managedEBookAssignment</span></span>

> <span data-ttu-id="72eee-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="72eee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="72eee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72eee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72eee-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72eee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72eee-107">Обновление свойств объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="72eee-107">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72eee-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="72eee-108">Prerequisites</span></span>
<span data-ttu-id="72eee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="72eee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="72eee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72eee-111">Permission type</span></span>|<span data-ttu-id="72eee-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="72eee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72eee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72eee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72eee-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72eee-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="72eee-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72eee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72eee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72eee-116">Not supported.</span></span>|
|<span data-ttu-id="72eee-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72eee-117">Application</span></span>|<span data-ttu-id="72eee-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72eee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72eee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72eee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="72eee-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72eee-120">Request headers</span></span>
|<span data-ttu-id="72eee-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72eee-121">Header</span></span>|<span data-ttu-id="72eee-122">Значение</span><span class="sxs-lookup"><span data-stu-id="72eee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72eee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="72eee-123">Authorization</span></span>|<span data-ttu-id="72eee-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="72eee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72eee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="72eee-125">Accept</span></span>|<span data-ttu-id="72eee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72eee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72eee-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72eee-127">Request body</span></span>
<span data-ttu-id="72eee-128">В тексте запроса добавьте представление объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72eee-128">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="72eee-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="72eee-129">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="72eee-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="72eee-130">Property</span></span>|<span data-ttu-id="72eee-131">Тип</span><span class="sxs-lookup"><span data-stu-id="72eee-131">Type</span></span>|<span data-ttu-id="72eee-132">Описание</span><span class="sxs-lookup"><span data-stu-id="72eee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72eee-133">id</span><span class="sxs-lookup"><span data-stu-id="72eee-133">id</span></span>|<span data-ttu-id="72eee-134">String</span><span class="sxs-lookup"><span data-stu-id="72eee-134">String</span></span>|<span data-ttu-id="72eee-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="72eee-135">Key of the entity.</span></span>|
|<span data-ttu-id="72eee-136">target</span><span class="sxs-lookup"><span data-stu-id="72eee-136">target</span></span>|[<span data-ttu-id="72eee-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="72eee-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="72eee-138">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="72eee-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="72eee-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="72eee-139">installIntent</span></span>|[<span data-ttu-id="72eee-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="72eee-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="72eee-141">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="72eee-141">The install intent for eBook.</span></span> <span data-ttu-id="72eee-142">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="72eee-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="72eee-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="72eee-143">Response</span></span>
<span data-ttu-id="72eee-144">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72eee-144">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72eee-145">Пример</span><span class="sxs-lookup"><span data-stu-id="72eee-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="72eee-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="72eee-146">Request</span></span>
<span data-ttu-id="72eee-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72eee-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="72eee-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="72eee-148">Response</span></span>
<span data-ttu-id="72eee-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="72eee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




