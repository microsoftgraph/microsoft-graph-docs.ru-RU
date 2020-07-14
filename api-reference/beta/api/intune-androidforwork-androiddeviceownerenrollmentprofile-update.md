---
title: Обновление Андроиддевицеовнеренроллментпрофиле
description: Обновление свойств объекта Андроиддевицеовнеренроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 41703511ef452849cb1073daa28da29b4212f3cf
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123556"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="e8b8a-103">Обновление Андроиддевицеовнеренроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="e8b8a-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

<span data-ttu-id="e8b8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8b8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8b8a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8b8a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8b8a-107">Обновление свойств объекта [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e8b8a-107">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8b8a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e8b8a-108">Prerequisites</span></span>
<span data-ttu-id="e8b8a-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e8b8a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8b8a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8b8a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8b8a-111">Permission type</span></span>|<span data-ttu-id="e8b8a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8b8a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8b8a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8b8a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8b8a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8b8a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8b8a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8b8a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8b8a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-116">Not supported.</span></span>|
|<span data-ttu-id="e8b8a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8b8a-117">Application</span></span>|<span data-ttu-id="e8b8a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8b8a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8b8a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8b8a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="e8b8a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e8b8a-120">Request headers</span></span>
|<span data-ttu-id="e8b8a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8b8a-121">Header</span></span>|<span data-ttu-id="e8b8a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e8b8a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8b8a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8b8a-123">Authorization</span></span>|<span data-ttu-id="e8b8a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8b8a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e8b8a-125">Accept</span></span>|<span data-ttu-id="e8b8a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8b8a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8b8a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8b8a-127">Request body</span></span>
<span data-ttu-id="e8b8a-128">В тексте запроса добавьте представление объекта [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-128">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="e8b8a-129">В следующей таблице приведены свойства, необходимые при создании [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e8b8a-129">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="e8b8a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8b8a-130">Property</span></span>|<span data-ttu-id="e8b8a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e8b8a-131">Type</span></span>|<span data-ttu-id="e8b8a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e8b8a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8b8a-133">accountId</span><span class="sxs-lookup"><span data-stu-id="e8b8a-133">accountId</span></span>|<span data-ttu-id="e8b8a-134">String</span><span class="sxs-lookup"><span data-stu-id="e8b8a-134">String</span></span>|<span data-ttu-id="e8b8a-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="e8b8a-136">id</span><span class="sxs-lookup"><span data-stu-id="e8b8a-136">id</span></span>|<span data-ttu-id="e8b8a-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e8b8a-137">String</span></span>|<span data-ttu-id="e8b8a-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="e8b8a-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e8b8a-139">displayName</span></span>|<span data-ttu-id="e8b8a-140">Строка</span><span class="sxs-lookup"><span data-stu-id="e8b8a-140">String</span></span>|<span data-ttu-id="e8b8a-141">Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="e8b8a-142">description</span><span class="sxs-lookup"><span data-stu-id="e8b8a-142">description</span></span>|<span data-ttu-id="e8b8a-143">String</span><span class="sxs-lookup"><span data-stu-id="e8b8a-143">String</span></span>|<span data-ttu-id="e8b8a-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="e8b8a-145">енроллментмоде</span><span class="sxs-lookup"><span data-stu-id="e8b8a-145">enrollmentMode</span></span>|[<span data-ttu-id="e8b8a-146">андроиддевицеовнеренроллментмоде</span><span class="sxs-lookup"><span data-stu-id="e8b8a-146">androidDeviceOwnerEnrollmentMode</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentmode.md)|<span data-ttu-id="e8b8a-147">Режим регистрации устройств, использующих этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-147">The enrollment mode of devices that use this enrollment profile.</span></span> <span data-ttu-id="e8b8a-148">Возможные значения: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-148">Possible values are: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`.</span></span>|
|<span data-ttu-id="e8b8a-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8b8a-149">createdDateTime</span></span>|<span data-ttu-id="e8b8a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8b8a-150">DateTimeOffset</span></span>|<span data-ttu-id="e8b8a-151">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-151">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="e8b8a-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8b8a-152">lastModifiedDateTime</span></span>|<span data-ttu-id="e8b8a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8b8a-153">DateTimeOffset</span></span>|<span data-ttu-id="e8b8a-154">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-154">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="e8b8a-155">tokenValue</span><span class="sxs-lookup"><span data-stu-id="e8b8a-155">tokenValue</span></span>|<span data-ttu-id="e8b8a-156">String</span><span class="sxs-lookup"><span data-stu-id="e8b8a-156">String</span></span>|<span data-ttu-id="e8b8a-157">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-157">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="e8b8a-158">токенкреатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="e8b8a-158">tokenCreationDateTime</span></span>|<span data-ttu-id="e8b8a-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8b8a-159">DateTimeOffset</span></span>|<span data-ttu-id="e8b8a-160">Дата и время создания последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-160">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="e8b8a-161">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e8b8a-161">tokenExpirationDateTime</span></span>|<span data-ttu-id="e8b8a-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8b8a-162">DateTimeOffset</span></span>|<span data-ttu-id="e8b8a-163">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-163">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="e8b8a-164">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e8b8a-164">enrolledDeviceCount</span></span>|<span data-ttu-id="e8b8a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e8b8a-165">Int32</span></span>|<span data-ttu-id="e8b8a-166">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-166">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="e8b8a-167">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="e8b8a-167">qrCodeContent</span></span>|<span data-ttu-id="e8b8a-168">String</span><span class="sxs-lookup"><span data-stu-id="e8b8a-168">String</span></span>|<span data-ttu-id="e8b8a-169">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-169">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="e8b8a-170">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="e8b8a-170">qrCodeImage</span></span>|[<span data-ttu-id="e8b8a-171">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e8b8a-171">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e8b8a-172">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-172">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="e8b8a-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e8b8a-173">roleScopeTagIds</span></span>|<span data-ttu-id="e8b8a-174">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e8b8a-174">String collection</span></span>|<span data-ttu-id="e8b8a-175">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-175">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="e8b8a-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8b8a-176">Response</span></span>
<span data-ttu-id="e8b8a-177">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-177">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8b8a-178">Пример</span><span class="sxs-lookup"><span data-stu-id="e8b8a-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8b8a-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8b8a-179">Request</span></span>
<span data-ttu-id="e8b8a-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
Content-type: application/json
Content-length: 678

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "enrollmentMode": "corporateOwnedFullyManaged",
  "tokenValue": "Token Value value",
  "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="e8b8a-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8b8a-181">Response</span></span>
<span data-ttu-id="e8b8a-182">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-182">Here is an example of the response.</span></span> <span data-ttu-id="e8b8a-183">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-183">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e8b8a-184">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e8b8a-184">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 850

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
  "displayName": "Display Name value",
  "description": "Description value",
  "enrollmentMode": "corporateOwnedFullyManaged",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```



