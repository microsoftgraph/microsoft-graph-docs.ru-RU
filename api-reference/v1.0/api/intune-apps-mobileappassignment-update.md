---
title: Обновление объекта mobileAppAssignment
description: Обновление свойств объекта mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c026138c1a4a8c75bf77251729efbf0aaa34d824
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979749"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="745f9-103">Обновление объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="745f9-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="745f9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="745f9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="745f9-105">Обновление свойств объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="745f9-105">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="745f9-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="745f9-106">Prerequisites</span></span>
<span data-ttu-id="745f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="745f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="745f9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="745f9-109">Permission type</span></span>|<span data-ttu-id="745f9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="745f9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="745f9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="745f9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="745f9-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="745f9-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="745f9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="745f9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="745f9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="745f9-114">Not supported.</span></span>|
|<span data-ttu-id="745f9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="745f9-115">Application</span></span>|<span data-ttu-id="745f9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="745f9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="745f9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="745f9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="745f9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="745f9-118">Request headers</span></span>
|<span data-ttu-id="745f9-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="745f9-119">Header</span></span>|<span data-ttu-id="745f9-120">Значение</span><span class="sxs-lookup"><span data-stu-id="745f9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="745f9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="745f9-121">Authorization</span></span>|<span data-ttu-id="745f9-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="745f9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="745f9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="745f9-123">Accept</span></span>|<span data-ttu-id="745f9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="745f9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="745f9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="745f9-125">Request body</span></span>
<span data-ttu-id="745f9-126">В тексте запроса добавьте представление объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="745f9-126">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="745f9-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="745f9-127">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="745f9-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="745f9-128">Property</span></span>|<span data-ttu-id="745f9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="745f9-129">Type</span></span>|<span data-ttu-id="745f9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="745f9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="745f9-131">id</span><span class="sxs-lookup"><span data-stu-id="745f9-131">id</span></span>|<span data-ttu-id="745f9-132">Строка</span><span class="sxs-lookup"><span data-stu-id="745f9-132">String</span></span>|<span data-ttu-id="745f9-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="745f9-133">Key of the entity.</span></span>|
|<span data-ttu-id="745f9-134">intent</span><span class="sxs-lookup"><span data-stu-id="745f9-134">intent</span></span>|[<span data-ttu-id="745f9-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="745f9-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="745f9-136">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="745f9-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="745f9-137">target</span><span class="sxs-lookup"><span data-stu-id="745f9-137">target</span></span>|[<span data-ttu-id="745f9-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="745f9-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="745f9-139">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="745f9-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="745f9-140">settings</span><span class="sxs-lookup"><span data-stu-id="745f9-140">settings</span></span>|[<span data-ttu-id="745f9-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="745f9-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="745f9-142">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="745f9-142">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="745f9-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="745f9-143">Response</span></span>
<span data-ttu-id="745f9-144">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="745f9-144">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="745f9-145">Пример</span><span class="sxs-lookup"><span data-stu-id="745f9-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="745f9-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="745f9-146">Request</span></span>
<span data-ttu-id="745f9-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="745f9-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
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

### <a name="response"></a><span data-ttu-id="745f9-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="745f9-148">Response</span></span>
<span data-ttu-id="745f9-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="745f9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



