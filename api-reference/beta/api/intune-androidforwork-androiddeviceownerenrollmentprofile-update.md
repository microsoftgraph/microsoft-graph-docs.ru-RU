---
title: Обновление Андроиддевицеовнеренроллментпрофиле
description: Обновление свойств объекта Андроиддевицеовнеренроллментпрофиле.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a387e4f0848afca4687cf6c71923cefa2d1b235e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815777"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="a9f5a-103">Обновление Андроиддевицеовнеренроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="a9f5a-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="a9f5a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9f5a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9f5a-106">Обновление свойств объекта [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a9f5a-106">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9f5a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a9f5a-107">Prerequisites</span></span>
<span data-ttu-id="a9f5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9f5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9f5a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9f5a-110">Permission type</span></span>|<span data-ttu-id="a9f5a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9f5a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9f5a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9f5a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a9f5a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9f5a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9f5a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9f5a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9f5a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-115">Not supported.</span></span>|
|<span data-ttu-id="a9f5a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a9f5a-116">Application</span></span>|<span data-ttu-id="a9f5a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9f5a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9f5a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9f5a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="a9f5a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a9f5a-119">Request headers</span></span>
|<span data-ttu-id="a9f5a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9f5a-120">Header</span></span>|<span data-ttu-id="a9f5a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a9f5a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9f5a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9f5a-122">Authorization</span></span>|<span data-ttu-id="a9f5a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9f5a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a9f5a-124">Accept</span></span>|<span data-ttu-id="a9f5a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a9f5a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9f5a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9f5a-126">Request body</span></span>
<span data-ttu-id="a9f5a-127">В тексте запроса добавьте представление объекта [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-127">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="a9f5a-128">В следующей таблице приведены свойства, необходимые при создании [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="a9f5a-128">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="a9f5a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9f5a-129">Property</span></span>|<span data-ttu-id="a9f5a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a9f5a-130">Type</span></span>|<span data-ttu-id="a9f5a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a9f5a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9f5a-132">accountId</span><span class="sxs-lookup"><span data-stu-id="a9f5a-132">accountId</span></span>|<span data-ttu-id="a9f5a-133">String</span><span class="sxs-lookup"><span data-stu-id="a9f5a-133">String</span></span>|<span data-ttu-id="a9f5a-134">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="a9f5a-135">id</span><span class="sxs-lookup"><span data-stu-id="a9f5a-135">id</span></span>|<span data-ttu-id="a9f5a-136">Строка</span><span class="sxs-lookup"><span data-stu-id="a9f5a-136">String</span></span>|<span data-ttu-id="a9f5a-137">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="a9f5a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="a9f5a-138">displayName</span></span>|<span data-ttu-id="a9f5a-139">Строка</span><span class="sxs-lookup"><span data-stu-id="a9f5a-139">String</span></span>|<span data-ttu-id="a9f5a-140">Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="a9f5a-141">description</span><span class="sxs-lookup"><span data-stu-id="a9f5a-141">description</span></span>|<span data-ttu-id="a9f5a-142">String</span><span class="sxs-lookup"><span data-stu-id="a9f5a-142">String</span></span>|<span data-ttu-id="a9f5a-143">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="a9f5a-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9f5a-144">createdDateTime</span></span>|<span data-ttu-id="a9f5a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9f5a-145">DateTimeOffset</span></span>|<span data-ttu-id="a9f5a-146">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="a9f5a-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9f5a-147">lastModifiedDateTime</span></span>|<span data-ttu-id="a9f5a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9f5a-148">DateTimeOffset</span></span>|<span data-ttu-id="a9f5a-149">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="a9f5a-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="a9f5a-150">tokenValue</span></span>|<span data-ttu-id="a9f5a-151">String</span><span class="sxs-lookup"><span data-stu-id="a9f5a-151">String</span></span>|<span data-ttu-id="a9f5a-152">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="a9f5a-153">токенкреатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="a9f5a-153">tokenCreationDateTime</span></span>|<span data-ttu-id="a9f5a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9f5a-154">DateTimeOffset</span></span>|<span data-ttu-id="a9f5a-155">Дата и время создания последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-155">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="a9f5a-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a9f5a-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="a9f5a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9f5a-157">DateTimeOffset</span></span>|<span data-ttu-id="a9f5a-158">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="a9f5a-159">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a9f5a-159">enrolledDeviceCount</span></span>|<span data-ttu-id="a9f5a-160">Int32</span><span class="sxs-lookup"><span data-stu-id="a9f5a-160">Int32</span></span>|<span data-ttu-id="a9f5a-161">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-161">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="a9f5a-162">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="a9f5a-162">qrCodeContent</span></span>|<span data-ttu-id="a9f5a-163">String</span><span class="sxs-lookup"><span data-stu-id="a9f5a-163">String</span></span>|<span data-ttu-id="a9f5a-164">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-164">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="a9f5a-165">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="a9f5a-165">qrCodeImage</span></span>|[<span data-ttu-id="a9f5a-166">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a9f5a-166">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a9f5a-167">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-167">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="a9f5a-168">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a9f5a-168">roleScopeTagIds</span></span>|<span data-ttu-id="a9f5a-169">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a9f5a-169">String collection</span></span>|<span data-ttu-id="a9f5a-170">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-170">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="a9f5a-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9f5a-171">Response</span></span>
<span data-ttu-id="a9f5a-172">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-172">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9f5a-173">Пример</span><span class="sxs-lookup"><span data-stu-id="a9f5a-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9f5a-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9f5a-174">Request</span></span>
<span data-ttu-id="a9f5a-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
Content-type: application/json
Content-length: 627

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="a9f5a-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9f5a-176">Response</span></span>
<span data-ttu-id="a9f5a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9f5a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 799

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
  "displayName": "Display Name value",
  "description": "Description value",
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




