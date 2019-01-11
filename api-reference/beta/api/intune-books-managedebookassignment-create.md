---
title: Создание объекта managedEBookAssignment
description: Создание объекта managedEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8699cac63bec90693a06d8e73879a53cd3d6a4b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892241"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="e1eb0-103">Создание объекта managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="e1eb0-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="e1eb0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e1eb0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1eb0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1eb0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1eb0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e1eb0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1eb0-107">Создание объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e1eb0-107">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1eb0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e1eb0-108">Prerequisites</span></span>
<span data-ttu-id="e1eb0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1eb0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1eb0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1eb0-111">Permission type</span></span>|<span data-ttu-id="e1eb0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1eb0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1eb0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1eb0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1eb0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1eb0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e1eb0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1eb0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1eb0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1eb0-116">Not supported.</span></span>|
|<span data-ttu-id="e1eb0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1eb0-117">Application</span></span>|<span data-ttu-id="e1eb0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1eb0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1eb0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1eb0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e1eb0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1eb0-120">Request headers</span></span>
|<span data-ttu-id="e1eb0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1eb0-121">Header</span></span>|<span data-ttu-id="e1eb0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e1eb0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1eb0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1eb0-123">Authorization</span></span>|<span data-ttu-id="e1eb0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e1eb0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1eb0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1eb0-125">Accept</span></span>|<span data-ttu-id="e1eb0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1eb0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1eb0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1eb0-127">Request body</span></span>
<span data-ttu-id="e1eb0-128">В тексте запроса добавьте представление объекта managedEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1eb0-128">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="e1eb0-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="e1eb0-129">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="e1eb0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1eb0-130">Property</span></span>|<span data-ttu-id="e1eb0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e1eb0-131">Type</span></span>|<span data-ttu-id="e1eb0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e1eb0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1eb0-133">id</span><span class="sxs-lookup"><span data-stu-id="e1eb0-133">id</span></span>|<span data-ttu-id="e1eb0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e1eb0-134">String</span></span>|<span data-ttu-id="e1eb0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e1eb0-135">Key of the entity.</span></span>|
|<span data-ttu-id="e1eb0-136">target</span><span class="sxs-lookup"><span data-stu-id="e1eb0-136">target</span></span>|[<span data-ttu-id="e1eb0-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e1eb0-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e1eb0-138">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="e1eb0-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="e1eb0-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="e1eb0-139">installIntent</span></span>|[<span data-ttu-id="e1eb0-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="e1eb0-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="e1eb0-141">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="e1eb0-141">The install intent for eBook.</span></span> <span data-ttu-id="e1eb0-142">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="e1eb0-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="e1eb0-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1eb0-143">Response</span></span>
<span data-ttu-id="e1eb0-144">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1eb0-144">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1eb0-145">Пример</span><span class="sxs-lookup"><span data-stu-id="e1eb0-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1eb0-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1eb0-146">Request</span></span>
<span data-ttu-id="e1eb0-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1eb0-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e1eb0-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1eb0-148">Response</span></span>
<span data-ttu-id="e1eb0-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e1eb0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





