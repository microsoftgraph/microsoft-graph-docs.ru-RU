---
title: Обновление объекта iosVppEBookAssignment
description: Обновление свойств объекта iosVppEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e9abf92f2af9ed0a674f7186ee6ebd2433c9e7a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892346"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="1e9b9-103">Обновление объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="1e9b9-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="1e9b9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1e9b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e9b9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e9b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e9b9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1e9b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e9b9-107">Обновление свойств объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1e9b9-107">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e9b9-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1e9b9-108">Prerequisites</span></span>
<span data-ttu-id="1e9b9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e9b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e9b9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e9b9-111">Permission type</span></span>|<span data-ttu-id="1e9b9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e9b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e9b9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e9b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e9b9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e9b9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1e9b9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e9b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e9b9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e9b9-116">Not supported.</span></span>|
|<span data-ttu-id="1e9b9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e9b9-117">Application</span></span>|<span data-ttu-id="1e9b9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e9b9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e9b9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e9b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1e9b9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e9b9-120">Request headers</span></span>
|<span data-ttu-id="1e9b9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1e9b9-121">Header</span></span>|<span data-ttu-id="1e9b9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1e9b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e9b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e9b9-123">Authorization</span></span>|<span data-ttu-id="1e9b9-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1e9b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e9b9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1e9b9-125">Accept</span></span>|<span data-ttu-id="1e9b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e9b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e9b9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e9b9-127">Request body</span></span>
<span data-ttu-id="1e9b9-128">В тексте запроса добавьте представление объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e9b9-128">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="1e9b9-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1e9b9-129">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="1e9b9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e9b9-130">Property</span></span>|<span data-ttu-id="1e9b9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1e9b9-131">Type</span></span>|<span data-ttu-id="1e9b9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1e9b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e9b9-133">id</span><span class="sxs-lookup"><span data-stu-id="1e9b9-133">id</span></span>|<span data-ttu-id="1e9b9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1e9b9-134">String</span></span>|<span data-ttu-id="1e9b9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1e9b9-135">Key of the entity.</span></span> <span data-ttu-id="1e9b9-136">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1e9b9-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="1e9b9-137">target</span><span class="sxs-lookup"><span data-stu-id="1e9b9-137">target</span></span>|[<span data-ttu-id="1e9b9-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1e9b9-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1e9b9-139">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="1e9b9-139">The assignment target for eBook.</span></span> <span data-ttu-id="1e9b9-140">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1e9b9-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="1e9b9-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="1e9b9-141">installIntent</span></span>|[<span data-ttu-id="1e9b9-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="1e9b9-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="1e9b9-143">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="1e9b9-143">The install intent for eBook.</span></span> <span data-ttu-id="1e9b9-144">Наследуется от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1e9b9-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="1e9b9-145">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="1e9b9-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="1e9b9-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e9b9-146">Response</span></span>
<span data-ttu-id="1e9b9-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1e9b9-147">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e9b9-148">Пример</span><span class="sxs-lookup"><span data-stu-id="1e9b9-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e9b9-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e9b9-149">Request</span></span>
<span data-ttu-id="1e9b9-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e9b9-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 133

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="1e9b9-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="1e9b9-151">Response</span></span>
<span data-ttu-id="1e9b9-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1e9b9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





