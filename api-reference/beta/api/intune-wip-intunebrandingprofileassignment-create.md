---
title: Создание intuneBrandingProfileAssignment
description: Создайте новый объект intuneBrandingProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fd4d3d7ef926e239e77333e0aed51e3a46fa49c8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133810"
---
# <a name="create-intunebrandingprofileassignment"></a><span data-ttu-id="1fd8a-103">Создание intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="1fd8a-103">Create intuneBrandingProfileAssignment</span></span>

<span data-ttu-id="1fd8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fd8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1fd8a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fd8a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fd8a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1fd8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fd8a-107">Создайте новый [объект intuneBrandingProfileAssignment.](../resources/intune-wip-intunebrandingprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1fd8a-107">Create a new [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fd8a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1fd8a-108">Prerequisites</span></span>
<span data-ttu-id="1fd8a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fd8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fd8a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fd8a-111">Permission type</span></span>|<span data-ttu-id="1fd8a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fd8a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fd8a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fd8a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1fd8a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fd8a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1fd8a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fd8a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fd8a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fd8a-116">Not supported.</span></span>|
|<span data-ttu-id="1fd8a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1fd8a-117">Application</span></span>|<span data-ttu-id="1fd8a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fd8a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fd8a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fd8a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1fd8a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1fd8a-120">Request headers</span></span>
|<span data-ttu-id="1fd8a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1fd8a-121">Header</span></span>|<span data-ttu-id="1fd8a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1fd8a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fd8a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fd8a-123">Authorization</span></span>|<span data-ttu-id="1fd8a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fd8a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fd8a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1fd8a-125">Accept</span></span>|<span data-ttu-id="1fd8a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1fd8a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fd8a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1fd8a-127">Request body</span></span>
<span data-ttu-id="1fd8a-128">В теле запроса поставляем представление JSON для объекта intuneBrandingProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="1fd8a-128">In the request body, supply a JSON representation for the intuneBrandingProfileAssignment object.</span></span>

<span data-ttu-id="1fd8a-129">В следующей таблице показаны свойства, необходимые при создании intuneBrandingProfileAssignment.</span><span class="sxs-lookup"><span data-stu-id="1fd8a-129">The following table shows the properties that are required when you create the intuneBrandingProfileAssignment.</span></span>

|<span data-ttu-id="1fd8a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fd8a-130">Property</span></span>|<span data-ttu-id="1fd8a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1fd8a-131">Type</span></span>|<span data-ttu-id="1fd8a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1fd8a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fd8a-133">id</span><span class="sxs-lookup"><span data-stu-id="1fd8a-133">id</span></span>|<span data-ttu-id="1fd8a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1fd8a-134">String</span></span>|<span data-ttu-id="1fd8a-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="1fd8a-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="1fd8a-136">target</span><span class="sxs-lookup"><span data-stu-id="1fd8a-136">target</span></span>|[<span data-ttu-id="1fd8a-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1fd8a-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1fd8a-138">Назначение цели, назначенной профилем брендинга.</span><span class="sxs-lookup"><span data-stu-id="1fd8a-138">Assignment target that the branding profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="1fd8a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fd8a-139">Response</span></span>
<span data-ttu-id="1fd8a-140">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1fd8a-140">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fd8a-141">Пример</span><span class="sxs-lookup"><span data-stu-id="1fd8a-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fd8a-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fd8a-142">Request</span></span>
<span data-ttu-id="1fd8a-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fd8a-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1fd8a-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fd8a-144">Response</span></span>
<span data-ttu-id="1fd8a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1fd8a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




