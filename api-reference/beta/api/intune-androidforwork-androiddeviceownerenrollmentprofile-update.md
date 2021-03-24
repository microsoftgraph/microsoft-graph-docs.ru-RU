---
title: Обновление androidDeviceOwnerEnrollmentProfile
description: Обновление свойств объекта androidDeviceOwnerEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dbf3a50d08e8f211c14f0d8eab8070e310f560c9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144797"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="16407-103">Обновление androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="16407-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

<span data-ttu-id="16407-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16407-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16407-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16407-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16407-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16407-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16407-107">Обновление свойств объекта [androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="16407-107">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16407-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="16407-108">Prerequisites</span></span>
<span data-ttu-id="16407-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16407-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16407-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16407-111">Permission type</span></span>|<span data-ttu-id="16407-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16407-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16407-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16407-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16407-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16407-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16407-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16407-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16407-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16407-116">Not supported.</span></span>|
|<span data-ttu-id="16407-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="16407-117">Application</span></span>|<span data-ttu-id="16407-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16407-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16407-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16407-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="16407-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="16407-120">Request headers</span></span>
|<span data-ttu-id="16407-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16407-121">Header</span></span>|<span data-ttu-id="16407-122">Значение</span><span class="sxs-lookup"><span data-stu-id="16407-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16407-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16407-123">Authorization</span></span>|<span data-ttu-id="16407-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16407-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16407-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16407-125">Accept</span></span>|<span data-ttu-id="16407-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16407-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16407-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16407-127">Request body</span></span>
<span data-ttu-id="16407-128">В теле запроса поставляем представление JSON для [объекта AndroidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="16407-128">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="16407-129">В следующей таблице показаны свойства, необходимые при создании [androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="16407-129">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="16407-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="16407-130">Property</span></span>|<span data-ttu-id="16407-131">Тип</span><span class="sxs-lookup"><span data-stu-id="16407-131">Type</span></span>|<span data-ttu-id="16407-132">Описание</span><span class="sxs-lookup"><span data-stu-id="16407-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16407-133">accountId</span><span class="sxs-lookup"><span data-stu-id="16407-133">accountId</span></span>|<span data-ttu-id="16407-134">String</span><span class="sxs-lookup"><span data-stu-id="16407-134">String</span></span>|<span data-ttu-id="16407-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="16407-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="16407-136">id</span><span class="sxs-lookup"><span data-stu-id="16407-136">id</span></span>|<span data-ttu-id="16407-137">Строка</span><span class="sxs-lookup"><span data-stu-id="16407-137">String</span></span>|<span data-ttu-id="16407-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="16407-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="16407-139">displayName</span><span class="sxs-lookup"><span data-stu-id="16407-139">displayName</span></span>|<span data-ttu-id="16407-140">Строка</span><span class="sxs-lookup"><span data-stu-id="16407-140">String</span></span>|<span data-ttu-id="16407-141">Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="16407-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="16407-142">description</span><span class="sxs-lookup"><span data-stu-id="16407-142">description</span></span>|<span data-ttu-id="16407-143">Строка</span><span class="sxs-lookup"><span data-stu-id="16407-143">String</span></span>|<span data-ttu-id="16407-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="16407-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="16407-145">enrollmentMode</span><span class="sxs-lookup"><span data-stu-id="16407-145">enrollmentMode</span></span>|[<span data-ttu-id="16407-146">androidDeviceOwnerEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="16407-146">androidDeviceOwnerEnrollmentMode</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentmode.md)|<span data-ttu-id="16407-147">Режим регистрации устройств, которые используют этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="16407-147">The enrollment mode of devices that use this enrollment profile.</span></span> <span data-ttu-id="16407-148">Возможные значения: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="16407-148">Possible values are: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`.</span></span>|
|<span data-ttu-id="16407-149">enrollmentTokenType</span><span class="sxs-lookup"><span data-stu-id="16407-149">enrollmentTokenType</span></span>|[<span data-ttu-id="16407-150">androidDeviceOwnerEnrollmentTokenType</span><span class="sxs-lookup"><span data-stu-id="16407-150">androidDeviceOwnerEnrollmentTokenType</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmenttokentype.md)|<span data-ttu-id="16407-151">Тип маркера регистрации для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="16407-151">The enrollment token type for an enrollment profile.</span></span> <span data-ttu-id="16407-152">Возможные значения: `default`, `corporateOwnedDedicatedDeviceWithAzureADSharedMode`.</span><span class="sxs-lookup"><span data-stu-id="16407-152">Possible values are: `default`, `corporateOwnedDedicatedDeviceWithAzureADSharedMode`.</span></span>|
|<span data-ttu-id="16407-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16407-153">createdDateTime</span></span>|<span data-ttu-id="16407-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16407-154">DateTimeOffset</span></span>|<span data-ttu-id="16407-155">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="16407-155">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="16407-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16407-156">lastModifiedDateTime</span></span>|<span data-ttu-id="16407-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16407-157">DateTimeOffset</span></span>|<span data-ttu-id="16407-158">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="16407-158">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="16407-159">tokenValue</span><span class="sxs-lookup"><span data-stu-id="16407-159">tokenValue</span></span>|<span data-ttu-id="16407-160">String</span><span class="sxs-lookup"><span data-stu-id="16407-160">String</span></span>|<span data-ttu-id="16407-161">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="16407-161">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="16407-162">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="16407-162">tokenCreationDateTime</span></span>|<span data-ttu-id="16407-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16407-163">DateTimeOffset</span></span>|<span data-ttu-id="16407-164">Дата создания последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="16407-164">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="16407-165">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="16407-165">tokenExpirationDateTime</span></span>|<span data-ttu-id="16407-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16407-166">DateTimeOffset</span></span>|<span data-ttu-id="16407-167">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="16407-167">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="16407-168">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16407-168">enrolledDeviceCount</span></span>|<span data-ttu-id="16407-169">Int32</span><span class="sxs-lookup"><span data-stu-id="16407-169">Int32</span></span>|<span data-ttu-id="16407-170">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="16407-170">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="16407-171">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="16407-171">qrCodeContent</span></span>|<span data-ttu-id="16407-172">String</span><span class="sxs-lookup"><span data-stu-id="16407-172">String</span></span>|<span data-ttu-id="16407-173">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="16407-173">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="16407-174">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="16407-174">qrCodeImage</span></span>|[<span data-ttu-id="16407-175">mimeContent</span><span class="sxs-lookup"><span data-stu-id="16407-175">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="16407-176">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="16407-176">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="16407-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="16407-177">roleScopeTagIds</span></span>|<span data-ttu-id="16407-178">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="16407-178">String collection</span></span>|<span data-ttu-id="16407-179">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="16407-179">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="16407-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="16407-180">Response</span></span>
<span data-ttu-id="16407-181">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="16407-181">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16407-182">Пример</span><span class="sxs-lookup"><span data-stu-id="16407-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="16407-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="16407-183">Request</span></span>
<span data-ttu-id="16407-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16407-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16407-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="16407-185">Response</span></span>
<span data-ttu-id="16407-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16407-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




