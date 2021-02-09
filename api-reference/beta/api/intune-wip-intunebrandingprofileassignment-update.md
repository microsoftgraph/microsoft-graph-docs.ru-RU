---
title: Обновление intuneBrandingProfileAssignment
description: Обновление свойств объекта intuneBrandingProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eeafacd7fa37b17f3cb74669f1c41cdf54768fdf
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157717"
---
# <a name="update-intunebrandingprofileassignment"></a><span data-ttu-id="405c6-103">Обновление intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="405c6-103">Update intuneBrandingProfileAssignment</span></span>

<span data-ttu-id="405c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="405c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="405c6-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="405c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="405c6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="405c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="405c6-107">Обновление свойств объекта [intuneBrandingProfileAssignment.](../resources/intune-wip-intunebrandingprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="405c6-107">Update the properties of a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="405c6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="405c6-108">Prerequisites</span></span>
<span data-ttu-id="405c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="405c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="405c6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="405c6-111">Permission type</span></span>|<span data-ttu-id="405c6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="405c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="405c6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="405c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="405c6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="405c6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="405c6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="405c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="405c6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="405c6-116">Not supported.</span></span>|
|<span data-ttu-id="405c6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="405c6-117">Application</span></span>|<span data-ttu-id="405c6-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="405c6-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="405c6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="405c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="405c6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="405c6-120">Request headers</span></span>
|<span data-ttu-id="405c6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="405c6-121">Header</span></span>|<span data-ttu-id="405c6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="405c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="405c6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="405c6-123">Authorization</span></span>|<span data-ttu-id="405c6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="405c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="405c6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="405c6-125">Accept</span></span>|<span data-ttu-id="405c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="405c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="405c6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="405c6-127">Request body</span></span>
<span data-ttu-id="405c6-128">В теле запроса укажу представление объекта [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="405c6-128">In the request body, supply a JSON representation for the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

<span data-ttu-id="405c6-129">В следующей таблице показаны свойства, необходимые при создании [объекта intuneBrandingProfileAssignment.](../resources/intune-wip-intunebrandingprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="405c6-129">The following table shows the properties that are required when you create the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md).</span></span>

|<span data-ttu-id="405c6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="405c6-130">Property</span></span>|<span data-ttu-id="405c6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="405c6-131">Type</span></span>|<span data-ttu-id="405c6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="405c6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="405c6-133">id</span><span class="sxs-lookup"><span data-stu-id="405c6-133">id</span></span>|<span data-ttu-id="405c6-134">String</span><span class="sxs-lookup"><span data-stu-id="405c6-134">String</span></span>|<span data-ttu-id="405c6-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="405c6-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="405c6-136">target</span><span class="sxs-lookup"><span data-stu-id="405c6-136">target</span></span>|[<span data-ttu-id="405c6-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="405c6-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="405c6-138">Целевой объект назначения, который назначен профилю фирменки.</span><span class="sxs-lookup"><span data-stu-id="405c6-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="405c6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="405c6-139">Response</span></span>
<span data-ttu-id="405c6-140">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="405c6-140">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="405c6-141">Пример</span><span class="sxs-lookup"><span data-stu-id="405c6-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="405c6-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="405c6-142">Request</span></span>
<span data-ttu-id="405c6-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="405c6-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
Content-type: application/json
Content-length: 390

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="405c6-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="405c6-144">Response</span></span>
<span data-ttu-id="405c6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="405c6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
  "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```




