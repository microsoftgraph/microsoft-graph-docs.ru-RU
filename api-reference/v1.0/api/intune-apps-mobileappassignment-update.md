---
title: Обновление объекта mobileAppAssignment
description: Обновление свойств объекта mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 647a5a4bb7a89b0b44ce650c411b95c5c20c162c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541768"
---
# <a name="update-mobileappassignment"></a><span data-ttu-id="a7ae4-103">Обновление объекта mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="a7ae4-103">Update mobileAppAssignment</span></span>

> <span data-ttu-id="a7ae4-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7ae4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7ae4-105">Обновление свойств объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a7ae4-105">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7ae4-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a7ae4-106">Prerequisites</span></span>
<span data-ttu-id="a7ae4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7ae4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7ae4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7ae4-109">Permission type</span></span>|<span data-ttu-id="a7ae4-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7ae4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7ae4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7ae4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a7ae4-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7ae4-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a7ae4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7ae4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7ae4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7ae4-114">Not supported.</span></span>|
|<span data-ttu-id="a7ae4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7ae4-115">Application</span></span>|<span data-ttu-id="a7ae4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7ae4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7ae4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7ae4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="a7ae4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7ae4-118">Request headers</span></span>
|<span data-ttu-id="a7ae4-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7ae4-119">Header</span></span>|<span data-ttu-id="a7ae4-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a7ae4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7ae4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7ae4-121">Authorization</span></span>|<span data-ttu-id="a7ae4-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7ae4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7ae4-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a7ae4-123">Accept</span></span>|<span data-ttu-id="a7ae4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a7ae4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7ae4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7ae4-125">Request body</span></span>
<span data-ttu-id="a7ae4-126">В тексте запроса добавьте представление объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7ae4-126">In the request body, supply a JSON representation for the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

<span data-ttu-id="a7ae4-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a7ae4-127">The following table shows the properties that are required when you create the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>

|<span data-ttu-id="a7ae4-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7ae4-128">Property</span></span>|<span data-ttu-id="a7ae4-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a7ae4-129">Type</span></span>|<span data-ttu-id="a7ae4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a7ae4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7ae4-131">id</span><span class="sxs-lookup"><span data-stu-id="a7ae4-131">id</span></span>|<span data-ttu-id="a7ae4-132">String</span><span class="sxs-lookup"><span data-stu-id="a7ae4-132">String</span></span>|<span data-ttu-id="a7ae4-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a7ae4-133">Key of the entity.</span></span>|
|<span data-ttu-id="a7ae4-134">intent</span><span class="sxs-lookup"><span data-stu-id="a7ae4-134">intent</span></span>|[<span data-ttu-id="a7ae4-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="a7ae4-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="a7ae4-136">Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span><span class="sxs-lookup"><span data-stu-id="a7ae4-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="a7ae4-137">target</span><span class="sxs-lookup"><span data-stu-id="a7ae4-137">target</span></span>|[<span data-ttu-id="a7ae4-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a7ae4-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a7ae4-139">Целевое назначение группы, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="a7ae4-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="a7ae4-140">settings</span><span class="sxs-lookup"><span data-stu-id="a7ae4-140">settings</span></span>|[<span data-ttu-id="a7ae4-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a7ae4-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="a7ae4-142">Параметры целевого назначения, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="a7ae4-142">The settings for target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="a7ae4-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7ae4-143">Response</span></span>
<span data-ttu-id="a7ae4-144">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a7ae4-144">If successful, this method returns a `200 OK` response code and an updated [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7ae4-145">Пример</span><span class="sxs-lookup"><span data-stu-id="a7ae4-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7ae4-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7ae4-146">Request</span></span>
<span data-ttu-id="a7ae4-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7ae4-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a7ae4-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7ae4-148">Response</span></span>
<span data-ttu-id="a7ae4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7ae4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



