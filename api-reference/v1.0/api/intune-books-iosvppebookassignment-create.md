---
title: Создание объекта iosVppEBookAssignment
description: Создание объекта iosVppEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b45e4a986306fbecf039abee29c2a6939f9b4e69
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962213"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="621e8-103">Создание объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="621e8-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="621e8-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="621e8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="621e8-105">Создание объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="621e8-105">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="621e8-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="621e8-106">Prerequisites</span></span>
<span data-ttu-id="621e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="621e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="621e8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="621e8-109">Permission type</span></span>|<span data-ttu-id="621e8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="621e8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="621e8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="621e8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="621e8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="621e8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="621e8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="621e8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="621e8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="621e8-114">Not supported.</span></span>|
|<span data-ttu-id="621e8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="621e8-115">Application</span></span>|<span data-ttu-id="621e8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="621e8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="621e8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="621e8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="621e8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="621e8-118">Request headers</span></span>
|<span data-ttu-id="621e8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="621e8-119">Header</span></span>|<span data-ttu-id="621e8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="621e8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="621e8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="621e8-121">Authorization</span></span>|<span data-ttu-id="621e8-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="621e8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="621e8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="621e8-123">Accept</span></span>|<span data-ttu-id="621e8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="621e8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="621e8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="621e8-125">Request body</span></span>
<span data-ttu-id="621e8-126">В тексте запроса добавьте представление объекта iosVppEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="621e8-126">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="621e8-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="621e8-127">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="621e8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="621e8-128">Property</span></span>|<span data-ttu-id="621e8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="621e8-129">Type</span></span>|<span data-ttu-id="621e8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="621e8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="621e8-131">id</span><span class="sxs-lookup"><span data-stu-id="621e8-131">id</span></span>|<span data-ttu-id="621e8-132">String</span><span class="sxs-lookup"><span data-stu-id="621e8-132">String</span></span>|<span data-ttu-id="621e8-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="621e8-133">Key of the entity.</span></span> <span data-ttu-id="621e8-134">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="621e8-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="621e8-135">target</span><span class="sxs-lookup"><span data-stu-id="621e8-135">target</span></span>|[<span data-ttu-id="621e8-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="621e8-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="621e8-137">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="621e8-137">The assignment target for eBook.</span></span> <span data-ttu-id="621e8-138">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="621e8-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="621e8-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="621e8-139">installIntent</span></span>|[<span data-ttu-id="621e8-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="621e8-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="621e8-141">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="621e8-141">The install intent for eBook.</span></span> <span data-ttu-id="621e8-142">НаСледуется от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="621e8-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="621e8-143">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="621e8-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="621e8-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="621e8-144">Response</span></span>
<span data-ttu-id="621e8-145">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="621e8-145">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="621e8-146">Пример</span><span class="sxs-lookup"><span data-stu-id="621e8-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="621e8-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="621e8-147">Request</span></span>
<span data-ttu-id="621e8-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="621e8-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="621e8-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="621e8-149">Response</span></span>
<span data-ttu-id="621e8-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="621e8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



