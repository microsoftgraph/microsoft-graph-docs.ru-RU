---
title: Создание объекта mobileAppAssignment
description: Создание объекта mobileAppAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0e4a8561e2bcd2e194c4a092262f173c77d9d008
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516061"
---
# <a name="create-mobileappassignment"></a><span data-ttu-id="68543-103">Создание объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="68543-103">Create mobileAppAssignment</span></span>

<span data-ttu-id="68543-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68543-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68543-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68543-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68543-106">Создание объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="68543-106">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68543-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="68543-107">Prerequisites</span></span>
<span data-ttu-id="68543-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68543-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68543-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68543-110">Permission type</span></span>|<span data-ttu-id="68543-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68543-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68543-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68543-112">Delegated (work or school account)</span></span>|<span data-ttu-id="68543-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68543-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="68543-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68543-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68543-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68543-115">Not supported.</span></span>|
|<span data-ttu-id="68543-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68543-116">Application</span></span>|<span data-ttu-id="68543-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68543-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68543-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68543-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="68543-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="68543-119">Request headers</span></span>
|<span data-ttu-id="68543-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68543-120">Header</span></span>|<span data-ttu-id="68543-121">Значение</span><span class="sxs-lookup"><span data-stu-id="68543-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68543-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="68543-122">Authorization</span></span>|<span data-ttu-id="68543-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68543-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68543-124">Accept</span><span class="sxs-lookup"><span data-stu-id="68543-124">Accept</span></span>|<span data-ttu-id="68543-125">application/json</span><span class="sxs-lookup"><span data-stu-id="68543-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68543-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68543-126">Request body</span></span>
<span data-ttu-id="68543-127">В тексте запроса добавьте представление объекта mobileAppAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68543-127">In the request body, supply a JSON representation for the mobileAppAssignment object.</span></span>

<span data-ttu-id="68543-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppAssignment.</span><span class="sxs-lookup"><span data-stu-id="68543-128">The following table shows the properties that are required when you create the mobileAppAssignment.</span></span>

|<span data-ttu-id="68543-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="68543-129">Property</span></span>|<span data-ttu-id="68543-130">Тип</span><span class="sxs-lookup"><span data-stu-id="68543-130">Type</span></span>|<span data-ttu-id="68543-131">Описание</span><span class="sxs-lookup"><span data-stu-id="68543-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68543-132">id</span><span class="sxs-lookup"><span data-stu-id="68543-132">id</span></span>|<span data-ttu-id="68543-133">Строка</span><span class="sxs-lookup"><span data-stu-id="68543-133">String</span></span>|<span data-ttu-id="68543-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="68543-134">Key of the entity.</span></span>|
|<span data-ttu-id="68543-135">intent</span><span class="sxs-lookup"><span data-stu-id="68543-135">intent</span></span>|[<span data-ttu-id="68543-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="68543-136">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="68543-137">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="68543-137">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="68543-138">target</span><span class="sxs-lookup"><span data-stu-id="68543-138">target</span></span>|[<span data-ttu-id="68543-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="68543-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="68543-140">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="68543-140">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="68543-141">settings</span><span class="sxs-lookup"><span data-stu-id="68543-141">settings</span></span>|[<span data-ttu-id="68543-142">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="68543-142">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="68543-143">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="68543-143">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="68543-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="68543-144">Response</span></span>
<span data-ttu-id="68543-145">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68543-145">If successful, this method returns a `201 Created` response code and a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68543-146">Пример</span><span class="sxs-lookup"><span data-stu-id="68543-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="68543-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="68543-147">Request</span></span>
<span data-ttu-id="68543-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68543-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
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

### <a name="response"></a><span data-ttu-id="68543-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="68543-149">Response</span></span>
<span data-ttu-id="68543-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68543-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




