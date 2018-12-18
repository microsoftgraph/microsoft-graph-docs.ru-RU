---
title: Создание объекта iosVppEBookAssignment
description: Создание объекта iosVppEBookAssignment.
author: tfitzmac
ms.openlocfilehash: dd829dfd22b38a6ca4b88e1fc110db4f9e2128ea
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302466"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="5c4fb-103">Создание объекта iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="5c4fb-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="5c4fb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5c4fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c4fb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c4fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c4fb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5c4fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c4fb-107">Создание объекта [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5c4fb-107">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c4fb-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5c4fb-108">Prerequisites</span></span>
<span data-ttu-id="5c4fb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c4fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c4fb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c4fb-111">Permission type</span></span>|<span data-ttu-id="5c4fb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c4fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c4fb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c4fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c4fb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c4fb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5c4fb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c4fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c4fb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c4fb-116">Not supported.</span></span>|
|<span data-ttu-id="5c4fb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c4fb-117">Application</span></span>|<span data-ttu-id="5c4fb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c4fb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c4fb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c4fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="5c4fb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c4fb-120">Request headers</span></span>
|<span data-ttu-id="5c4fb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c4fb-121">Header</span></span>|<span data-ttu-id="5c4fb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5c4fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c4fb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c4fb-123">Authorization</span></span>|<span data-ttu-id="5c4fb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5c4fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c4fb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5c4fb-125">Accept</span></span>|<span data-ttu-id="5c4fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c4fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c4fb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c4fb-127">Request body</span></span>
<span data-ttu-id="5c4fb-128">В тексте запроса добавьте представление объекта iosVppEBookAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c4fb-128">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="5c4fb-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта iosVppEBookAssignment.</span><span class="sxs-lookup"><span data-stu-id="5c4fb-129">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="5c4fb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c4fb-130">Property</span></span>|<span data-ttu-id="5c4fb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5c4fb-131">Type</span></span>|<span data-ttu-id="5c4fb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5c4fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c4fb-133">id</span><span class="sxs-lookup"><span data-stu-id="5c4fb-133">id</span></span>|<span data-ttu-id="5c4fb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5c4fb-134">String</span></span>|<span data-ttu-id="5c4fb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5c4fb-135">Key of the entity.</span></span> <span data-ttu-id="5c4fb-136">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5c4fb-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="5c4fb-137">target</span><span class="sxs-lookup"><span data-stu-id="5c4fb-137">target</span></span>|[<span data-ttu-id="5c4fb-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5c4fb-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5c4fb-139">Цель назначения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5c4fb-139">The assignment target for eBook.</span></span> <span data-ttu-id="5c4fb-140">Наследуется от объекта [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5c4fb-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="5c4fb-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="5c4fb-141">installIntent</span></span>|[<span data-ttu-id="5c4fb-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="5c4fb-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="5c4fb-143">Цель установки электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5c4fb-143">The install intent for eBook.</span></span> <span data-ttu-id="5c4fb-144">Наследуется от [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5c4fb-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="5c4fb-145">Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="5c4fb-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="5c4fb-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c4fb-146">Response</span></span>
<span data-ttu-id="5c4fb-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5c4fb-147">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c4fb-148">Пример</span><span class="sxs-lookup"><span data-stu-id="5c4fb-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c4fb-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c4fb-149">Request</span></span>
<span data-ttu-id="5c4fb-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c4fb-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5c4fb-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c4fb-151">Response</span></span>
<span data-ttu-id="5c4fb-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5c4fb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





