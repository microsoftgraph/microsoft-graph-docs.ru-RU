---
title: Обновление объекта mobileAppAssignment
description: Обновление свойств объекта mobileAppAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e3def82afd878729122dec3112a3e91bb6d76dfa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961019"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="b7f00-103">Обновление объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="b7f00-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="b7f00-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7f00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7f00-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7f00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7f00-106">Обновление свойств объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b7f00-106">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7f00-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b7f00-107">Prerequisites</span></span>
<span data-ttu-id="b7f00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7f00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7f00-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7f00-110">Permission type</span></span>|<span data-ttu-id="b7f00-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7f00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7f00-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7f00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7f00-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7f00-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b7f00-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7f00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7f00-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7f00-115">Not supported.</span></span>|
|<span data-ttu-id="b7f00-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7f00-116">Application</span></span>|<span data-ttu-id="b7f00-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7f00-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7f00-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7f00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b7f00-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7f00-119">Request headers</span></span>
|<span data-ttu-id="b7f00-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7f00-120">Header</span></span>|<span data-ttu-id="b7f00-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b7f00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7f00-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7f00-122">Authorization</span></span>|<span data-ttu-id="b7f00-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7f00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7f00-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b7f00-124">Accept</span></span>|<span data-ttu-id="b7f00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7f00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7f00-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b7f00-126">Request body</span></span>
<span data-ttu-id="b7f00-127">В тексте запроса добавьте представление объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7f00-127">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="b7f00-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b7f00-128">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="b7f00-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7f00-129">Property</span></span>|<span data-ttu-id="b7f00-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b7f00-130">Type</span></span>|<span data-ttu-id="b7f00-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b7f00-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7f00-132">id</span><span class="sxs-lookup"><span data-stu-id="b7f00-132">id</span></span>|<span data-ttu-id="b7f00-133">String</span><span class="sxs-lookup"><span data-stu-id="b7f00-133">String</span></span>|<span data-ttu-id="b7f00-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b7f00-134">Key of the entity.</span></span>|
|<span data-ttu-id="b7f00-135">intent</span><span class="sxs-lookup"><span data-stu-id="b7f00-135">intent</span></span>|[<span data-ttu-id="b7f00-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="b7f00-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="b7f00-137">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="b7f00-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="b7f00-138">target</span><span class="sxs-lookup"><span data-stu-id="b7f00-138">target</span></span>|[<span data-ttu-id="b7f00-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b7f00-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b7f00-140">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="b7f00-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="b7f00-141">settings</span><span class="sxs-lookup"><span data-stu-id="b7f00-141">settings</span></span>|[<span data-ttu-id="b7f00-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="b7f00-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="b7f00-143">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="b7f00-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="b7f00-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7f00-144">Response</span></span>
<span data-ttu-id="b7f00-145">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b7f00-145">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7f00-146">Пример</span><span class="sxs-lookup"><span data-stu-id="b7f00-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7f00-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7f00-147">Request</span></span>
<span data-ttu-id="b7f00-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7f00-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
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

### <a name="response"></a><span data-ttu-id="b7f00-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7f00-149">Response</span></span>
<span data-ttu-id="b7f00-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7f00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





