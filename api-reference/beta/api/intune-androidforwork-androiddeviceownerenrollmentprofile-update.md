---
title: Обновление Андроиддевицеовнеренроллментпрофиле
description: Обновление свойств объекта Андроиддевицеовнеренроллментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: edc74d3b23c290cd6fb3473ba2764a6418ac8df7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446263"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="732df-103">Обновление Андроиддевицеовнеренроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="732df-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

<span data-ttu-id="732df-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="732df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="732df-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="732df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="732df-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="732df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="732df-107">Обновление свойств объекта [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="732df-107">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="732df-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="732df-108">Prerequisites</span></span>
<span data-ttu-id="732df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="732df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="732df-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="732df-111">Permission type</span></span>|<span data-ttu-id="732df-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="732df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="732df-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="732df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="732df-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="732df-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="732df-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="732df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="732df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="732df-116">Not supported.</span></span>|
|<span data-ttu-id="732df-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="732df-117">Application</span></span>|<span data-ttu-id="732df-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="732df-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="732df-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="732df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="732df-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="732df-120">Request headers</span></span>
|<span data-ttu-id="732df-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="732df-121">Header</span></span>|<span data-ttu-id="732df-122">Значение</span><span class="sxs-lookup"><span data-stu-id="732df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="732df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="732df-123">Authorization</span></span>|<span data-ttu-id="732df-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="732df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="732df-125">Accept</span><span class="sxs-lookup"><span data-stu-id="732df-125">Accept</span></span>|<span data-ttu-id="732df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="732df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="732df-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="732df-127">Request body</span></span>
<span data-ttu-id="732df-128">В тексте запроса добавьте представление объекта [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="732df-128">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="732df-129">В следующей таблице приведены свойства, необходимые при создании [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="732df-129">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="732df-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="732df-130">Property</span></span>|<span data-ttu-id="732df-131">Тип</span><span class="sxs-lookup"><span data-stu-id="732df-131">Type</span></span>|<span data-ttu-id="732df-132">Описание</span><span class="sxs-lookup"><span data-stu-id="732df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="732df-133">accountId</span><span class="sxs-lookup"><span data-stu-id="732df-133">accountId</span></span>|<span data-ttu-id="732df-134">String</span><span class="sxs-lookup"><span data-stu-id="732df-134">String</span></span>|<span data-ttu-id="732df-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="732df-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="732df-136">id</span><span class="sxs-lookup"><span data-stu-id="732df-136">id</span></span>|<span data-ttu-id="732df-137">Строка</span><span class="sxs-lookup"><span data-stu-id="732df-137">String</span></span>|<span data-ttu-id="732df-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="732df-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="732df-139">displayName</span><span class="sxs-lookup"><span data-stu-id="732df-139">displayName</span></span>|<span data-ttu-id="732df-140">Строка</span><span class="sxs-lookup"><span data-stu-id="732df-140">String</span></span>|<span data-ttu-id="732df-141">Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="732df-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="732df-142">description</span><span class="sxs-lookup"><span data-stu-id="732df-142">description</span></span>|<span data-ttu-id="732df-143">String</span><span class="sxs-lookup"><span data-stu-id="732df-143">String</span></span>|<span data-ttu-id="732df-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="732df-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="732df-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="732df-145">createdDateTime</span></span>|<span data-ttu-id="732df-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="732df-146">DateTimeOffset</span></span>|<span data-ttu-id="732df-147">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="732df-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="732df-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="732df-148">lastModifiedDateTime</span></span>|<span data-ttu-id="732df-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="732df-149">DateTimeOffset</span></span>|<span data-ttu-id="732df-150">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="732df-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="732df-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="732df-151">tokenValue</span></span>|<span data-ttu-id="732df-152">String</span><span class="sxs-lookup"><span data-stu-id="732df-152">String</span></span>|<span data-ttu-id="732df-153">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="732df-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="732df-154">токенкреатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="732df-154">tokenCreationDateTime</span></span>|<span data-ttu-id="732df-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="732df-155">DateTimeOffset</span></span>|<span data-ttu-id="732df-156">Дата и время создания последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="732df-156">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="732df-157">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="732df-157">tokenExpirationDateTime</span></span>|<span data-ttu-id="732df-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="732df-158">DateTimeOffset</span></span>|<span data-ttu-id="732df-159">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="732df-159">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="732df-160">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="732df-160">enrolledDeviceCount</span></span>|<span data-ttu-id="732df-161">Int32</span><span class="sxs-lookup"><span data-stu-id="732df-161">Int32</span></span>|<span data-ttu-id="732df-162">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="732df-162">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="732df-163">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="732df-163">qrCodeContent</span></span>|<span data-ttu-id="732df-164">String</span><span class="sxs-lookup"><span data-stu-id="732df-164">String</span></span>|<span data-ttu-id="732df-165">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="732df-165">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="732df-166">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="732df-166">qrCodeImage</span></span>|[<span data-ttu-id="732df-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="732df-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="732df-168">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="732df-168">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="732df-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="732df-169">roleScopeTagIds</span></span>|<span data-ttu-id="732df-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="732df-170">String collection</span></span>|<span data-ttu-id="732df-171">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="732df-171">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="732df-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="732df-172">Response</span></span>
<span data-ttu-id="732df-173">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="732df-173">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="732df-174">Пример</span><span class="sxs-lookup"><span data-stu-id="732df-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="732df-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="732df-175">Request</span></span>
<span data-ttu-id="732df-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="732df-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="732df-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="732df-177">Response</span></span>
<span data-ttu-id="732df-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="732df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





