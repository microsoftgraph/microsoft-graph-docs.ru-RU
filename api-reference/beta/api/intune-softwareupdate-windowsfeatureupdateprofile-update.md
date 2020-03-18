---
title: Обновление Виндовсфеатуреупдатепрофиле
description: Обновление свойств объекта Виндовсфеатуреупдатепрофиле.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f79c22deb2738ce92d3b9fc17be5c14871ff1ff5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800377"
---
# <a name="update-windowsfeatureupdateprofile"></a><span data-ttu-id="bb9d6-103">Обновление Виндовсфеатуреупдатепрофиле</span><span class="sxs-lookup"><span data-stu-id="bb9d6-103">Update windowsFeatureUpdateProfile</span></span>

> <span data-ttu-id="bb9d6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb9d6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb9d6-106">Обновление свойств объекта [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="bb9d6-106">Update the properties of a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb9d6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bb9d6-107">Prerequisites</span></span>
<span data-ttu-id="bb9d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb9d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb9d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb9d6-110">Permission type</span></span>|<span data-ttu-id="bb9d6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb9d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb9d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb9d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb9d6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb9d6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb9d6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb9d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb9d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-115">Not supported.</span></span>|
|<span data-ttu-id="bb9d6-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="bb9d6-116">Application</span></span>|<span data-ttu-id="bb9d6-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb9d6-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb9d6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb9d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="bb9d6-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bb9d6-119">Request headers</span></span>
|<span data-ttu-id="bb9d6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb9d6-120">Header</span></span>|<span data-ttu-id="bb9d6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bb9d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb9d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb9d6-122">Authorization</span></span>|<span data-ttu-id="bb9d6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb9d6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bb9d6-124">Accept</span></span>|<span data-ttu-id="bb9d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb9d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb9d6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb9d6-126">Request body</span></span>
<span data-ttu-id="bb9d6-127">В тексте запроса добавьте представление объекта [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-127">In the request body, supply a JSON representation for the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

<span data-ttu-id="bb9d6-128">В следующей таблице приведены свойства, необходимые при создании [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="bb9d6-128">The following table shows the properties that are required when you create the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).</span></span>

|<span data-ttu-id="bb9d6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb9d6-129">Property</span></span>|<span data-ttu-id="bb9d6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bb9d6-130">Type</span></span>|<span data-ttu-id="bb9d6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bb9d6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb9d6-132">id</span><span class="sxs-lookup"><span data-stu-id="bb9d6-132">id</span></span>|<span data-ttu-id="bb9d6-133">String</span><span class="sxs-lookup"><span data-stu-id="bb9d6-133">String</span></span>|<span data-ttu-id="bb9d6-134">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-134">The Identifier of the entity.</span></span>|
|<span data-ttu-id="bb9d6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="bb9d6-135">displayName</span></span>|<span data-ttu-id="bb9d6-136">Строка</span><span class="sxs-lookup"><span data-stu-id="bb9d6-136">String</span></span>|<span data-ttu-id="bb9d6-137">Отображаемое имя профиля.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-137">The display name of the profile.</span></span>|
|<span data-ttu-id="bb9d6-138">description</span><span class="sxs-lookup"><span data-stu-id="bb9d6-138">description</span></span>|<span data-ttu-id="bb9d6-139">String</span><span class="sxs-lookup"><span data-stu-id="bb9d6-139">String</span></span>|<span data-ttu-id="bb9d6-140">Описание профиля, указанного пользователем.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-140">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="bb9d6-141">феатуреупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="bb9d6-141">featureUpdateVersion</span></span>|<span data-ttu-id="bb9d6-142">String</span><span class="sxs-lookup"><span data-stu-id="bb9d6-142">String</span></span>|<span data-ttu-id="bb9d6-143">Версия обновления компонентов, которая будет развернута на устройствах, предназначенных для этого профиля.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-143">The feature update version that will be deployed to the devices targeted by this profile.</span></span> <span data-ttu-id="bb9d6-144">Версией может быть любая поддерживаемая версия, например 1709, 1803 или 1809 и т. д.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-144">The version could be any supported version for example 1709, 1803 or 1809 and so on.</span></span>|
|<span data-ttu-id="bb9d6-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb9d6-145">createdDateTime</span></span>|<span data-ttu-id="bb9d6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb9d6-146">DateTimeOffset</span></span>|<span data-ttu-id="bb9d6-147">Дата и время создания профиля.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-147">The date time that the profile was created.</span></span>|
|<span data-ttu-id="bb9d6-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb9d6-148">lastModifiedDateTime</span></span>|<span data-ttu-id="bb9d6-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb9d6-149">DateTimeOffset</span></span>|<span data-ttu-id="bb9d6-150">Дата и время последнего изменения профиля.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-150">The date time that the profile was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="bb9d6-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb9d6-151">Response</span></span>
<span data-ttu-id="bb9d6-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-152">If successful, this method returns a `200 OK` response code and an updated [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb9d6-153">Пример</span><span class="sxs-lookup"><span data-stu-id="bb9d6-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb9d6-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb9d6-154">Request</span></span>
<span data-ttu-id="bb9d6-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
Content-type: application/json
Content-length: 207

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value"
}
```

### <a name="response"></a><span data-ttu-id="bb9d6-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb9d6-156">Response</span></span>
<span data-ttu-id="bb9d6-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb9d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 379

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "id": "885bd4ee-d4ee-885b-eed4-5b88eed45b88",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




