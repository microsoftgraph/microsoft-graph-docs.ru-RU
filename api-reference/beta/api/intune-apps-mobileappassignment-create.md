---
title: Создание объекта mobileAppAssignment
description: Создание объекта mobileAppAssignment.
author: tfitzmac
ms.openlocfilehash: d662002d02c688698f77e4fd2908b27b8863a5cf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359061"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="c8e77-103">Создание объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="c8e77-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="c8e77-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c8e77-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8e77-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e77-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8e77-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c8e77-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8e77-107">Создание объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c8e77-107">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8e77-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c8e77-108">Prerequisites</span></span>
<span data-ttu-id="c8e77-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8e77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8e77-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8e77-111">Permission type</span></span>|<span data-ttu-id="c8e77-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8e77-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8e77-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8e77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8e77-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8e77-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c8e77-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8e77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8e77-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e77-116">Not supported.</span></span>|
|<span data-ttu-id="c8e77-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8e77-117">Application</span></span>|<span data-ttu-id="c8e77-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e77-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8e77-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8e77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c8e77-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8e77-120">Request headers</span></span>
|<span data-ttu-id="c8e77-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8e77-121">Header</span></span>|<span data-ttu-id="c8e77-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c8e77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8e77-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8e77-123">Authorization</span></span>|<span data-ttu-id="c8e77-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c8e77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8e77-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8e77-125">Accept</span></span>|<span data-ttu-id="c8e77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8e77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8e77-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8e77-127">Request body</span></span>
<span data-ttu-id="c8e77-128">В тексте запроса добавьте представление объекта mobileAppAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8e77-128">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="c8e77-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="c8e77-129">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="c8e77-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8e77-130">Property</span></span>|<span data-ttu-id="c8e77-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c8e77-131">Type</span></span>|<span data-ttu-id="c8e77-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c8e77-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8e77-133">id</span><span class="sxs-lookup"><span data-stu-id="c8e77-133">id</span></span>|<span data-ttu-id="c8e77-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c8e77-134">String</span></span>|<span data-ttu-id="c8e77-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c8e77-135">Key of the entity.</span></span>|
|<span data-ttu-id="c8e77-136">intent</span><span class="sxs-lookup"><span data-stu-id="c8e77-136">intent</span></span>|[<span data-ttu-id="c8e77-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="c8e77-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="c8e77-138">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="c8e77-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="c8e77-139">target</span><span class="sxs-lookup"><span data-stu-id="c8e77-139">target</span></span>|[<span data-ttu-id="c8e77-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c8e77-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c8e77-141">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="c8e77-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="c8e77-142">settings</span><span class="sxs-lookup"><span data-stu-id="c8e77-142">settings</span></span>|[<span data-ttu-id="c8e77-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="c8e77-143">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="c8e77-144">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="c8e77-144">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="c8e77-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8e77-145">Response</span></span>
<span data-ttu-id="c8e77-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8e77-146">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8e77-147">Пример</span><span class="sxs-lookup"><span data-stu-id="c8e77-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8e77-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8e77-148">Request</span></span>
<span data-ttu-id="c8e77-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8e77-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```

### <a name="response"></a><span data-ttu-id="c8e77-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8e77-150">Response</span></span>
<span data-ttu-id="c8e77-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c8e77-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 322

{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "591620b7-20b7-5916-b720-1659b7201659",
  "intent": "required",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```





