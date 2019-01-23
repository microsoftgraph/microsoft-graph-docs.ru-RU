---
title: Создание объекта mobileAppAssignment
description: Создание объекта mobileAppAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 94fb6e79077e687df11cda4b28b71b8e97360971
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397983"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="ff930-103">Создание объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="ff930-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="ff930-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ff930-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ff930-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff930-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff930-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff930-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff930-107">Создание объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ff930-107">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff930-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ff930-108">Prerequisites</span></span>
<span data-ttu-id="ff930-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ff930-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ff930-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff930-111">Permission type</span></span>|<span data-ttu-id="ff930-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff930-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff930-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff930-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff930-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff930-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ff930-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff930-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff930-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff930-116">Not supported.</span></span>|
|<span data-ttu-id="ff930-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff930-117">Application</span></span>|<span data-ttu-id="ff930-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff930-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff930-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff930-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ff930-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff930-120">Request headers</span></span>
|<span data-ttu-id="ff930-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff930-121">Header</span></span>|<span data-ttu-id="ff930-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ff930-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff930-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff930-123">Authorization</span></span>|<span data-ttu-id="ff930-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ff930-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff930-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ff930-125">Accept</span></span>|<span data-ttu-id="ff930-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff930-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff930-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff930-127">Request body</span></span>
<span data-ttu-id="ff930-128">В тексте запроса добавьте представление объекта mobileAppAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff930-128">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="ff930-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="ff930-129">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="ff930-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff930-130">Property</span></span>|<span data-ttu-id="ff930-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ff930-131">Type</span></span>|<span data-ttu-id="ff930-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ff930-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff930-133">id</span><span class="sxs-lookup"><span data-stu-id="ff930-133">id</span></span>|<span data-ttu-id="ff930-134">String</span><span class="sxs-lookup"><span data-stu-id="ff930-134">String</span></span>|<span data-ttu-id="ff930-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ff930-135">Key of the entity.</span></span>|
|<span data-ttu-id="ff930-136">intent</span><span class="sxs-lookup"><span data-stu-id="ff930-136">intent</span></span>|[<span data-ttu-id="ff930-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="ff930-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="ff930-138">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="ff930-138">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="ff930-139">target</span><span class="sxs-lookup"><span data-stu-id="ff930-139">target</span></span>|[<span data-ttu-id="ff930-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ff930-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ff930-141">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="ff930-141">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="ff930-142">settings</span><span class="sxs-lookup"><span data-stu-id="ff930-142">settings</span></span>|[<span data-ttu-id="ff930-143">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ff930-143">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="ff930-144">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="ff930-144">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="ff930-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff930-145">Response</span></span>
<span data-ttu-id="ff930-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ff930-146">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff930-147">Пример</span><span class="sxs-lookup"><span data-stu-id="ff930-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff930-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff930-148">Request</span></span>
<span data-ttu-id="ff930-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff930-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ff930-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff930-150">Response</span></span>
<span data-ttu-id="ff930-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ff930-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




