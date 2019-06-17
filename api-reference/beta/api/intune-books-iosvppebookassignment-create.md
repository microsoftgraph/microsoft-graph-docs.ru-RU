---
title: Создание объекта iosVppEBookAssignment
description: Создание объекта iosVppEBookAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9682e5f1d3d539e5a9528404beac4f2b535230f7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972300"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="51d05-103">Создание объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="51d05-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="51d05-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51d05-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51d05-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51d05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51d05-106">Создание объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="51d05-106">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51d05-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="51d05-107">Prerequisites</span></span>
<span data-ttu-id="51d05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51d05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51d05-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51d05-110">Permission type</span></span>|<span data-ttu-id="51d05-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51d05-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51d05-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51d05-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51d05-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51d05-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51d05-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51d05-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51d05-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51d05-115">Not supported.</span></span>|
|<span data-ttu-id="51d05-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51d05-116">Application</span></span>|<span data-ttu-id="51d05-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51d05-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51d05-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51d05-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="51d05-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51d05-119">Request headers</span></span>
|<span data-ttu-id="51d05-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51d05-120">Header</span></span>|<span data-ttu-id="51d05-121">Значение</span><span class="sxs-lookup"><span data-stu-id="51d05-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51d05-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51d05-122">Authorization</span></span>|<span data-ttu-id="51d05-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51d05-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51d05-124">Accept</span><span class="sxs-lookup"><span data-stu-id="51d05-124">Accept</span></span>|<span data-ttu-id="51d05-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51d05-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51d05-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51d05-126">Request body</span></span>
<span data-ttu-id="51d05-127">В тексте запроса добавьте представление объекта iosVppEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51d05-127">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="51d05-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="51d05-128">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="51d05-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="51d05-129">Property</span></span>|<span data-ttu-id="51d05-130">Тип</span><span class="sxs-lookup"><span data-stu-id="51d05-130">Type</span></span>|<span data-ttu-id="51d05-131">Описание</span><span class="sxs-lookup"><span data-stu-id="51d05-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51d05-132">id</span><span class="sxs-lookup"><span data-stu-id="51d05-132">id</span></span>|<span data-ttu-id="51d05-133">String</span><span class="sxs-lookup"><span data-stu-id="51d05-133">String</span></span>|<span data-ttu-id="51d05-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="51d05-134">Key of the entity.</span></span> <span data-ttu-id="51d05-135">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="51d05-135">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="51d05-136">target</span><span class="sxs-lookup"><span data-stu-id="51d05-136">target</span></span>|[<span data-ttu-id="51d05-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="51d05-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="51d05-138">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="51d05-138">The assignment target for eBook.</span></span> <span data-ttu-id="51d05-139">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="51d05-139">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="51d05-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="51d05-140">installIntent</span></span>|[<span data-ttu-id="51d05-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="51d05-141">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="51d05-142">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="51d05-142">The install intent for eBook.</span></span> <span data-ttu-id="51d05-143">Наследуется от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="51d05-143">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="51d05-144">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="51d05-144">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="51d05-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="51d05-145">Response</span></span>
<span data-ttu-id="51d05-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51d05-146">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51d05-147">Пример</span><span class="sxs-lookup"><span data-stu-id="51d05-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="51d05-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="51d05-148">Request</span></span>
<span data-ttu-id="51d05-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51d05-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="51d05-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="51d05-150">Response</span></span>
<span data-ttu-id="51d05-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51d05-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





