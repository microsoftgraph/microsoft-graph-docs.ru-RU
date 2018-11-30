---
title: Создание объекта managedEBookAssignment
description: Создание объекта managedEBookAssignment.
ms.openlocfilehash: 74e65f386d4699010924e9ac616b479f14464f66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074970"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="cb3b2-103">Создание объекта managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="cb3b2-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="cb3b2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cb3b2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb3b2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb3b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb3b2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cb3b2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb3b2-107">Создание объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cb3b2-107">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cb3b2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cb3b2-108">Prerequisites</span></span>
<span data-ttu-id="cb3b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb3b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb3b2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb3b2-111">Permission type</span></span>|<span data-ttu-id="cb3b2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb3b2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb3b2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb3b2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb3b2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb3b2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cb3b2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb3b2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb3b2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb3b2-116">Not supported.</span></span>|
|<span data-ttu-id="cb3b2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb3b2-117">Application</span></span>|<span data-ttu-id="cb3b2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb3b2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb3b2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb3b2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="cb3b2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb3b2-120">Request headers</span></span>
|<span data-ttu-id="cb3b2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb3b2-121">Header</span></span>|<span data-ttu-id="cb3b2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cb3b2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb3b2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb3b2-123">Authorization</span></span>|<span data-ttu-id="cb3b2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cb3b2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb3b2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cb3b2-125">Accept</span></span>|<span data-ttu-id="cb3b2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb3b2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb3b2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb3b2-127">Request body</span></span>
<span data-ttu-id="cb3b2-128">В тексте запроса добавьте представление объекта managedEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb3b2-128">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="cb3b2-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="cb3b2-129">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="cb3b2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb3b2-130">Property</span></span>|<span data-ttu-id="cb3b2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cb3b2-131">Type</span></span>|<span data-ttu-id="cb3b2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cb3b2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb3b2-133">id</span><span class="sxs-lookup"><span data-stu-id="cb3b2-133">id</span></span>|<span data-ttu-id="cb3b2-134">String</span><span class="sxs-lookup"><span data-stu-id="cb3b2-134">String</span></span>|<span data-ttu-id="cb3b2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cb3b2-135">Key of the entity.</span></span>|
|<span data-ttu-id="cb3b2-136">target</span><span class="sxs-lookup"><span data-stu-id="cb3b2-136">target</span></span>|[<span data-ttu-id="cb3b2-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cb3b2-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cb3b2-138">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="cb3b2-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="cb3b2-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="cb3b2-139">installIntent</span></span>|[<span data-ttu-id="cb3b2-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="cb3b2-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="cb3b2-141">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="cb3b2-141">The install intent for eBook.</span></span> <span data-ttu-id="cb3b2-142">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="cb3b2-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="cb3b2-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb3b2-143">Response</span></span>
<span data-ttu-id="cb3b2-144">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cb3b2-144">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb3b2-145">Пример</span><span class="sxs-lookup"><span data-stu-id="cb3b2-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="cb3b2-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb3b2-146">Request</span></span>
<span data-ttu-id="cb3b2-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb3b2-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cb3b2-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb3b2-148">Response</span></span>
<span data-ttu-id="cb3b2-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cb3b2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





