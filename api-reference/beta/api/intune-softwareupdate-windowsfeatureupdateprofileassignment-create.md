---
title: Создание Виндовсфеатуреупдатепрофилеассигнмент
description: Создание нового объекта Виндовсфеатуреупдатепрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3af8015708c8dd2563a6e76ef3f92f9e0337efb7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49200568"
---
# <a name="create-windowsfeatureupdateprofileassignment"></a><span data-ttu-id="bb4cf-103">Создание Виндовсфеатуреупдатепрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="bb4cf-103">Create windowsFeatureUpdateProfileAssignment</span></span>

<span data-ttu-id="bb4cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb4cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb4cf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb4cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb4cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb4cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb4cf-107">Создание нового объекта [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="bb4cf-107">Create a new [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb4cf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bb4cf-108">Prerequisites</span></span>
<span data-ttu-id="bb4cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb4cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb4cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb4cf-111">Permission type</span></span>|<span data-ttu-id="bb4cf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb4cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb4cf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb4cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb4cf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb4cf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb4cf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb4cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb4cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb4cf-116">Not supported.</span></span>|
|<span data-ttu-id="bb4cf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bb4cf-117">Application</span></span>|<span data-ttu-id="bb4cf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb4cf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb4cf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb4cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="bb4cf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bb4cf-120">Request headers</span></span>
|<span data-ttu-id="bb4cf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb4cf-121">Header</span></span>|<span data-ttu-id="bb4cf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bb4cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb4cf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb4cf-123">Authorization</span></span>|<span data-ttu-id="bb4cf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb4cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb4cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bb4cf-125">Accept</span></span>|<span data-ttu-id="bb4cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb4cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb4cf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb4cf-127">Request body</span></span>
<span data-ttu-id="bb4cf-128">В тексте запроса добавьте представление объекта Виндовсфеатуреупдатепрофилеассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb4cf-128">In the request body, supply a JSON representation for the windowsFeatureUpdateProfileAssignment object.</span></span>

<span data-ttu-id="bb4cf-129">В следующей таблице приведены свойства, необходимые при создании Виндовсфеатуреупдатепрофилеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="bb4cf-129">The following table shows the properties that are required when you create the windowsFeatureUpdateProfileAssignment.</span></span>

|<span data-ttu-id="bb4cf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb4cf-130">Property</span></span>|<span data-ttu-id="bb4cf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bb4cf-131">Type</span></span>|<span data-ttu-id="bb4cf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bb4cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb4cf-133">id</span><span class="sxs-lookup"><span data-stu-id="bb4cf-133">id</span></span>|<span data-ttu-id="bb4cf-134">String</span><span class="sxs-lookup"><span data-stu-id="bb4cf-134">String</span></span>|<span data-ttu-id="bb4cf-135">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="bb4cf-135">The Identifier of the entity</span></span>|
|<span data-ttu-id="bb4cf-136">target</span><span class="sxs-lookup"><span data-stu-id="bb4cf-136">target</span></span>|[<span data-ttu-id="bb4cf-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bb4cf-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bb4cf-138">Цель назначения, которой назначен профиль обновления компонента.</span><span class="sxs-lookup"><span data-stu-id="bb4cf-138">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="bb4cf-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb4cf-139">Response</span></span>
<span data-ttu-id="bb4cf-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb4cf-140">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb4cf-141">Пример</span><span class="sxs-lookup"><span data-stu-id="bb4cf-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb4cf-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb4cf-142">Request</span></span>
<span data-ttu-id="bb4cf-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb4cf-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
Content-type: application/json
Content-length: 344

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="bb4cf-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb4cf-144">Response</span></span>
<span data-ttu-id="bb4cf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb4cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 393

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "id": "567a744f-744f-567a-4f74-7a564f747a56",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




