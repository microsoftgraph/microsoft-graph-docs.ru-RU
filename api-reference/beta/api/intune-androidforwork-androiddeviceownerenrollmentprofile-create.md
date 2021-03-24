---
title: Создание androidDeviceOwnerEnrollmentProfile
description: Создайте новый объект androidDeviceOwnerEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8edd0c3a50d32aa4fe07512886fcadb88d5e9d5e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144839"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="c4b5c-103">Создание androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c4b5c-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

<span data-ttu-id="c4b5c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4b5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4b5c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4b5c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4b5c-107">Создайте новый [объект androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c4b5c-107">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4b5c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c4b5c-108">Prerequisites</span></span>
<span data-ttu-id="c4b5c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4b5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4b5c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4b5c-111">Permission type</span></span>|<span data-ttu-id="c4b5c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4b5c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4b5c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4b5c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4b5c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4b5c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4b5c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4b5c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4b5c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-116">Not supported.</span></span>|
|<span data-ttu-id="c4b5c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c4b5c-117">Application</span></span>|<span data-ttu-id="c4b5c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4b5c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4b5c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4b5c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="c4b5c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c4b5c-120">Request headers</span></span>
|<span data-ttu-id="c4b5c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4b5c-121">Header</span></span>|<span data-ttu-id="c4b5c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c4b5c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4b5c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4b5c-123">Authorization</span></span>|<span data-ttu-id="c4b5c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4b5c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c4b5c-125">Accept</span></span>|<span data-ttu-id="c4b5c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4b5c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4b5c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4b5c-127">Request body</span></span>
<span data-ttu-id="c4b5c-128">В теле запроса поставляем представление JSON для объекта AndroidDeviceOwnerEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-128">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="c4b5c-129">В следующей таблице показаны свойства, необходимые при создании androidDeviceOwnerEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-129">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="c4b5c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4b5c-130">Property</span></span>|<span data-ttu-id="c4b5c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c4b5c-131">Type</span></span>|<span data-ttu-id="c4b5c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c4b5c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4b5c-133">accountId</span><span class="sxs-lookup"><span data-stu-id="c4b5c-133">accountId</span></span>|<span data-ttu-id="c4b5c-134">String</span><span class="sxs-lookup"><span data-stu-id="c4b5c-134">String</span></span>|<span data-ttu-id="c4b5c-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="c4b5c-136">id</span><span class="sxs-lookup"><span data-stu-id="c4b5c-136">id</span></span>|<span data-ttu-id="c4b5c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c4b5c-137">String</span></span>|<span data-ttu-id="c4b5c-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="c4b5c-139">displayName</span><span class="sxs-lookup"><span data-stu-id="c4b5c-139">displayName</span></span>|<span data-ttu-id="c4b5c-140">Строка</span><span class="sxs-lookup"><span data-stu-id="c4b5c-140">String</span></span>|<span data-ttu-id="c4b5c-141">Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="c4b5c-142">description</span><span class="sxs-lookup"><span data-stu-id="c4b5c-142">description</span></span>|<span data-ttu-id="c4b5c-143">Строка</span><span class="sxs-lookup"><span data-stu-id="c4b5c-143">String</span></span>|<span data-ttu-id="c4b5c-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="c4b5c-145">enrollmentMode</span><span class="sxs-lookup"><span data-stu-id="c4b5c-145">enrollmentMode</span></span>|[<span data-ttu-id="c4b5c-146">androidDeviceOwnerEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="c4b5c-146">androidDeviceOwnerEnrollmentMode</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentmode.md)|<span data-ttu-id="c4b5c-147">Режим регистрации устройств, которые используют этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-147">The enrollment mode of devices that use this enrollment profile.</span></span> <span data-ttu-id="c4b5c-148">Возможные значения: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-148">Possible values are: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`.</span></span>|
|<span data-ttu-id="c4b5c-149">enrollmentTokenType</span><span class="sxs-lookup"><span data-stu-id="c4b5c-149">enrollmentTokenType</span></span>|[<span data-ttu-id="c4b5c-150">androidDeviceOwnerEnrollmentTokenType</span><span class="sxs-lookup"><span data-stu-id="c4b5c-150">androidDeviceOwnerEnrollmentTokenType</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmenttokentype.md)|<span data-ttu-id="c4b5c-151">Тип маркера регистрации для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-151">The enrollment token type for an enrollment profile.</span></span> <span data-ttu-id="c4b5c-152">Возможные значения: `default`, `corporateOwnedDedicatedDeviceWithAzureADSharedMode`.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-152">Possible values are: `default`, `corporateOwnedDedicatedDeviceWithAzureADSharedMode`.</span></span>|
|<span data-ttu-id="c4b5c-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4b5c-153">createdDateTime</span></span>|<span data-ttu-id="c4b5c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4b5c-154">DateTimeOffset</span></span>|<span data-ttu-id="c4b5c-155">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-155">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="c4b5c-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4b5c-156">lastModifiedDateTime</span></span>|<span data-ttu-id="c4b5c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4b5c-157">DateTimeOffset</span></span>|<span data-ttu-id="c4b5c-158">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-158">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="c4b5c-159">tokenValue</span><span class="sxs-lookup"><span data-stu-id="c4b5c-159">tokenValue</span></span>|<span data-ttu-id="c4b5c-160">String</span><span class="sxs-lookup"><span data-stu-id="c4b5c-160">String</span></span>|<span data-ttu-id="c4b5c-161">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-161">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="c4b5c-162">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="c4b5c-162">tokenCreationDateTime</span></span>|<span data-ttu-id="c4b5c-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4b5c-163">DateTimeOffset</span></span>|<span data-ttu-id="c4b5c-164">Дата создания последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-164">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="c4b5c-165">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c4b5c-165">tokenExpirationDateTime</span></span>|<span data-ttu-id="c4b5c-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4b5c-166">DateTimeOffset</span></span>|<span data-ttu-id="c4b5c-167">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-167">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="c4b5c-168">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c4b5c-168">enrolledDeviceCount</span></span>|<span data-ttu-id="c4b5c-169">Int32</span><span class="sxs-lookup"><span data-stu-id="c4b5c-169">Int32</span></span>|<span data-ttu-id="c4b5c-170">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-170">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="c4b5c-171">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="c4b5c-171">qrCodeContent</span></span>|<span data-ttu-id="c4b5c-172">String</span><span class="sxs-lookup"><span data-stu-id="c4b5c-172">String</span></span>|<span data-ttu-id="c4b5c-173">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-173">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="c4b5c-174">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="c4b5c-174">qrCodeImage</span></span>|[<span data-ttu-id="c4b5c-175">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c4b5c-175">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c4b5c-176">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-176">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="c4b5c-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c4b5c-177">roleScopeTagIds</span></span>|<span data-ttu-id="c4b5c-178">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c4b5c-178">String collection</span></span>|<span data-ttu-id="c4b5c-179">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-179">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="c4b5c-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4b5c-180">Response</span></span>
<span data-ttu-id="c4b5c-181">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-181">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4b5c-182">Пример</span><span class="sxs-lookup"><span data-stu-id="c4b5c-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4b5c-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4b5c-183">Request</span></span>
<span data-ttu-id="c4b5c-184">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c4b5c-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4b5c-185">Response</span></span>
<span data-ttu-id="c4b5c-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4b5c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




