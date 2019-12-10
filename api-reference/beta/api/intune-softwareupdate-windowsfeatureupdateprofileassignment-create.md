---
title: Создание Виндовсфеатуреупдатепрофилеассигнмент
description: Создание нового объекта Виндовсфеатуреупдатепрофилеассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a970c57f5826169d7d2ddda977c4444188e347ea
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939264"
---
# <a name="create-windowsfeatureupdateprofileassignment"></a><span data-ttu-id="adfe4-103">Создание Виндовсфеатуреупдатепрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="adfe4-103">Create windowsFeatureUpdateProfileAssignment</span></span>

> <span data-ttu-id="adfe4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adfe4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adfe4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="adfe4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adfe4-106">Создание нового объекта [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="adfe4-106">Create a new [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="adfe4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="adfe4-107">Prerequisites</span></span>
<span data-ttu-id="adfe4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adfe4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adfe4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="adfe4-110">Permission type</span></span>|<span data-ttu-id="adfe4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="adfe4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adfe4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="adfe4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="adfe4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adfe4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="adfe4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="adfe4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adfe4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adfe4-115">Not supported.</span></span>|
|<span data-ttu-id="adfe4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="adfe4-116">Application</span></span>|<span data-ttu-id="adfe4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adfe4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="adfe4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="adfe4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="adfe4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="adfe4-119">Request headers</span></span>
|<span data-ttu-id="adfe4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="adfe4-120">Header</span></span>|<span data-ttu-id="adfe4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="adfe4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adfe4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="adfe4-122">Authorization</span></span>|<span data-ttu-id="adfe4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="adfe4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adfe4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="adfe4-124">Accept</span></span>|<span data-ttu-id="adfe4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="adfe4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adfe4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="adfe4-126">Request body</span></span>
<span data-ttu-id="adfe4-127">В тексте запроса добавьте представление объекта Виндовсфеатуреупдатепрофилеассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adfe4-127">In the request body, supply a JSON representation for the windowsFeatureUpdateProfileAssignment object.</span></span>

<span data-ttu-id="adfe4-128">В следующей таблице приведены свойства, необходимые при создании Виндовсфеатуреупдатепрофилеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="adfe4-128">The following table shows the properties that are required when you create the windowsFeatureUpdateProfileAssignment.</span></span>

|<span data-ttu-id="adfe4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="adfe4-129">Property</span></span>|<span data-ttu-id="adfe4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="adfe4-130">Type</span></span>|<span data-ttu-id="adfe4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="adfe4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adfe4-132">id</span><span class="sxs-lookup"><span data-stu-id="adfe4-132">id</span></span>|<span data-ttu-id="adfe4-133">Строка</span><span class="sxs-lookup"><span data-stu-id="adfe4-133">String</span></span>|<span data-ttu-id="adfe4-134">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="adfe4-134">The Identifier of the entity</span></span>|
|<span data-ttu-id="adfe4-135">target</span><span class="sxs-lookup"><span data-stu-id="adfe4-135">target</span></span>|[<span data-ttu-id="adfe4-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="adfe4-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="adfe4-137">Цель назначения, которой назначен профиль обновления компонента.</span><span class="sxs-lookup"><span data-stu-id="adfe4-137">The assignment target that the feature update profile is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="adfe4-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="adfe4-138">Response</span></span>
<span data-ttu-id="adfe4-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="adfe4-139">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adfe4-140">Пример</span><span class="sxs-lookup"><span data-stu-id="adfe4-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="adfe4-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="adfe4-141">Request</span></span>
<span data-ttu-id="adfe4-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adfe4-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="adfe4-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="adfe4-143">Response</span></span>
<span data-ttu-id="adfe4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="adfe4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





