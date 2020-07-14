---
title: Создание Виндовсфеатуреупдатепрофиле
description: Создание нового объекта Виндовсфеатуреупдатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b2f5b68a0cb3f2773b2ea6ab933cbf341515811e
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124011"
---
# <a name="create-windowsfeatureupdateprofile"></a><span data-ttu-id="ddb6e-103">Создание Виндовсфеатуреупдатепрофиле</span><span class="sxs-lookup"><span data-stu-id="ddb6e-103">Create windowsFeatureUpdateProfile</span></span>

<span data-ttu-id="ddb6e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddb6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ddb6e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddb6e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddb6e-107">Создание нового объекта [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ddb6e-107">Create a new [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddb6e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ddb6e-108">Prerequisites</span></span>
<span data-ttu-id="ddb6e-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ddb6e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddb6e-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddb6e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddb6e-111">Permission type</span></span>|<span data-ttu-id="ddb6e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddb6e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddb6e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddb6e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ddb6e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb6e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ddb6e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddb6e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddb6e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-116">Not supported.</span></span>|
|<span data-ttu-id="ddb6e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddb6e-117">Application</span></span>|<span data-ttu-id="ddb6e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb6e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddb6e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddb6e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsFeatureUpdateProfiles
```

## <a name="request-headers"></a><span data-ttu-id="ddb6e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ddb6e-120">Request headers</span></span>
|<span data-ttu-id="ddb6e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ddb6e-121">Header</span></span>|<span data-ttu-id="ddb6e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ddb6e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddb6e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ddb6e-123">Authorization</span></span>|<span data-ttu-id="ddb6e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddb6e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ddb6e-125">Accept</span></span>|<span data-ttu-id="ddb6e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ddb6e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddb6e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddb6e-127">Request body</span></span>
<span data-ttu-id="ddb6e-128">В тексте запроса добавьте представление объекта Виндовсфеатуреупдатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-128">In the request body, supply a JSON representation for the windowsFeatureUpdateProfile object.</span></span>

<span data-ttu-id="ddb6e-129">В следующей таблице приведены свойства, необходимые при создании Виндовсфеатуреупдатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-129">The following table shows the properties that are required when you create the windowsFeatureUpdateProfile.</span></span>

|<span data-ttu-id="ddb6e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddb6e-130">Property</span></span>|<span data-ttu-id="ddb6e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ddb6e-131">Type</span></span>|<span data-ttu-id="ddb6e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ddb6e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddb6e-133">id</span><span class="sxs-lookup"><span data-stu-id="ddb6e-133">id</span></span>|<span data-ttu-id="ddb6e-134">String</span><span class="sxs-lookup"><span data-stu-id="ddb6e-134">String</span></span>|<span data-ttu-id="ddb6e-135">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-135">The Identifier of the entity.</span></span>|
|<span data-ttu-id="ddb6e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ddb6e-136">displayName</span></span>|<span data-ttu-id="ddb6e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="ddb6e-137">String</span></span>|<span data-ttu-id="ddb6e-138">Отображаемое имя профиля.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-138">The display name of the profile.</span></span>|
|<span data-ttu-id="ddb6e-139">description</span><span class="sxs-lookup"><span data-stu-id="ddb6e-139">description</span></span>|<span data-ttu-id="ddb6e-140">String</span><span class="sxs-lookup"><span data-stu-id="ddb6e-140">String</span></span>|<span data-ttu-id="ddb6e-141">Описание профиля, указанного пользователем.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="ddb6e-142">феатуреупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="ddb6e-142">featureUpdateVersion</span></span>|<span data-ttu-id="ddb6e-143">String</span><span class="sxs-lookup"><span data-stu-id="ddb6e-143">String</span></span>|<span data-ttu-id="ddb6e-144">Версия обновления компонентов, которая будет развернута на устройствах, предназначенных для этого профиля.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-144">The feature update version that will be deployed to the devices targeted by this profile.</span></span> <span data-ttu-id="ddb6e-145">Версией может быть любая поддерживаемая версия, например 1709, 1803 или 1809 и т. д.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-145">The version could be any supported version for example 1709, 1803 or 1809 and so on.</span></span>|
|<span data-ttu-id="ddb6e-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ddb6e-146">createdDateTime</span></span>|<span data-ttu-id="ddb6e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddb6e-147">DateTimeOffset</span></span>|<span data-ttu-id="ddb6e-148">Дата и время создания профиля.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-148">The date time that the profile was created.</span></span>|
|<span data-ttu-id="ddb6e-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddb6e-149">lastModifiedDateTime</span></span>|<span data-ttu-id="ddb6e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddb6e-150">DateTimeOffset</span></span>|<span data-ttu-id="ddb6e-151">Дата и время последнего изменения профиля.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-151">The date time that the profile was last modified.</span></span>|
|<span data-ttu-id="ddb6e-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ddb6e-152">roleScopeTagIds</span></span>|<span data-ttu-id="ddb6e-153">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ddb6e-153">String collection</span></span>|<span data-ttu-id="ddb6e-154">Список тегов областей для этого элемента обновления компонента.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-154">List of Scope Tags for this Feature Update entity.</span></span>|



## <a name="response"></a><span data-ttu-id="ddb6e-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddb6e-155">Response</span></span>
<span data-ttu-id="ddb6e-156">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсфеатуреупдатепрофиле](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-156">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddb6e-157">Пример</span><span class="sxs-lookup"><span data-stu-id="ddb6e-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddb6e-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddb6e-158">Request</span></span>
<span data-ttu-id="ddb6e-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles
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

### <a name="response"></a><span data-ttu-id="ddb6e-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddb6e-160">Response</span></span>
<span data-ttu-id="ddb6e-161">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-161">Here is an example of the response.</span></span> <span data-ttu-id="ddb6e-162">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-162">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ddb6e-163">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="ddb6e-163">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



