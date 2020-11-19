---
title: Обновление Андроиддевицеовнеренроллментпрофиле
description: Обновление свойств объекта Андроиддевицеовнеренроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b4ebeb016f2085868149fcea3f3422617a4de4c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255113"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="b28c1-103">Обновление Андроиддевицеовнеренроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="b28c1-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

<span data-ttu-id="b28c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b28c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b28c1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b28c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b28c1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b28c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b28c1-107">Обновление свойств объекта [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b28c1-107">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b28c1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b28c1-108">Prerequisites</span></span>
<span data-ttu-id="b28c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b28c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b28c1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b28c1-111">Permission type</span></span>|<span data-ttu-id="b28c1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b28c1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b28c1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b28c1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b28c1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b28c1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b28c1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b28c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b28c1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b28c1-116">Not supported.</span></span>|
|<span data-ttu-id="b28c1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b28c1-117">Application</span></span>|<span data-ttu-id="b28c1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b28c1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b28c1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b28c1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="b28c1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b28c1-120">Request headers</span></span>
|<span data-ttu-id="b28c1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b28c1-121">Header</span></span>|<span data-ttu-id="b28c1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b28c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b28c1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b28c1-123">Authorization</span></span>|<span data-ttu-id="b28c1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b28c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b28c1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b28c1-125">Accept</span></span>|<span data-ttu-id="b28c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b28c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b28c1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b28c1-127">Request body</span></span>
<span data-ttu-id="b28c1-128">В тексте запроса добавьте представление объекта [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b28c1-128">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="b28c1-129">В следующей таблице приведены свойства, необходимые при создании [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="b28c1-129">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="b28c1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b28c1-130">Property</span></span>|<span data-ttu-id="b28c1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b28c1-131">Type</span></span>|<span data-ttu-id="b28c1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b28c1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b28c1-133">accountId</span><span class="sxs-lookup"><span data-stu-id="b28c1-133">accountId</span></span>|<span data-ttu-id="b28c1-134">String</span><span class="sxs-lookup"><span data-stu-id="b28c1-134">String</span></span>|<span data-ttu-id="b28c1-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="b28c1-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="b28c1-136">id</span><span class="sxs-lookup"><span data-stu-id="b28c1-136">id</span></span>|<span data-ttu-id="b28c1-137">String</span><span class="sxs-lookup"><span data-stu-id="b28c1-137">String</span></span>|<span data-ttu-id="b28c1-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="b28c1-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="b28c1-139">displayName</span><span class="sxs-lookup"><span data-stu-id="b28c1-139">displayName</span></span>|<span data-ttu-id="b28c1-140">String</span><span class="sxs-lookup"><span data-stu-id="b28c1-140">String</span></span>|<span data-ttu-id="b28c1-141">Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="b28c1-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="b28c1-142">description</span><span class="sxs-lookup"><span data-stu-id="b28c1-142">description</span></span>|<span data-ttu-id="b28c1-143">String</span><span class="sxs-lookup"><span data-stu-id="b28c1-143">String</span></span>|<span data-ttu-id="b28c1-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="b28c1-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="b28c1-145">енроллментмоде</span><span class="sxs-lookup"><span data-stu-id="b28c1-145">enrollmentMode</span></span>|[<span data-ttu-id="b28c1-146">androidDeviceOwnerEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="b28c1-146">androidDeviceOwnerEnrollmentMode</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentmode.md)|<span data-ttu-id="b28c1-147">Режим регистрации устройств, использующих этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="b28c1-147">The enrollment mode of devices that use this enrollment profile.</span></span> <span data-ttu-id="b28c1-148">Возможные значения: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`, `corporateOwnedAOSPUserlessDevice`.</span><span class="sxs-lookup"><span data-stu-id="b28c1-148">Possible values are: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`, `corporateOwnedAOSPUserlessDevice`.</span></span>|
|<span data-ttu-id="b28c1-149">енроллменттокентипе</span><span class="sxs-lookup"><span data-stu-id="b28c1-149">enrollmentTokenType</span></span>|[<span data-ttu-id="b28c1-150">androidDeviceOwnerEnrollmentTokenType</span><span class="sxs-lookup"><span data-stu-id="b28c1-150">androidDeviceOwnerEnrollmentTokenType</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmenttokentype.md)|<span data-ttu-id="b28c1-151">Тип маркера регистрации для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="b28c1-151">The enrollment token type for an enrollment profile.</span></span> <span data-ttu-id="b28c1-152">Возможные значения: `default`, `corporateOwnedDedicatedDeviceWithAzureADSharedMode`.</span><span class="sxs-lookup"><span data-stu-id="b28c1-152">Possible values are: `default`, `corporateOwnedDedicatedDeviceWithAzureADSharedMode`.</span></span>|
|<span data-ttu-id="b28c1-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b28c1-153">createdDateTime</span></span>|<span data-ttu-id="b28c1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b28c1-154">DateTimeOffset</span></span>|<span data-ttu-id="b28c1-155">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="b28c1-155">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="b28c1-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b28c1-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b28c1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b28c1-157">DateTimeOffset</span></span>|<span data-ttu-id="b28c1-158">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="b28c1-158">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="b28c1-159">tokenValue</span><span class="sxs-lookup"><span data-stu-id="b28c1-159">tokenValue</span></span>|<span data-ttu-id="b28c1-160">String</span><span class="sxs-lookup"><span data-stu-id="b28c1-160">String</span></span>|<span data-ttu-id="b28c1-161">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="b28c1-161">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="b28c1-162">токенкреатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="b28c1-162">tokenCreationDateTime</span></span>|<span data-ttu-id="b28c1-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b28c1-163">DateTimeOffset</span></span>|<span data-ttu-id="b28c1-164">Дата и время создания последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="b28c1-164">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="b28c1-165">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b28c1-165">tokenExpirationDateTime</span></span>|<span data-ttu-id="b28c1-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b28c1-166">DateTimeOffset</span></span>|<span data-ttu-id="b28c1-167">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="b28c1-167">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="b28c1-168">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b28c1-168">enrolledDeviceCount</span></span>|<span data-ttu-id="b28c1-169">Int32</span><span class="sxs-lookup"><span data-stu-id="b28c1-169">Int32</span></span>|<span data-ttu-id="b28c1-170">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="b28c1-170">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="b28c1-171">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="b28c1-171">qrCodeContent</span></span>|<span data-ttu-id="b28c1-172">String</span><span class="sxs-lookup"><span data-stu-id="b28c1-172">String</span></span>|<span data-ttu-id="b28c1-173">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="b28c1-173">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="b28c1-174">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="b28c1-174">qrCodeImage</span></span>|[<span data-ttu-id="b28c1-175">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b28c1-175">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b28c1-176">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="b28c1-176">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="b28c1-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b28c1-177">roleScopeTagIds</span></span>|<span data-ttu-id="b28c1-178">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b28c1-178">String collection</span></span>|<span data-ttu-id="b28c1-179">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b28c1-179">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="b28c1-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="b28c1-180">Response</span></span>
<span data-ttu-id="b28c1-181">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b28c1-181">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b28c1-182">Пример</span><span class="sxs-lookup"><span data-stu-id="b28c1-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="b28c1-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="b28c1-183">Request</span></span>
<span data-ttu-id="b28c1-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b28c1-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
Content-type: application/json
Content-length: 758

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "enrollmentMode": "corporateOwnedFullyManaged",
  "enrollmentTokenType": "corporateOwnedDedicatedDeviceWithAzureADSharedMode",
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

### <a name="response"></a><span data-ttu-id="b28c1-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="b28c1-185">Response</span></span>
<span data-ttu-id="b28c1-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b28c1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 930

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
  "displayName": "Display Name value",
  "description": "Description value",
  "enrollmentMode": "corporateOwnedFullyManaged",
  "enrollmentTokenType": "corporateOwnedDedicatedDeviceWithAzureADSharedMode",
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




