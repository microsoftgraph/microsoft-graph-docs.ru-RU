---
title: Обновление windowsQualityUpdateProfileAssignment
description: Обновление свойств объекта windowsQualityUpdateProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b994c483fd24e7865ad2c73f17d77b7c086b3ec2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160712"
---
# <a name="update-windowsqualityupdateprofileassignment"></a><span data-ttu-id="d9921-103">Обновление windowsQualityUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="d9921-103">Update windowsQualityUpdateProfileAssignment</span></span>

<span data-ttu-id="d9921-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9921-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9921-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9921-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9921-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9921-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9921-107">Обновление свойств объекта [windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d9921-107">Update the properties of a [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9921-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d9921-108">Prerequisites</span></span>
<span data-ttu-id="d9921-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9921-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9921-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9921-111">Permission type</span></span>|<span data-ttu-id="d9921-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9921-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9921-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9921-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9921-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9921-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9921-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9921-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9921-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9921-116">Not supported.</span></span>|
|<span data-ttu-id="d9921-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9921-117">Application</span></span>|<span data-ttu-id="d9921-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9921-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9921-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9921-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}/assignments/{windowsQualityUpdateProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d9921-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d9921-120">Request headers</span></span>
|<span data-ttu-id="d9921-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d9921-121">Header</span></span>|<span data-ttu-id="d9921-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d9921-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9921-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9921-123">Authorization</span></span>|<span data-ttu-id="d9921-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9921-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9921-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d9921-125">Accept</span></span>|<span data-ttu-id="d9921-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9921-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9921-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9921-127">Request body</span></span>
<span data-ttu-id="d9921-128">В теле запроса укажу представление объекта [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="d9921-128">In the request body, supply a JSON representation for the [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) object.</span></span>

<span data-ttu-id="d9921-129">В следующей таблице показаны свойства, необходимые при создании [объекта windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d9921-129">The following table shows the properties that are required when you create the [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md).</span></span>

|<span data-ttu-id="d9921-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9921-130">Property</span></span>|<span data-ttu-id="d9921-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d9921-131">Type</span></span>|<span data-ttu-id="d9921-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d9921-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9921-133">id</span><span class="sxs-lookup"><span data-stu-id="d9921-133">id</span></span>|<span data-ttu-id="d9921-134">String</span><span class="sxs-lookup"><span data-stu-id="d9921-134">String</span></span>|<span data-ttu-id="d9921-135">Идентификатор сущности</span><span class="sxs-lookup"><span data-stu-id="d9921-135">The Identifier of the entity</span></span>|
|<span data-ttu-id="d9921-136">target</span><span class="sxs-lookup"><span data-stu-id="d9921-136">target</span></span>|[<span data-ttu-id="d9921-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d9921-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d9921-138">Целевой объект назначения, который назначен профилю обновления функций.</span><span class="sxs-lookup"><span data-stu-id="d9921-138">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="d9921-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9921-139">Response</span></span>
<span data-ttu-id="d9921-140">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d9921-140">If successful, this method returns a `200 OK` response code and an updated [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9921-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d9921-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9921-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9921-142">Request</span></span>
<span data-ttu-id="d9921-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9921-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}/assignments/{windowsQualityUpdateProfileAssignmentId}
Content-type: application/json
Content-length: 344

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="d9921-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9921-144">Response</span></span>
<span data-ttu-id="d9921-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9921-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 393

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfileAssignment",
  "id": "0c3a8422-8422-0c3a-2284-3a0c22843a0c",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




