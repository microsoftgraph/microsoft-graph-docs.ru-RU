---
title: Создание intuneBrandingProfileAssignment
description: Создание объекта intuneBrandingProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 64aa7d8e1ca3a1ad33e69921a67258f820348704
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157745"
---
# <a name="create-intunebrandingprofileassignment"></a><span data-ttu-id="81fdb-103">Создание intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="81fdb-103">Create intuneBrandingProfileAssignment</span></span>

<span data-ttu-id="81fdb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81fdb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81fdb-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81fdb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81fdb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81fdb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81fdb-107">Создание объекта [intuneBrandingProfileAssignment.](../resources/intune-wip-intunebrandingprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="81fdb-107">Create a new [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81fdb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="81fdb-108">Prerequisites</span></span>
<span data-ttu-id="81fdb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81fdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81fdb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81fdb-111">Permission type</span></span>|<span data-ttu-id="81fdb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="81fdb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81fdb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81fdb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81fdb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81fdb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="81fdb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81fdb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81fdb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81fdb-116">Not supported.</span></span>|
|<span data-ttu-id="81fdb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81fdb-117">Application</span></span>|<span data-ttu-id="81fdb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81fdb-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81fdb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81fdb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="81fdb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="81fdb-120">Request headers</span></span>
|<span data-ttu-id="81fdb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81fdb-121">Header</span></span>|<span data-ttu-id="81fdb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="81fdb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81fdb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81fdb-123">Authorization</span></span>|<span data-ttu-id="81fdb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81fdb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81fdb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="81fdb-125">Accept</span></span>|<span data-ttu-id="81fdb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81fdb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81fdb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81fdb-127">Request body</span></span>
<span data-ttu-id="81fdb-128">В теле запроса укажу представление объекта intuneBrandingProfileAssignment в JSON.</span><span class="sxs-lookup"><span data-stu-id="81fdb-128">In the request body, supply a JSON representation for the intuneBrandingProfileAssignment object.</span></span>

<span data-ttu-id="81fdb-129">В следующей таблице показаны свойства, необходимые при создании intuneBrandingProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="81fdb-129">The following table shows the properties that are required when you create the intuneBrandingProfileAssignment.</span></span>

|<span data-ttu-id="81fdb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="81fdb-130">Property</span></span>|<span data-ttu-id="81fdb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="81fdb-131">Type</span></span>|<span data-ttu-id="81fdb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="81fdb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81fdb-133">id</span><span class="sxs-lookup"><span data-stu-id="81fdb-133">id</span></span>|<span data-ttu-id="81fdb-134">String</span><span class="sxs-lookup"><span data-stu-id="81fdb-134">String</span></span>|<span data-ttu-id="81fdb-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="81fdb-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="81fdb-136">target</span><span class="sxs-lookup"><span data-stu-id="81fdb-136">target</span></span>|[<span data-ttu-id="81fdb-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="81fdb-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="81fdb-138">Целевой объект назначения, который назначен профилю фирменки.</span><span class="sxs-lookup"><span data-stu-id="81fdb-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="81fdb-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="81fdb-139">Response</span></span>
<span data-ttu-id="81fdb-140">В случае успешного выполнения этот метод возвращает код отклика и объект `201 Created` [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="81fdb-140">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81fdb-141">Пример</span><span class="sxs-lookup"><span data-stu-id="81fdb-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="81fdb-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="81fdb-142">Request</span></span>
<span data-ttu-id="81fdb-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81fdb-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
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

### <a name="response"></a><span data-ttu-id="81fdb-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="81fdb-144">Response</span></span>
<span data-ttu-id="81fdb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="81fdb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




