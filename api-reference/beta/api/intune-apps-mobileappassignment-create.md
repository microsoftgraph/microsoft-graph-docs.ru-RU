---
title: Создание объекта mobileAppAssignment
description: Создание объекта mobileAppAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8fc2f072e73e00e5673025ecfc760d405be839e6
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37177222"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="4b5c0-103">Создание объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="4b5c0-103">Create mobileAppAssignment</span></span>

> <span data-ttu-id="4b5c0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b5c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b5c0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b5c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b5c0-106">Создание объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4b5c0-106">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b5c0-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4b5c0-107">Prerequisites</span></span>
<span data-ttu-id="4b5c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b5c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b5c0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b5c0-110">Permission type</span></span>|<span data-ttu-id="4b5c0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b5c0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b5c0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b5c0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b5c0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b5c0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4b5c0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b5c0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b5c0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b5c0-115">Not supported.</span></span>|
|<span data-ttu-id="4b5c0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b5c0-116">Application</span></span>|<span data-ttu-id="4b5c0-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b5c0-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b5c0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b5c0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="4b5c0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b5c0-119">Request headers</span></span>
|<span data-ttu-id="4b5c0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b5c0-120">Header</span></span>|<span data-ttu-id="4b5c0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4b5c0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b5c0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b5c0-122">Authorization</span></span>|<span data-ttu-id="4b5c0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b5c0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b5c0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4b5c0-124">Accept</span></span>|<span data-ttu-id="4b5c0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b5c0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b5c0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4b5c0-126">Request body</span></span>
<span data-ttu-id="4b5c0-127">В тексте запроса добавьте представление объекта mobileAppAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b5c0-127">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="4b5c0-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="4b5c0-128">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="4b5c0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b5c0-129">Property</span></span>|<span data-ttu-id="4b5c0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4b5c0-130">Type</span></span>|<span data-ttu-id="4b5c0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4b5c0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b5c0-132">id</span><span class="sxs-lookup"><span data-stu-id="4b5c0-132">id</span></span>|<span data-ttu-id="4b5c0-133">String</span><span class="sxs-lookup"><span data-stu-id="4b5c0-133">String</span></span>|<span data-ttu-id="4b5c0-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4b5c0-134">Key of the entity.</span></span>|
|<span data-ttu-id="4b5c0-135">intent</span><span class="sxs-lookup"><span data-stu-id="4b5c0-135">intent</span></span>|[<span data-ttu-id="4b5c0-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="4b5c0-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="4b5c0-137">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="4b5c0-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="4b5c0-138">target</span><span class="sxs-lookup"><span data-stu-id="4b5c0-138">target</span></span>|[<span data-ttu-id="4b5c0-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4b5c0-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4b5c0-140">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="4b5c0-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="4b5c0-141">settings</span><span class="sxs-lookup"><span data-stu-id="4b5c0-141">settings</span></span>|[<span data-ttu-id="4b5c0-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="4b5c0-142">mobileAppAssignmentSettings</span></span>](../resources/intune-shared-mobileappassignmentsettings.md)|<span data-ttu-id="4b5c0-143">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="4b5c0-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="4b5c0-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b5c0-144">Response</span></span>
<span data-ttu-id="4b5c0-145">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b5c0-145">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b5c0-146">Пример</span><span class="sxs-lookup"><span data-stu-id="4b5c0-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b5c0-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b5c0-147">Request</span></span>
<span data-ttu-id="4b5c0-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b5c0-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4b5c0-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b5c0-149">Response</span></span>
<span data-ttu-id="4b5c0-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b5c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




