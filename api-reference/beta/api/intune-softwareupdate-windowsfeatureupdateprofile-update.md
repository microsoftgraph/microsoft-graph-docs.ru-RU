---
title: Обновление Виндовсфеатуреупдатепрофиле
description: Обновление свойств объекта Виндовсфеатуреупдатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 686450bd34be0f251de0c6bc898761d63cfc1a37
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123577"
---
# <a name="update-windowsfeatureupdateprofile"></a><span data-ttu-id="6895a-103">Обновление Виндовсфеатуреупдатепрофиле</span><span class="sxs-lookup"><span data-stu-id="6895a-103">Update windowsFeatureUpdateProfile</span></span>

<span data-ttu-id="6895a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6895a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6895a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6895a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6895a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6895a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6895a-107">Обновление свойств объекта [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6895a-107">Update the properties of a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6895a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6895a-108">Prerequisites</span></span>
<span data-ttu-id="6895a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6895a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6895a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6895a-111">Permission type</span></span>|<span data-ttu-id="6895a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6895a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6895a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6895a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6895a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6895a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6895a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6895a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6895a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6895a-116">Not supported.</span></span>|
|<span data-ttu-id="6895a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6895a-117">Application</span></span>|<span data-ttu-id="6895a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6895a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6895a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6895a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="6895a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6895a-120">Request headers</span></span>
|<span data-ttu-id="6895a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6895a-121">Header</span></span>|<span data-ttu-id="6895a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6895a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6895a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6895a-123">Authorization</span></span>|<span data-ttu-id="6895a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6895a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6895a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6895a-125">Accept</span></span>|<span data-ttu-id="6895a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6895a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6895a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6895a-127">Request body</span></span>
<span data-ttu-id="6895a-128">В тексте запроса добавьте представление объекта [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6895a-128">In the request body, supply a JSON representation for the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

<span data-ttu-id="6895a-129">В следующей таблице приведены свойства, необходимые при создании [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="6895a-129">The following table shows the properties that are required when you create the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).</span></span>

|<span data-ttu-id="6895a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6895a-130">Property</span></span>|<span data-ttu-id="6895a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6895a-131">Type</span></span>|<span data-ttu-id="6895a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6895a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6895a-133">id</span><span class="sxs-lookup"><span data-stu-id="6895a-133">id</span></span>|<span data-ttu-id="6895a-134">String</span><span class="sxs-lookup"><span data-stu-id="6895a-134">String</span></span>|<span data-ttu-id="6895a-135">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="6895a-135">The Identifier of the entity.</span></span>|
|<span data-ttu-id="6895a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6895a-136">displayName</span></span>|<span data-ttu-id="6895a-137">Строка</span><span class="sxs-lookup"><span data-stu-id="6895a-137">String</span></span>|<span data-ttu-id="6895a-138">Отображаемое имя профиля.</span><span class="sxs-lookup"><span data-stu-id="6895a-138">The display name of the profile.</span></span>|
|<span data-ttu-id="6895a-139">description</span><span class="sxs-lookup"><span data-stu-id="6895a-139">description</span></span>|<span data-ttu-id="6895a-140">String</span><span class="sxs-lookup"><span data-stu-id="6895a-140">String</span></span>|<span data-ttu-id="6895a-141">Описание профиля, указанного пользователем.</span><span class="sxs-lookup"><span data-stu-id="6895a-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="6895a-142">феатуреупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="6895a-142">featureUpdateVersion</span></span>|<span data-ttu-id="6895a-143">String</span><span class="sxs-lookup"><span data-stu-id="6895a-143">String</span></span>|<span data-ttu-id="6895a-144">Версия обновления компонентов, которая будет развернута на устройствах, предназначенных для этого профиля.</span><span class="sxs-lookup"><span data-stu-id="6895a-144">The feature update version that will be deployed to the devices targeted by this profile.</span></span> <span data-ttu-id="6895a-145">Версией может быть любая поддерживаемая версия, например 1709, 1803 или 1809 и т. д.</span><span class="sxs-lookup"><span data-stu-id="6895a-145">The version could be any supported version for example 1709, 1803 or 1809 and so on.</span></span>|
|<span data-ttu-id="6895a-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6895a-146">createdDateTime</span></span>|<span data-ttu-id="6895a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6895a-147">DateTimeOffset</span></span>|<span data-ttu-id="6895a-148">Дата и время создания профиля.</span><span class="sxs-lookup"><span data-stu-id="6895a-148">The date time that the profile was created.</span></span>|
|<span data-ttu-id="6895a-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6895a-149">lastModifiedDateTime</span></span>|<span data-ttu-id="6895a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6895a-150">DateTimeOffset</span></span>|<span data-ttu-id="6895a-151">Дата и время последнего изменения профиля.</span><span class="sxs-lookup"><span data-stu-id="6895a-151">The date time that the profile was last modified.</span></span>|
|<span data-ttu-id="6895a-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6895a-152">roleScopeTagIds</span></span>|<span data-ttu-id="6895a-153">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6895a-153">String collection</span></span>|<span data-ttu-id="6895a-154">Список тегов областей для этого элемента обновления компонента.</span><span class="sxs-lookup"><span data-stu-id="6895a-154">List of Scope Tags for this Feature Update entity.</span></span>|



## <a name="response"></a><span data-ttu-id="6895a-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="6895a-155">Response</span></span>
<span data-ttu-id="6895a-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6895a-156">If successful, this method returns a `200 OK` response code and an updated [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6895a-157">Пример</span><span class="sxs-lookup"><span data-stu-id="6895a-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="6895a-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="6895a-158">Request</span></span>
<span data-ttu-id="6895a-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6895a-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
Content-type: application/json
Content-length: 269

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="6895a-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="6895a-160">Response</span></span>
<span data-ttu-id="6895a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6895a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "id": "885bd4ee-d4ee-885b-eed4-5b88eed45b88",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```



