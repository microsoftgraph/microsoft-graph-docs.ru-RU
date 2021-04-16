---
title: Создание windowsFeatureUpdateProfile
description: Создайте новый объект windowsFeatureUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3f4f727455c735e130eb39cf395d7f7a0ff35030
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865364"
---
# <a name="create-windowsfeatureupdateprofile"></a><span data-ttu-id="6bfe1-103">Создание windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="6bfe1-103">Create windowsFeatureUpdateProfile</span></span>

<span data-ttu-id="6bfe1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bfe1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6bfe1-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bfe1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bfe1-107">Создайте [новый объект windowsFeatureUpdateProfile.](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6bfe1-107">Create a new [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6bfe1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6bfe1-108">Prerequisites</span></span>
<span data-ttu-id="6bfe1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bfe1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bfe1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6bfe1-111">Permission type</span></span>|<span data-ttu-id="6bfe1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6bfe1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bfe1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6bfe1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6bfe1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bfe1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6bfe1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6bfe1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bfe1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-116">Not supported.</span></span>|
|<span data-ttu-id="6bfe1-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6bfe1-117">Application</span></span>|<span data-ttu-id="6bfe1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bfe1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bfe1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6bfe1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsFeatureUpdateProfiles
```

## <a name="request-headers"></a><span data-ttu-id="6bfe1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6bfe1-120">Request headers</span></span>
|<span data-ttu-id="6bfe1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6bfe1-121">Header</span></span>|<span data-ttu-id="6bfe1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6bfe1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bfe1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6bfe1-123">Authorization</span></span>|<span data-ttu-id="6bfe1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bfe1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6bfe1-125">Accept</span></span>|<span data-ttu-id="6bfe1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6bfe1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bfe1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6bfe1-127">Request body</span></span>
<span data-ttu-id="6bfe1-128">В теле запроса поставляем представление JSON для объекта windowsFeatureUpdateProfile.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-128">In the request body, supply a JSON representation for the windowsFeatureUpdateProfile object.</span></span>

<span data-ttu-id="6bfe1-129">В следующей таблице показаны свойства, необходимые при создании windowsFeatureUpdateProfile.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-129">The following table shows the properties that are required when you create the windowsFeatureUpdateProfile.</span></span>

|<span data-ttu-id="6bfe1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6bfe1-130">Property</span></span>|<span data-ttu-id="6bfe1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6bfe1-131">Type</span></span>|<span data-ttu-id="6bfe1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6bfe1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bfe1-133">id</span><span class="sxs-lookup"><span data-stu-id="6bfe1-133">id</span></span>|<span data-ttu-id="6bfe1-134">String</span><span class="sxs-lookup"><span data-stu-id="6bfe1-134">String</span></span>|<span data-ttu-id="6bfe1-135">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-135">The Identifier of the entity.</span></span>|
|<span data-ttu-id="6bfe1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6bfe1-136">displayName</span></span>|<span data-ttu-id="6bfe1-137">String</span><span class="sxs-lookup"><span data-stu-id="6bfe1-137">String</span></span>|<span data-ttu-id="6bfe1-138">Имя отображения профиля.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-138">The display name of the profile.</span></span>|
|<span data-ttu-id="6bfe1-139">description</span><span class="sxs-lookup"><span data-stu-id="6bfe1-139">description</span></span>|<span data-ttu-id="6bfe1-140">String</span><span class="sxs-lookup"><span data-stu-id="6bfe1-140">String</span></span>|<span data-ttu-id="6bfe1-141">Описание профиля, указанного пользователем.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="6bfe1-142">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="6bfe1-142">featureUpdateVersion</span></span>|<span data-ttu-id="6bfe1-143">String</span><span class="sxs-lookup"><span data-stu-id="6bfe1-143">String</span></span>|<span data-ttu-id="6bfe1-144">Версия обновления функций, которая будет развернута на устройствах, на которые ориентирован этот профиль.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-144">The feature update version that will be deployed to the devices targeted by this profile.</span></span> <span data-ttu-id="6bfe1-145">Версия может быть любой поддерживаемой версией, например 1709, 1803 или 1809 и так далее.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-145">The version could be any supported version for example 1709, 1803 or 1809 and so on.</span></span>|
|<span data-ttu-id="6bfe1-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6bfe1-146">createdDateTime</span></span>|<span data-ttu-id="6bfe1-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bfe1-147">DateTimeOffset</span></span>|<span data-ttu-id="6bfe1-148">Время создания профиля.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-148">The date time that the profile was created.</span></span>|
|<span data-ttu-id="6bfe1-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6bfe1-149">lastModifiedDateTime</span></span>|<span data-ttu-id="6bfe1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bfe1-150">DateTimeOffset</span></span>|<span data-ttu-id="6bfe1-151">Дата последнего изменения профиля.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-151">The date time that the profile was last modified.</span></span>|
|<span data-ttu-id="6bfe1-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6bfe1-152">roleScopeTagIds</span></span>|<span data-ttu-id="6bfe1-153">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6bfe1-153">String collection</span></span>|<span data-ttu-id="6bfe1-154">Список тегов области для этого объекта обновления функций.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-154">List of Scope Tags for this Feature Update entity.</span></span>|
|<span data-ttu-id="6bfe1-155">deployableContentDisplayName</span><span class="sxs-lookup"><span data-stu-id="6bfe1-155">deployableContentDisplayName</span></span>|<span data-ttu-id="6bfe1-156">String</span><span class="sxs-lookup"><span data-stu-id="6bfe1-156">String</span></span>|<span data-ttu-id="6bfe1-157">Удобное отображаемое имя развернутого контента профиля обновления качества</span><span class="sxs-lookup"><span data-stu-id="6bfe1-157">Friendly display name of the quality update profile deployable content</span></span>|
|<span data-ttu-id="6bfe1-158">endOfSupportDate</span><span class="sxs-lookup"><span data-stu-id="6bfe1-158">endOfSupportDate</span></span>|<span data-ttu-id="6bfe1-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bfe1-159">DateTimeOffset</span></span>|<span data-ttu-id="6bfe1-160">Последняя поддерживаемая дата обновления функций</span><span class="sxs-lookup"><span data-stu-id="6bfe1-160">The last supported date for a feature update</span></span>|



## <a name="response"></a><span data-ttu-id="6bfe1-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bfe1-161">Response</span></span>
<span data-ttu-id="6bfe1-162">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-162">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bfe1-163">Пример</span><span class="sxs-lookup"><span data-stu-id="6bfe1-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="6bfe1-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bfe1-164">Request</span></span>
<span data-ttu-id="6bfe1-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles
Content-type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "deployableContentDisplayName": "Deployable Content Display Name value",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00"
}
```

### <a name="response"></a><span data-ttu-id="6bfe1-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bfe1-166">Response</span></span>
<span data-ttu-id="6bfe1-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6bfe1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 577

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
  ],
  "deployableContentDisplayName": "Deployable Content Display Name value",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00"
}
```




