---
title: Обновление Интунебрандингпрофилеассигнмент
description: Обновление свойств объекта Интунебрандингпрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 718a2e538b619a4138ef64987009bd5f6415851a
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791211"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="be00c-103">Обновление Интунебрандингпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="be00c-103">Update intuneBrandingProfileAssignment</span></span>

<span data-ttu-id="be00c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be00c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be00c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be00c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be00c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be00c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be00c-107">Обновление свойств объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="be00c-107">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be00c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="be00c-108">Prerequisites</span></span>
<span data-ttu-id="be00c-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="be00c-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="be00c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be00c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be00c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be00c-111">Permission type</span></span>|<span data-ttu-id="be00c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be00c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be00c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be00c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="be00c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be00c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="be00c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be00c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be00c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be00c-116">Not supported.</span></span>|
|<span data-ttu-id="be00c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be00c-117">Application</span></span>|<span data-ttu-id="be00c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be00c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be00c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be00c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="be00c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="be00c-120">Request headers</span></span>
|<span data-ttu-id="be00c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be00c-121">Header</span></span>|<span data-ttu-id="be00c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="be00c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be00c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be00c-123">Authorization</span></span>|<span data-ttu-id="be00c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be00c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be00c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="be00c-125">Accept</span></span>|<span data-ttu-id="be00c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be00c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be00c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be00c-127">Request body</span></span>
<span data-ttu-id="be00c-128">В тексте запроса добавьте представление объекта [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be00c-128">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="be00c-129">В следующей таблице приведены свойства, необходимые при создании [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="be00c-129">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="be00c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="be00c-130">Property</span></span>|<span data-ttu-id="be00c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="be00c-131">Type</span></span>|<span data-ttu-id="be00c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="be00c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be00c-133">id</span><span class="sxs-lookup"><span data-stu-id="be00c-133">id</span></span>|<span data-ttu-id="be00c-134">String</span><span class="sxs-lookup"><span data-stu-id="be00c-134">String</span></span>|<span data-ttu-id="be00c-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="be00c-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="be00c-136">target</span><span class="sxs-lookup"><span data-stu-id="be00c-136">target</span></span>|[<span data-ttu-id="be00c-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="be00c-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="be00c-138">Цель назначения, которой назначен профиль фирменной символики.</span><span class="sxs-lookup"><span data-stu-id="be00c-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="be00c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="be00c-139">Response</span></span>
<span data-ttu-id="be00c-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [интунебрандингпрофилеассигнмент](../resources/intune-wip-intunebrandingprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be00c-140">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be00c-141">Пример</span><span class="sxs-lookup"><span data-stu-id="be00c-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="be00c-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="be00c-142">Request</span></span>
<span data-ttu-id="be00c-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be00c-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
Content-type: application/json
Content-length: 326

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="be00c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="be00c-144">Response</span></span>
<span data-ttu-id="be00c-145">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="be00c-145">Here is an example of the response.</span></span> <span data-ttu-id="be00c-146">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="be00c-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="be00c-147">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="be00c-147">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 375

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



