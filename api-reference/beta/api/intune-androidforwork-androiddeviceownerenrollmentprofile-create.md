---
title: Создание Андроиддевицеовнеренроллментпрофиле
description: Создание нового объекта Андроиддевицеовнеренроллментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2dfb96d29de65fd36bdc3d4ac782f1627d5f8437
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446312"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="23f73-103">Создание Андроиддевицеовнеренроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="23f73-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

<span data-ttu-id="23f73-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="23f73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23f73-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23f73-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23f73-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23f73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23f73-107">Создание нового объекта [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="23f73-107">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23f73-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="23f73-108">Prerequisites</span></span>
<span data-ttu-id="23f73-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23f73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23f73-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23f73-111">Permission type</span></span>|<span data-ttu-id="23f73-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="23f73-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23f73-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23f73-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23f73-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23f73-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23f73-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23f73-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23f73-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23f73-116">Not supported.</span></span>|
|<span data-ttu-id="23f73-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23f73-117">Application</span></span>|<span data-ttu-id="23f73-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23f73-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23f73-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23f73-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="23f73-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="23f73-120">Request headers</span></span>
|<span data-ttu-id="23f73-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23f73-121">Header</span></span>|<span data-ttu-id="23f73-122">Значение</span><span class="sxs-lookup"><span data-stu-id="23f73-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23f73-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23f73-123">Authorization</span></span>|<span data-ttu-id="23f73-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23f73-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23f73-125">Accept</span><span class="sxs-lookup"><span data-stu-id="23f73-125">Accept</span></span>|<span data-ttu-id="23f73-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23f73-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23f73-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23f73-127">Request body</span></span>
<span data-ttu-id="23f73-128">В тексте запроса добавьте представление объекта Андроиддевицеовнеренроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23f73-128">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="23f73-129">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнеренроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="23f73-129">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="23f73-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="23f73-130">Property</span></span>|<span data-ttu-id="23f73-131">Тип</span><span class="sxs-lookup"><span data-stu-id="23f73-131">Type</span></span>|<span data-ttu-id="23f73-132">Описание</span><span class="sxs-lookup"><span data-stu-id="23f73-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23f73-133">accountId</span><span class="sxs-lookup"><span data-stu-id="23f73-133">accountId</span></span>|<span data-ttu-id="23f73-134">String</span><span class="sxs-lookup"><span data-stu-id="23f73-134">String</span></span>|<span data-ttu-id="23f73-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="23f73-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="23f73-136">id</span><span class="sxs-lookup"><span data-stu-id="23f73-136">id</span></span>|<span data-ttu-id="23f73-137">Строка</span><span class="sxs-lookup"><span data-stu-id="23f73-137">String</span></span>|<span data-ttu-id="23f73-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="23f73-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="23f73-139">displayName</span><span class="sxs-lookup"><span data-stu-id="23f73-139">displayName</span></span>|<span data-ttu-id="23f73-140">Строка</span><span class="sxs-lookup"><span data-stu-id="23f73-140">String</span></span>|<span data-ttu-id="23f73-141">Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="23f73-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="23f73-142">description</span><span class="sxs-lookup"><span data-stu-id="23f73-142">description</span></span>|<span data-ttu-id="23f73-143">String</span><span class="sxs-lookup"><span data-stu-id="23f73-143">String</span></span>|<span data-ttu-id="23f73-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="23f73-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="23f73-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23f73-145">createdDateTime</span></span>|<span data-ttu-id="23f73-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23f73-146">DateTimeOffset</span></span>|<span data-ttu-id="23f73-147">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="23f73-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="23f73-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23f73-148">lastModifiedDateTime</span></span>|<span data-ttu-id="23f73-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23f73-149">DateTimeOffset</span></span>|<span data-ttu-id="23f73-150">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="23f73-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="23f73-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="23f73-151">tokenValue</span></span>|<span data-ttu-id="23f73-152">String</span><span class="sxs-lookup"><span data-stu-id="23f73-152">String</span></span>|<span data-ttu-id="23f73-153">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="23f73-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="23f73-154">токенкреатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="23f73-154">tokenCreationDateTime</span></span>|<span data-ttu-id="23f73-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23f73-155">DateTimeOffset</span></span>|<span data-ttu-id="23f73-156">Дата и время создания последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="23f73-156">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="23f73-157">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="23f73-157">tokenExpirationDateTime</span></span>|<span data-ttu-id="23f73-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23f73-158">DateTimeOffset</span></span>|<span data-ttu-id="23f73-159">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="23f73-159">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="23f73-160">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="23f73-160">enrolledDeviceCount</span></span>|<span data-ttu-id="23f73-161">Int32</span><span class="sxs-lookup"><span data-stu-id="23f73-161">Int32</span></span>|<span data-ttu-id="23f73-162">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="23f73-162">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="23f73-163">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="23f73-163">qrCodeContent</span></span>|<span data-ttu-id="23f73-164">String</span><span class="sxs-lookup"><span data-stu-id="23f73-164">String</span></span>|<span data-ttu-id="23f73-165">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="23f73-165">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="23f73-166">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="23f73-166">qrCodeImage</span></span>|[<span data-ttu-id="23f73-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="23f73-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="23f73-168">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="23f73-168">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="23f73-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="23f73-169">roleScopeTagIds</span></span>|<span data-ttu-id="23f73-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="23f73-170">String collection</span></span>|<span data-ttu-id="23f73-171">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="23f73-171">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="23f73-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="23f73-172">Response</span></span>
<span data-ttu-id="23f73-173">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23f73-173">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23f73-174">Пример</span><span class="sxs-lookup"><span data-stu-id="23f73-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="23f73-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="23f73-175">Request</span></span>
<span data-ttu-id="23f73-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23f73-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="23f73-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="23f73-177">Response</span></span>
<span data-ttu-id="23f73-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23f73-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





