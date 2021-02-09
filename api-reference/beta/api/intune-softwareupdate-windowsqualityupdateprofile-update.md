---
title: Обновление windowsQualityUpdateProfile
description: Обновление свойств объекта windowsQualityUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1733570906276f259f2f8fa4147df9b61e390a23
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160739"
---
# <a name="update-windowsqualityupdateprofile"></a><span data-ttu-id="1e11d-103">Обновление windowsQualityUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="1e11d-103">Update windowsQualityUpdateProfile</span></span>

<span data-ttu-id="1e11d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e11d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e11d-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e11d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e11d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1e11d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e11d-107">Обновление свойств объекта [windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1e11d-107">Update the properties of a [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e11d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1e11d-108">Prerequisites</span></span>
<span data-ttu-id="1e11d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e11d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e11d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e11d-111">Permission type</span></span>|<span data-ttu-id="1e11d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e11d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e11d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e11d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1e11d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e11d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1e11d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e11d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e11d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e11d-116">Not supported.</span></span>|
|<span data-ttu-id="1e11d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e11d-117">Application</span></span>|<span data-ttu-id="1e11d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e11d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e11d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e11d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="1e11d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1e11d-120">Request headers</span></span>
|<span data-ttu-id="1e11d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1e11d-121">Header</span></span>|<span data-ttu-id="1e11d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1e11d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e11d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1e11d-123">Authorization</span></span>|<span data-ttu-id="1e11d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e11d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e11d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1e11d-125">Accept</span></span>|<span data-ttu-id="1e11d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1e11d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e11d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1e11d-127">Request body</span></span>
<span data-ttu-id="1e11d-128">В теле запроса укажу представление объекта [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="1e11d-128">In the request body, supply a JSON representation for the [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object.</span></span>

<span data-ttu-id="1e11d-129">В следующей таблице показаны свойства, необходимые при создании [объекта windowsQualityUpdateProfile.](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1e11d-129">The following table shows the properties that are required when you create the [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md).</span></span>

|<span data-ttu-id="1e11d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e11d-130">Property</span></span>|<span data-ttu-id="1e11d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1e11d-131">Type</span></span>|<span data-ttu-id="1e11d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1e11d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e11d-133">id</span><span class="sxs-lookup"><span data-stu-id="1e11d-133">id</span></span>|<span data-ttu-id="1e11d-134">String</span><span class="sxs-lookup"><span data-stu-id="1e11d-134">String</span></span>|<span data-ttu-id="1e11d-135">ИД политики Intune.</span><span class="sxs-lookup"><span data-stu-id="1e11d-135">The Intune policy id.</span></span>|
|<span data-ttu-id="1e11d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1e11d-136">displayName</span></span>|<span data-ttu-id="1e11d-137">String</span><span class="sxs-lookup"><span data-stu-id="1e11d-137">String</span></span>|<span data-ttu-id="1e11d-138">Отображаемая имя профиля.</span><span class="sxs-lookup"><span data-stu-id="1e11d-138">The display name for the profile.</span></span>|
|<span data-ttu-id="1e11d-139">description</span><span class="sxs-lookup"><span data-stu-id="1e11d-139">description</span></span>|<span data-ttu-id="1e11d-140">String</span><span class="sxs-lookup"><span data-stu-id="1e11d-140">String</span></span>|<span data-ttu-id="1e11d-141">Описание профиля, указанного пользователем.</span><span class="sxs-lookup"><span data-stu-id="1e11d-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="1e11d-142">expeditedUpdateSettings</span><span class="sxs-lookup"><span data-stu-id="1e11d-142">expeditedUpdateSettings</span></span>|[<span data-ttu-id="1e11d-143">expeditedWindowsQualityUpdateSettings</span><span class="sxs-lookup"><span data-stu-id="1e11d-143">expeditedWindowsQualityUpdateSettings</span></span>](../resources/intune-softwareupdate-expeditedwindowsqualityupdatesettings.md)|<span data-ttu-id="1e11d-144">Параметры ускорения обновления.</span><span class="sxs-lookup"><span data-stu-id="1e11d-144">Expedited update settings.</span></span>|
|<span data-ttu-id="1e11d-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e11d-145">createdDateTime</span></span>|<span data-ttu-id="1e11d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e11d-146">DateTimeOffset</span></span>|<span data-ttu-id="1e11d-147">Дата создания профиля.</span><span class="sxs-lookup"><span data-stu-id="1e11d-147">The date time that the profile was created.</span></span>|
|<span data-ttu-id="1e11d-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e11d-148">lastModifiedDateTime</span></span>|<span data-ttu-id="1e11d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e11d-149">DateTimeOffset</span></span>|<span data-ttu-id="1e11d-150">Дата последнего изменения профиля.</span><span class="sxs-lookup"><span data-stu-id="1e11d-150">The date time that the profile was last modified.</span></span>|
|<span data-ttu-id="1e11d-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1e11d-151">roleScopeTagIds</span></span>|<span data-ttu-id="1e11d-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1e11d-152">String collection</span></span>|<span data-ttu-id="1e11d-153">Список тегов области для этого объекта обновления качества.</span><span class="sxs-lookup"><span data-stu-id="1e11d-153">List of Scope Tags for this Quality Update entity.</span></span>|



## <a name="response"></a><span data-ttu-id="1e11d-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e11d-154">Response</span></span>
<span data-ttu-id="1e11d-155">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1e11d-155">If successful, this method returns a `200 OK` response code and an updated [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e11d-156">Пример</span><span class="sxs-lookup"><span data-stu-id="1e11d-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e11d-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e11d-157">Request</span></span>
<span data-ttu-id="1e11d-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e11d-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}
Content-type: application/json
Content-length: 418

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="1e11d-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e11d-159">Response</span></span>
<span data-ttu-id="1e11d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e11d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

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
  ]
}
```




