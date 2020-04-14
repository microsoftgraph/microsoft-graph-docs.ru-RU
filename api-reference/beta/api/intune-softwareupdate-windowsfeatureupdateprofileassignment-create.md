---
title: Создание Виндовсфеатуреупдатепрофилеассигнмент
description: Создание нового объекта Виндовсфеатуреупдатепрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 04f74ec382f1266bfceb9bbb438f655b9f464543
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457607"
---
# <a name="create-windowsfeatureupdateprofileassignment"></a><span data-ttu-id="53c54-103">Создание Виндовсфеатуреупдатепрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="53c54-103">Create windowsFeatureUpdateProfileAssignment</span></span>

<span data-ttu-id="53c54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53c54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53c54-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53c54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53c54-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53c54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53c54-107">Создание нового объекта [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="53c54-107">Create a new [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53c54-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="53c54-108">Prerequisites</span></span>
<span data-ttu-id="53c54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53c54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53c54-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53c54-111">Permission type</span></span>|<span data-ttu-id="53c54-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53c54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53c54-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53c54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53c54-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53c54-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="53c54-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53c54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53c54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53c54-116">Not supported.</span></span>|
|<span data-ttu-id="53c54-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53c54-117">Application</span></span>|<span data-ttu-id="53c54-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53c54-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53c54-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53c54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="53c54-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="53c54-120">Request headers</span></span>
|<span data-ttu-id="53c54-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53c54-121">Header</span></span>|<span data-ttu-id="53c54-122">Значение</span><span class="sxs-lookup"><span data-stu-id="53c54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53c54-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53c54-123">Authorization</span></span>|<span data-ttu-id="53c54-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53c54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53c54-125">Accept</span><span class="sxs-lookup"><span data-stu-id="53c54-125">Accept</span></span>|<span data-ttu-id="53c54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53c54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53c54-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="53c54-127">Request body</span></span>
<span data-ttu-id="53c54-128">В тексте запроса добавьте представление объекта Виндовсфеатуреупдатепрофилеассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53c54-128">In the request body, supply a JSON representation for the windowsFeatureUpdateProfileAssignment object.</span></span>

<span data-ttu-id="53c54-129">В следующей таблице приведены свойства, необходимые при создании Виндовсфеатуреупдатепрофилеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="53c54-129">The following table shows the properties that are required when you create the windowsFeatureUpdateProfileAssignment.</span></span>

|<span data-ttu-id="53c54-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="53c54-130">Property</span></span>|<span data-ttu-id="53c54-131">Тип</span><span class="sxs-lookup"><span data-stu-id="53c54-131">Type</span></span>|<span data-ttu-id="53c54-132">Описание</span><span class="sxs-lookup"><span data-stu-id="53c54-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53c54-133">id</span><span class="sxs-lookup"><span data-stu-id="53c54-133">id</span></span>|<span data-ttu-id="53c54-134">String</span><span class="sxs-lookup"><span data-stu-id="53c54-134">String</span></span>|<span data-ttu-id="53c54-135">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="53c54-135">The Identifier of the entity</span></span>|
|<span data-ttu-id="53c54-136">target</span><span class="sxs-lookup"><span data-stu-id="53c54-136">target</span></span>|[<span data-ttu-id="53c54-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="53c54-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="53c54-138">Цель назначения, которой назначен профиль обновления компонента.</span><span class="sxs-lookup"><span data-stu-id="53c54-138">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="53c54-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="53c54-139">Response</span></span>
<span data-ttu-id="53c54-140">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53c54-140">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53c54-141">Пример</span><span class="sxs-lookup"><span data-stu-id="53c54-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="53c54-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="53c54-142">Request</span></span>
<span data-ttu-id="53c54-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53c54-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
Content-type: application/json
Content-length: 177

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="53c54-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="53c54-144">Response</span></span>
<span data-ttu-id="53c54-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53c54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



