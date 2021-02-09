---
title: Обновление androidDeviceOwnerEnrollmentProfile
description: Обновление свойств объекта androidDeviceOwnerEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7e0bf99c710ac8699127dca1988136376156dec2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156310"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="dc997-103">Обновление androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="dc997-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

<span data-ttu-id="dc997-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc997-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc997-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc997-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc997-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc997-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc997-107">Обновление свойств объекта [androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="dc997-107">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc997-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dc997-108">Prerequisites</span></span>
<span data-ttu-id="dc997-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc997-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc997-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc997-111">Permission type</span></span>|<span data-ttu-id="dc997-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc997-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc997-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc997-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc997-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc997-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dc997-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc997-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc997-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc997-116">Not supported.</span></span>|
|<span data-ttu-id="dc997-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc997-117">Application</span></span>|<span data-ttu-id="dc997-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc997-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc997-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc997-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="dc997-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dc997-120">Request headers</span></span>
|<span data-ttu-id="dc997-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc997-121">Header</span></span>|<span data-ttu-id="dc997-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dc997-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc997-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc997-123">Authorization</span></span>|<span data-ttu-id="dc997-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc997-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc997-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dc997-125">Accept</span></span>|<span data-ttu-id="dc997-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc997-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc997-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc997-127">Request body</span></span>
<span data-ttu-id="dc997-128">В теле запроса укажу представление объекта [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="dc997-128">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="dc997-129">В следующей таблице показаны свойства, необходимые при создании [объекта androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="dc997-129">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="dc997-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc997-130">Property</span></span>|<span data-ttu-id="dc997-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dc997-131">Type</span></span>|<span data-ttu-id="dc997-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dc997-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc997-133">accountId</span><span class="sxs-lookup"><span data-stu-id="dc997-133">accountId</span></span>|<span data-ttu-id="dc997-134">String</span><span class="sxs-lookup"><span data-stu-id="dc997-134">String</span></span>|<span data-ttu-id="dc997-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="dc997-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="dc997-136">id</span><span class="sxs-lookup"><span data-stu-id="dc997-136">id</span></span>|<span data-ttu-id="dc997-137">String</span><span class="sxs-lookup"><span data-stu-id="dc997-137">String</span></span>|<span data-ttu-id="dc997-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="dc997-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="dc997-139">displayName</span><span class="sxs-lookup"><span data-stu-id="dc997-139">displayName</span></span>|<span data-ttu-id="dc997-140">String</span><span class="sxs-lookup"><span data-stu-id="dc997-140">String</span></span>|<span data-ttu-id="dc997-141">Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="dc997-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="dc997-142">description</span><span class="sxs-lookup"><span data-stu-id="dc997-142">description</span></span>|<span data-ttu-id="dc997-143">String</span><span class="sxs-lookup"><span data-stu-id="dc997-143">String</span></span>|<span data-ttu-id="dc997-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="dc997-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="dc997-145">enrollmentMode</span><span class="sxs-lookup"><span data-stu-id="dc997-145">enrollmentMode</span></span>|[<span data-ttu-id="dc997-146">androidDeviceOwnerEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="dc997-146">androidDeviceOwnerEnrollmentMode</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentmode.md)|<span data-ttu-id="dc997-147">Режим регистрации устройств, которые используют этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="dc997-147">The enrollment mode of devices that use this enrollment profile.</span></span> <span data-ttu-id="dc997-148">Возможные значения: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="dc997-148">Possible values are: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`.</span></span>|
|<span data-ttu-id="dc997-149">enrollmentTokenType</span><span class="sxs-lookup"><span data-stu-id="dc997-149">enrollmentTokenType</span></span>|[<span data-ttu-id="dc997-150">androidDeviceOwnerEnrollmentTokenType</span><span class="sxs-lookup"><span data-stu-id="dc997-150">androidDeviceOwnerEnrollmentTokenType</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmenttokentype.md)|<span data-ttu-id="dc997-151">Тип маркера регистрации для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="dc997-151">The enrollment token type for an enrollment profile.</span></span> <span data-ttu-id="dc997-152">Возможные значения: `default`, `corporateOwnedDedicatedDeviceWithAzureADSharedMode`.</span><span class="sxs-lookup"><span data-stu-id="dc997-152">Possible values are: `default`, `corporateOwnedDedicatedDeviceWithAzureADSharedMode`.</span></span>|
|<span data-ttu-id="dc997-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dc997-153">createdDateTime</span></span>|<span data-ttu-id="dc997-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc997-154">DateTimeOffset</span></span>|<span data-ttu-id="dc997-155">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="dc997-155">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="dc997-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc997-156">lastModifiedDateTime</span></span>|<span data-ttu-id="dc997-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc997-157">DateTimeOffset</span></span>|<span data-ttu-id="dc997-158">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="dc997-158">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="dc997-159">tokenValue</span><span class="sxs-lookup"><span data-stu-id="dc997-159">tokenValue</span></span>|<span data-ttu-id="dc997-160">String</span><span class="sxs-lookup"><span data-stu-id="dc997-160">String</span></span>|<span data-ttu-id="dc997-161">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="dc997-161">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="dc997-162">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="dc997-162">tokenCreationDateTime</span></span>|<span data-ttu-id="dc997-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc997-163">DateTimeOffset</span></span>|<span data-ttu-id="dc997-164">Дата создания последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="dc997-164">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="dc997-165">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dc997-165">tokenExpirationDateTime</span></span>|<span data-ttu-id="dc997-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc997-166">DateTimeOffset</span></span>|<span data-ttu-id="dc997-167">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="dc997-167">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="dc997-168">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dc997-168">enrolledDeviceCount</span></span>|<span data-ttu-id="dc997-169">Int32</span><span class="sxs-lookup"><span data-stu-id="dc997-169">Int32</span></span>|<span data-ttu-id="dc997-170">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="dc997-170">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="dc997-171">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="dc997-171">qrCodeContent</span></span>|<span data-ttu-id="dc997-172">String</span><span class="sxs-lookup"><span data-stu-id="dc997-172">String</span></span>|<span data-ttu-id="dc997-173">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="dc997-173">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="dc997-174">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="dc997-174">qrCodeImage</span></span>|[<span data-ttu-id="dc997-175">mimeContent</span><span class="sxs-lookup"><span data-stu-id="dc997-175">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="dc997-176">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="dc997-176">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="dc997-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dc997-177">roleScopeTagIds</span></span>|<span data-ttu-id="dc997-178">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dc997-178">String collection</span></span>|<span data-ttu-id="dc997-179">Список тегов области для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="dc997-179">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="dc997-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc997-180">Response</span></span>
<span data-ttu-id="dc997-181">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dc997-181">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc997-182">Пример</span><span class="sxs-lookup"><span data-stu-id="dc997-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc997-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc997-183">Request</span></span>
<span data-ttu-id="dc997-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc997-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dc997-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc997-185">Response</span></span>
<span data-ttu-id="dc997-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc997-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




