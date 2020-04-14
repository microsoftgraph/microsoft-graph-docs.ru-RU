---
title: Обновление Виндовсфеатуреупдатепрофилеассигнмент
description: Обновление свойств объекта Виндовсфеатуреупдатепрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3b808fea3a16da8d02d8e7cb54dae112c1aef09c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457579"
---
# <a name="update-windowsfeatureupdateprofileassignment"></a><span data-ttu-id="9f986-103">Обновление Виндовсфеатуреупдатепрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="9f986-103">Update windowsFeatureUpdateProfileAssignment</span></span>

<span data-ttu-id="9f986-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f986-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f986-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f986-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f986-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f986-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f986-107">Обновление свойств объекта [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9f986-107">Update the properties of a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f986-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f986-108">Prerequisites</span></span>
<span data-ttu-id="9f986-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f986-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f986-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f986-111">Permission type</span></span>|<span data-ttu-id="9f986-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f986-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f986-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f986-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f986-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f986-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f986-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f986-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f986-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f986-116">Not supported.</span></span>|
|<span data-ttu-id="9f986-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f986-117">Application</span></span>|<span data-ttu-id="9f986-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f986-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f986-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f986-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9f986-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9f986-120">Request headers</span></span>
|<span data-ttu-id="9f986-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f986-121">Header</span></span>|<span data-ttu-id="9f986-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9f986-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f986-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f986-123">Authorization</span></span>|<span data-ttu-id="9f986-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f986-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f986-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9f986-125">Accept</span></span>|<span data-ttu-id="9f986-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f986-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f986-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f986-127">Request body</span></span>
<span data-ttu-id="9f986-128">В тексте запроса добавьте представление объекта [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f986-128">In the request body, supply a JSON representation for the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

<span data-ttu-id="9f986-129">В следующей таблице приведены свойства, необходимые при создании [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9f986-129">The following table shows the properties that are required when you create the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).</span></span>

|<span data-ttu-id="9f986-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f986-130">Property</span></span>|<span data-ttu-id="9f986-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9f986-131">Type</span></span>|<span data-ttu-id="9f986-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9f986-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f986-133">id</span><span class="sxs-lookup"><span data-stu-id="9f986-133">id</span></span>|<span data-ttu-id="9f986-134">String</span><span class="sxs-lookup"><span data-stu-id="9f986-134">String</span></span>|<span data-ttu-id="9f986-135">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="9f986-135">The Identifier of the entity</span></span>|
|<span data-ttu-id="9f986-136">target</span><span class="sxs-lookup"><span data-stu-id="9f986-136">target</span></span>|[<span data-ttu-id="9f986-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9f986-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9f986-138">Цель назначения, которой назначен профиль обновления компонента.</span><span class="sxs-lookup"><span data-stu-id="9f986-138">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="9f986-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f986-139">Response</span></span>
<span data-ttu-id="9f986-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f986-140">If successful, this method returns a `200 OK` response code and an updated [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f986-141">Пример</span><span class="sxs-lookup"><span data-stu-id="9f986-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f986-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f986-142">Request</span></span>
<span data-ttu-id="9f986-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f986-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
Content-type: application/json
Content-length: 177

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="9f986-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f986-144">Response</span></span>
<span data-ttu-id="9f986-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f986-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 226

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "id": "567a744f-744f-567a-4f74-7a564f747a56",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



