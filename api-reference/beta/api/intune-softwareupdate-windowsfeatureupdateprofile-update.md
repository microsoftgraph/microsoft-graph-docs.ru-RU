---
title: Обновление Виндовсфеатуреупдатепрофиле
description: Обновление свойств объекта Виндовсфеатуреупдатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 230d2dc672a1f0c24caa712eba77e0cd595dc12d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295763"
---
# <a name="update-windowsfeatureupdateprofile"></a><span data-ttu-id="6ddc1-103">Обновление Виндовсфеатуреупдатепрофиле</span><span class="sxs-lookup"><span data-stu-id="6ddc1-103">Update windowsFeatureUpdateProfile</span></span>

<span data-ttu-id="6ddc1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ddc1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ddc1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ddc1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ddc1-107">Обновление свойств объекта [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6ddc1-107">Update the properties of a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ddc1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6ddc1-108">Prerequisites</span></span>
<span data-ttu-id="6ddc1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ddc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ddc1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ddc1-111">Permission type</span></span>|<span data-ttu-id="6ddc1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ddc1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ddc1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ddc1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ddc1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ddc1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ddc1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ddc1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ddc1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-116">Not supported.</span></span>|
|<span data-ttu-id="6ddc1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ddc1-117">Application</span></span>|<span data-ttu-id="6ddc1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ddc1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ddc1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ddc1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="6ddc1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6ddc1-120">Request headers</span></span>
|<span data-ttu-id="6ddc1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ddc1-121">Header</span></span>|<span data-ttu-id="6ddc1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6ddc1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ddc1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ddc1-123">Authorization</span></span>|<span data-ttu-id="6ddc1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ddc1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6ddc1-125">Accept</span></span>|<span data-ttu-id="6ddc1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ddc1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ddc1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ddc1-127">Request body</span></span>
<span data-ttu-id="6ddc1-128">В тексте запроса добавьте представление объекта [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-128">In the request body, supply a JSON representation for the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

<span data-ttu-id="6ddc1-129">В следующей таблице приведены свойства, необходимые при создании [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="6ddc1-129">The following table shows the properties that are required when you create the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).</span></span>

|<span data-ttu-id="6ddc1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ddc1-130">Property</span></span>|<span data-ttu-id="6ddc1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6ddc1-131">Type</span></span>|<span data-ttu-id="6ddc1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6ddc1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ddc1-133">id</span><span class="sxs-lookup"><span data-stu-id="6ddc1-133">id</span></span>|<span data-ttu-id="6ddc1-134">String</span><span class="sxs-lookup"><span data-stu-id="6ddc1-134">String</span></span>|<span data-ttu-id="6ddc1-135">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-135">The Identifier of the entity.</span></span>|
|<span data-ttu-id="6ddc1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6ddc1-136">displayName</span></span>|<span data-ttu-id="6ddc1-137">String</span><span class="sxs-lookup"><span data-stu-id="6ddc1-137">String</span></span>|<span data-ttu-id="6ddc1-138">Отображаемое имя профиля.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-138">The display name of the profile.</span></span>|
|<span data-ttu-id="6ddc1-139">description</span><span class="sxs-lookup"><span data-stu-id="6ddc1-139">description</span></span>|<span data-ttu-id="6ddc1-140">String</span><span class="sxs-lookup"><span data-stu-id="6ddc1-140">String</span></span>|<span data-ttu-id="6ddc1-141">Описание профиля, указанного пользователем.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="6ddc1-142">феатуреупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="6ddc1-142">featureUpdateVersion</span></span>|<span data-ttu-id="6ddc1-143">String</span><span class="sxs-lookup"><span data-stu-id="6ddc1-143">String</span></span>|<span data-ttu-id="6ddc1-144">Версия обновления компонентов, которая будет развернута на устройствах, предназначенных для этого профиля.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-144">The feature update version that will be deployed to the devices targeted by this profile.</span></span> <span data-ttu-id="6ddc1-145">Версией может быть любая поддерживаемая версия, например 1709, 1803 или 1809 и т. д.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-145">The version could be any supported version for example 1709, 1803 or 1809 and so on.</span></span>|
|<span data-ttu-id="6ddc1-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ddc1-146">createdDateTime</span></span>|<span data-ttu-id="6ddc1-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ddc1-147">DateTimeOffset</span></span>|<span data-ttu-id="6ddc1-148">Дата и время создания профиля.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-148">The date time that the profile was created.</span></span>|
|<span data-ttu-id="6ddc1-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ddc1-149">lastModifiedDateTime</span></span>|<span data-ttu-id="6ddc1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ddc1-150">DateTimeOffset</span></span>|<span data-ttu-id="6ddc1-151">Дата и время последнего изменения профиля.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-151">The date time that the profile was last modified.</span></span>|
|<span data-ttu-id="6ddc1-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6ddc1-152">roleScopeTagIds</span></span>|<span data-ttu-id="6ddc1-153">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6ddc1-153">String collection</span></span>|<span data-ttu-id="6ddc1-154">Список тегов областей для этого элемента обновления компонента.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-154">List of Scope Tags for this Feature Update entity.</span></span>|



## <a name="response"></a><span data-ttu-id="6ddc1-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ddc1-155">Response</span></span>
<span data-ttu-id="6ddc1-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-156">If successful, this method returns a `200 OK` response code and an updated [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ddc1-157">Пример</span><span class="sxs-lookup"><span data-stu-id="6ddc1-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ddc1-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ddc1-158">Request</span></span>
<span data-ttu-id="6ddc1-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6ddc1-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ddc1-160">Response</span></span>
<span data-ttu-id="6ddc1-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ddc1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




