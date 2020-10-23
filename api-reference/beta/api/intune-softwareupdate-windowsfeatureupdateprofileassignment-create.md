---
title: Создание Виндовсфеатуреупдатепрофилеассигнмент
description: Создание нового объекта Виндовсфеатуреупдатепрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 09ebd4853548aa3e3d8ebc628177404400826541
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695210"
---
# <a name="create-windowsfeatureupdateprofileassignment"></a><span data-ttu-id="69b08-103">Создание Виндовсфеатуреупдатепрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="69b08-103">Create windowsFeatureUpdateProfileAssignment</span></span>

<span data-ttu-id="69b08-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69b08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69b08-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69b08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69b08-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="69b08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69b08-107">Создание нового объекта [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="69b08-107">Create a new [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69b08-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="69b08-108">Prerequisites</span></span>
<span data-ttu-id="69b08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69b08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69b08-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69b08-111">Permission type</span></span>|<span data-ttu-id="69b08-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="69b08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69b08-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69b08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69b08-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b08-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69b08-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69b08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69b08-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69b08-116">Not supported.</span></span>|
|<span data-ttu-id="69b08-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69b08-117">Application</span></span>|<span data-ttu-id="69b08-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b08-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69b08-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69b08-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="69b08-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="69b08-120">Request headers</span></span>
|<span data-ttu-id="69b08-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69b08-121">Header</span></span>|<span data-ttu-id="69b08-122">Значение</span><span class="sxs-lookup"><span data-stu-id="69b08-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69b08-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69b08-123">Authorization</span></span>|<span data-ttu-id="69b08-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69b08-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69b08-125">Accept</span><span class="sxs-lookup"><span data-stu-id="69b08-125">Accept</span></span>|<span data-ttu-id="69b08-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69b08-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69b08-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69b08-127">Request body</span></span>
<span data-ttu-id="69b08-128">В тексте запроса добавьте представление объекта Виндовсфеатуреупдатепрофилеассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69b08-128">In the request body, supply a JSON representation for the windowsFeatureUpdateProfileAssignment object.</span></span>

<span data-ttu-id="69b08-129">В следующей таблице приведены свойства, необходимые при создании Виндовсфеатуреупдатепрофилеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="69b08-129">The following table shows the properties that are required when you create the windowsFeatureUpdateProfileAssignment.</span></span>

|<span data-ttu-id="69b08-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="69b08-130">Property</span></span>|<span data-ttu-id="69b08-131">Тип</span><span class="sxs-lookup"><span data-stu-id="69b08-131">Type</span></span>|<span data-ttu-id="69b08-132">Описание</span><span class="sxs-lookup"><span data-stu-id="69b08-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69b08-133">id</span><span class="sxs-lookup"><span data-stu-id="69b08-133">id</span></span>|<span data-ttu-id="69b08-134">Строка</span><span class="sxs-lookup"><span data-stu-id="69b08-134">String</span></span>|<span data-ttu-id="69b08-135">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="69b08-135">The Identifier of the entity</span></span>|
|<span data-ttu-id="69b08-136">target</span><span class="sxs-lookup"><span data-stu-id="69b08-136">target</span></span>|[<span data-ttu-id="69b08-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="69b08-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="69b08-138">Цель назначения, которой назначен профиль обновления компонента.</span><span class="sxs-lookup"><span data-stu-id="69b08-138">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="69b08-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="69b08-139">Response</span></span>
<span data-ttu-id="69b08-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69b08-140">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69b08-141">Пример</span><span class="sxs-lookup"><span data-stu-id="69b08-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="69b08-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="69b08-142">Request</span></span>
<span data-ttu-id="69b08-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69b08-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="69b08-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="69b08-144">Response</span></span>
<span data-ttu-id="69b08-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69b08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





