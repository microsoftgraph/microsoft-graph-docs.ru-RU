---
title: Обновление windowsQualityUpdateProfile
description: Обновление свойств объекта windowsQualityUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 62932ae10bc64ecf63ece2648527d7babad8731e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156179"
---
# <a name="update-windowsqualityupdateprofile"></a><span data-ttu-id="c4488-103">Обновление windowsQualityUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="c4488-103">Update windowsQualityUpdateProfile</span></span>

<span data-ttu-id="c4488-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4488-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4488-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4488-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4488-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4488-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4488-107">Обновление свойств объекта [windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c4488-107">Update the properties of a [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4488-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c4488-108">Prerequisites</span></span>
<span data-ttu-id="c4488-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4488-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4488-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4488-111">Permission type</span></span>|<span data-ttu-id="c4488-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4488-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4488-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4488-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4488-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4488-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4488-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4488-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4488-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4488-116">Not supported.</span></span>|
|<span data-ttu-id="c4488-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c4488-117">Application</span></span>|<span data-ttu-id="c4488-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4488-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4488-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4488-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="c4488-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c4488-120">Request headers</span></span>
|<span data-ttu-id="c4488-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4488-121">Header</span></span>|<span data-ttu-id="c4488-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c4488-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4488-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4488-123">Authorization</span></span>|<span data-ttu-id="c4488-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4488-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4488-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c4488-125">Accept</span></span>|<span data-ttu-id="c4488-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4488-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4488-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4488-127">Request body</span></span>
<span data-ttu-id="c4488-128">В теле запроса поставляем представление JSON для [объекта WindowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c4488-128">In the request body, supply a JSON representation for the [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object.</span></span>

<span data-ttu-id="c4488-129">В следующей таблице показаны свойства, необходимые при создании [windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c4488-129">The following table shows the properties that are required when you create the [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md).</span></span>

|<span data-ttu-id="c4488-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4488-130">Property</span></span>|<span data-ttu-id="c4488-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c4488-131">Type</span></span>|<span data-ttu-id="c4488-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c4488-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4488-133">id</span><span class="sxs-lookup"><span data-stu-id="c4488-133">id</span></span>|<span data-ttu-id="c4488-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c4488-134">String</span></span>|<span data-ttu-id="c4488-135">ID политики Intune.</span><span class="sxs-lookup"><span data-stu-id="c4488-135">The Intune policy id.</span></span>|
|<span data-ttu-id="c4488-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c4488-136">displayName</span></span>|<span data-ttu-id="c4488-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c4488-137">String</span></span>|<span data-ttu-id="c4488-138">Имя отображения для профиля.</span><span class="sxs-lookup"><span data-stu-id="c4488-138">The display name for the profile.</span></span>|
|<span data-ttu-id="c4488-139">description</span><span class="sxs-lookup"><span data-stu-id="c4488-139">description</span></span>|<span data-ttu-id="c4488-140">Строка</span><span class="sxs-lookup"><span data-stu-id="c4488-140">String</span></span>|<span data-ttu-id="c4488-141">Описание профиля, указанного пользователем.</span><span class="sxs-lookup"><span data-stu-id="c4488-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="c4488-142">expeditedUpdateSettings</span><span class="sxs-lookup"><span data-stu-id="c4488-142">expeditedUpdateSettings</span></span>|[<span data-ttu-id="c4488-143">expeditedWindowsQualityUpdateSettings</span><span class="sxs-lookup"><span data-stu-id="c4488-143">expeditedWindowsQualityUpdateSettings</span></span>](../resources/intune-softwareupdate-expeditedwindowsqualityupdatesettings.md)|<span data-ttu-id="c4488-144">Параметры ускоренного обновления.</span><span class="sxs-lookup"><span data-stu-id="c4488-144">Expedited update settings.</span></span>|
|<span data-ttu-id="c4488-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4488-145">createdDateTime</span></span>|<span data-ttu-id="c4488-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4488-146">DateTimeOffset</span></span>|<span data-ttu-id="c4488-147">Время создания профиля.</span><span class="sxs-lookup"><span data-stu-id="c4488-147">The date time that the profile was created.</span></span>|
|<span data-ttu-id="c4488-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4488-148">lastModifiedDateTime</span></span>|<span data-ttu-id="c4488-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4488-149">DateTimeOffset</span></span>|<span data-ttu-id="c4488-150">Дата последнего изменения профиля.</span><span class="sxs-lookup"><span data-stu-id="c4488-150">The date time that the profile was last modified.</span></span>|
|<span data-ttu-id="c4488-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c4488-151">roleScopeTagIds</span></span>|<span data-ttu-id="c4488-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c4488-152">String collection</span></span>|<span data-ttu-id="c4488-153">Список тегов области для этого объекта обновления качества.</span><span class="sxs-lookup"><span data-stu-id="c4488-153">List of Scope Tags for this Quality Update entity.</span></span>|
|<span data-ttu-id="c4488-154">releaseDateDisplayName</span><span class="sxs-lookup"><span data-stu-id="c4488-154">releaseDateDisplayName</span></span>|<span data-ttu-id="c4488-155">Строка</span><span class="sxs-lookup"><span data-stu-id="c4488-155">String</span></span>|<span data-ttu-id="c4488-156">Содружественная дата выпуска для отображения для выпуска обновления качества</span><span class="sxs-lookup"><span data-stu-id="c4488-156">Friendly release date to display for a Quality Update release</span></span>|
|<span data-ttu-id="c4488-157">deployableContentDisplayName</span><span class="sxs-lookup"><span data-stu-id="c4488-157">deployableContentDisplayName</span></span>|<span data-ttu-id="c4488-158">Строка</span><span class="sxs-lookup"><span data-stu-id="c4488-158">String</span></span>|<span data-ttu-id="c4488-159">Удобное отображаемое имя развернутого контента профиля обновления качества</span><span class="sxs-lookup"><span data-stu-id="c4488-159">Friendly display name of the quality update profile deployable content</span></span>|



## <a name="response"></a><span data-ttu-id="c4488-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4488-160">Response</span></span>
<span data-ttu-id="c4488-161">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c4488-161">If successful, this method returns a `200 OK` response code and an updated [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4488-162">Пример</span><span class="sxs-lookup"><span data-stu-id="c4488-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4488-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4488-163">Request</span></span>
<span data-ttu-id="c4488-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4488-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}
Content-type: application/json
Content-length: 558

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "expeditedUpdateSettings": {
    "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings",
    "qualityUpdateRelease": "Quality Update Release value",
    "daysUntilForcedReboot": 5
  },
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "releaseDateDisplayName": "Release Date Display Name value",
  "deployableContentDisplayName": "Deployable Content Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="c4488-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4488-165">Response</span></span>
<span data-ttu-id="c4488-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4488-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 730

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfile",
  "id": "76fc7b65-7b65-76fc-657b-fc76657bfc76",
  "displayName": "Display Name value",
  "description": "Description value",
  "expeditedUpdateSettings": {
    "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings",
    "qualityUpdateRelease": "Quality Update Release value",
    "daysUntilForcedReboot": 5
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "releaseDateDisplayName": "Release Date Display Name value",
  "deployableContentDisplayName": "Deployable Content Display Name value"
}
```




