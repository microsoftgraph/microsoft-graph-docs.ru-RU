---
title: Создание объекта managedEBookAssignment
description: Создание объекта managedEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d3f8ad25a36c6e60152844bf21c346850ad04f34
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264171"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="2474c-103">Создание объекта managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="2474c-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="2474c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2474c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2474c-105">Создание объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2474c-105">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2474c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2474c-106">Prerequisites</span></span>
<span data-ttu-id="2474c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2474c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2474c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2474c-109">Permission type</span></span>|<span data-ttu-id="2474c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2474c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2474c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2474c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2474c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2474c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2474c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2474c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2474c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2474c-114">Not supported.</span></span>|
|<span data-ttu-id="2474c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2474c-115">Application</span></span>|<span data-ttu-id="2474c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2474c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2474c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2474c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2474c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2474c-118">Request headers</span></span>
|<span data-ttu-id="2474c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2474c-119">Header</span></span>|<span data-ttu-id="2474c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2474c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2474c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2474c-121">Authorization</span></span>|<span data-ttu-id="2474c-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2474c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2474c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2474c-123">Accept</span></span>|<span data-ttu-id="2474c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2474c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2474c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2474c-125">Request body</span></span>
<span data-ttu-id="2474c-126">В тексте запроса добавьте представление объекта managedEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2474c-126">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="2474c-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="2474c-127">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="2474c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2474c-128">Property</span></span>|<span data-ttu-id="2474c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2474c-129">Type</span></span>|<span data-ttu-id="2474c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2474c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2474c-131">id</span><span class="sxs-lookup"><span data-stu-id="2474c-131">id</span></span>|<span data-ttu-id="2474c-132">String</span><span class="sxs-lookup"><span data-stu-id="2474c-132">String</span></span>|<span data-ttu-id="2474c-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2474c-133">Key of the entity.</span></span>|
|<span data-ttu-id="2474c-134">target</span><span class="sxs-lookup"><span data-stu-id="2474c-134">target</span></span>|[<span data-ttu-id="2474c-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2474c-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2474c-136">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="2474c-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="2474c-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="2474c-137">installIntent</span></span>|[<span data-ttu-id="2474c-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="2474c-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="2474c-139">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="2474c-139">The install intent for eBook.</span></span> <span data-ttu-id="2474c-140">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="2474c-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="2474c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2474c-141">Response</span></span>
<span data-ttu-id="2474c-142">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2474c-142">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2474c-143">Пример</span><span class="sxs-lookup"><span data-stu-id="2474c-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="2474c-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2474c-144">Request</span></span>
<span data-ttu-id="2474c-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2474c-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="2474c-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="2474c-146">Response</span></span>
<span data-ttu-id="2474c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2474c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



