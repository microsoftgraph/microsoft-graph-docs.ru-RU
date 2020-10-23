---
title: Создание Андроиддевицеовнеренроллментпрофиле
description: Создание нового объекта Андроиддевицеовнеренроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 80a6399df5133ac7dfe23cb7b7ffe26746bc6fda
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701328"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="2b7da-103">Создание Андроиддевицеовнеренроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="2b7da-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

<span data-ttu-id="2b7da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b7da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b7da-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b7da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b7da-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b7da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b7da-107">Создание нового объекта [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2b7da-107">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b7da-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2b7da-108">Prerequisites</span></span>
<span data-ttu-id="2b7da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b7da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b7da-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b7da-111">Permission type</span></span>|<span data-ttu-id="2b7da-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b7da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b7da-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b7da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b7da-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b7da-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2b7da-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b7da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b7da-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b7da-116">Not supported.</span></span>|
|<span data-ttu-id="2b7da-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b7da-117">Application</span></span>|<span data-ttu-id="2b7da-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b7da-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b7da-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b7da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="2b7da-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2b7da-120">Request headers</span></span>
|<span data-ttu-id="2b7da-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b7da-121">Header</span></span>|<span data-ttu-id="2b7da-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2b7da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b7da-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b7da-123">Authorization</span></span>|<span data-ttu-id="2b7da-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b7da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b7da-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b7da-125">Accept</span></span>|<span data-ttu-id="2b7da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b7da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b7da-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2b7da-127">Request body</span></span>
<span data-ttu-id="2b7da-128">В тексте запроса добавьте представление объекта Андроиддевицеовнеренроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b7da-128">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="2b7da-129">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнеренроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="2b7da-129">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="2b7da-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b7da-130">Property</span></span>|<span data-ttu-id="2b7da-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2b7da-131">Type</span></span>|<span data-ttu-id="2b7da-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2b7da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b7da-133">accountId</span><span class="sxs-lookup"><span data-stu-id="2b7da-133">accountId</span></span>|<span data-ttu-id="2b7da-134">String</span><span class="sxs-lookup"><span data-stu-id="2b7da-134">String</span></span>|<span data-ttu-id="2b7da-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="2b7da-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="2b7da-136">id</span><span class="sxs-lookup"><span data-stu-id="2b7da-136">id</span></span>|<span data-ttu-id="2b7da-137">Строка</span><span class="sxs-lookup"><span data-stu-id="2b7da-137">String</span></span>|<span data-ttu-id="2b7da-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="2b7da-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="2b7da-139">displayName</span><span class="sxs-lookup"><span data-stu-id="2b7da-139">displayName</span></span>|<span data-ttu-id="2b7da-140">Строка</span><span class="sxs-lookup"><span data-stu-id="2b7da-140">String</span></span>|<span data-ttu-id="2b7da-141">Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="2b7da-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="2b7da-142">description</span><span class="sxs-lookup"><span data-stu-id="2b7da-142">description</span></span>|<span data-ttu-id="2b7da-143">Строка</span><span class="sxs-lookup"><span data-stu-id="2b7da-143">String</span></span>|<span data-ttu-id="2b7da-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="2b7da-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="2b7da-145">енроллментмоде</span><span class="sxs-lookup"><span data-stu-id="2b7da-145">enrollmentMode</span></span>|[<span data-ttu-id="2b7da-146">androidDeviceOwnerEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="2b7da-146">androidDeviceOwnerEnrollmentMode</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentmode.md)|<span data-ttu-id="2b7da-147">Режим регистрации устройств, использующих этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="2b7da-147">The enrollment mode of devices that use this enrollment profile.</span></span> <span data-ttu-id="2b7da-148">Возможные значения: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="2b7da-148">Possible values are: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`.</span></span>|
|<span data-ttu-id="2b7da-149">енроллменттокентипе</span><span class="sxs-lookup"><span data-stu-id="2b7da-149">enrollmentTokenType</span></span>|[<span data-ttu-id="2b7da-150">андроиддевицеовнеренроллменттокентипе</span><span class="sxs-lookup"><span data-stu-id="2b7da-150">androidDeviceOwnerEnrollmentTokenType</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmenttokentype.md)|<span data-ttu-id="2b7da-151">Тип маркера регистрации для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="2b7da-151">The enrollment token type for an enrollment profile.</span></span> <span data-ttu-id="2b7da-152">Возможные значения: `default`, `corporateOwnedDedicatedDeviceWithAzureADSharedMode`.</span><span class="sxs-lookup"><span data-stu-id="2b7da-152">Possible values are: `default`, `corporateOwnedDedicatedDeviceWithAzureADSharedMode`.</span></span>|
|<span data-ttu-id="2b7da-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b7da-153">createdDateTime</span></span>|<span data-ttu-id="2b7da-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b7da-154">DateTimeOffset</span></span>|<span data-ttu-id="2b7da-155">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="2b7da-155">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="2b7da-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b7da-156">lastModifiedDateTime</span></span>|<span data-ttu-id="2b7da-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b7da-157">DateTimeOffset</span></span>|<span data-ttu-id="2b7da-158">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="2b7da-158">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="2b7da-159">tokenValue</span><span class="sxs-lookup"><span data-stu-id="2b7da-159">tokenValue</span></span>|<span data-ttu-id="2b7da-160">String</span><span class="sxs-lookup"><span data-stu-id="2b7da-160">String</span></span>|<span data-ttu-id="2b7da-161">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="2b7da-161">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="2b7da-162">токенкреатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="2b7da-162">tokenCreationDateTime</span></span>|<span data-ttu-id="2b7da-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b7da-163">DateTimeOffset</span></span>|<span data-ttu-id="2b7da-164">Дата и время создания последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="2b7da-164">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="2b7da-165">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2b7da-165">tokenExpirationDateTime</span></span>|<span data-ttu-id="2b7da-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b7da-166">DateTimeOffset</span></span>|<span data-ttu-id="2b7da-167">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="2b7da-167">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="2b7da-168">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2b7da-168">enrolledDeviceCount</span></span>|<span data-ttu-id="2b7da-169">Int32</span><span class="sxs-lookup"><span data-stu-id="2b7da-169">Int32</span></span>|<span data-ttu-id="2b7da-170">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="2b7da-170">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="2b7da-171">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="2b7da-171">qrCodeContent</span></span>|<span data-ttu-id="2b7da-172">String</span><span class="sxs-lookup"><span data-stu-id="2b7da-172">String</span></span>|<span data-ttu-id="2b7da-173">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="2b7da-173">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="2b7da-174">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="2b7da-174">qrCodeImage</span></span>|[<span data-ttu-id="2b7da-175">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2b7da-175">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2b7da-176">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="2b7da-176">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="2b7da-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2b7da-177">roleScopeTagIds</span></span>|<span data-ttu-id="2b7da-178">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2b7da-178">String collection</span></span>|<span data-ttu-id="2b7da-179">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2b7da-179">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="2b7da-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b7da-180">Response</span></span>
<span data-ttu-id="2b7da-181">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b7da-181">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b7da-182">Пример</span><span class="sxs-lookup"><span data-stu-id="2b7da-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b7da-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b7da-183">Request</span></span>
<span data-ttu-id="2b7da-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b7da-184">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="2b7da-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b7da-185">Response</span></span>
<span data-ttu-id="2b7da-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b7da-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





