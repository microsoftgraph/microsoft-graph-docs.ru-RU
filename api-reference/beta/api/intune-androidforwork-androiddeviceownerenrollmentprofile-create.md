---
title: Создание Андроиддевицеовнеренроллментпрофиле
description: Создание нового объекта Андроиддевицеовнеренроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cdf6e3d05ef5b094decffe7bd9d0e847ffa435e2
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123661"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="1b09b-103">Создание Андроиддевицеовнеренроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="1b09b-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

<span data-ttu-id="1b09b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b09b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b09b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b09b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b09b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b09b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b09b-107">Создание нового объекта [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="1b09b-107">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b09b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1b09b-108">Prerequisites</span></span>
<span data-ttu-id="1b09b-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1b09b-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1b09b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b09b-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b09b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b09b-111">Permission type</span></span>|<span data-ttu-id="1b09b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b09b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b09b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b09b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b09b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b09b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b09b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b09b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b09b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b09b-116">Not supported.</span></span>|
|<span data-ttu-id="1b09b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b09b-117">Application</span></span>|<span data-ttu-id="1b09b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b09b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b09b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b09b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="1b09b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1b09b-120">Request headers</span></span>
|<span data-ttu-id="1b09b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b09b-121">Header</span></span>|<span data-ttu-id="1b09b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1b09b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b09b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b09b-123">Authorization</span></span>|<span data-ttu-id="1b09b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b09b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b09b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1b09b-125">Accept</span></span>|<span data-ttu-id="1b09b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b09b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b09b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b09b-127">Request body</span></span>
<span data-ttu-id="1b09b-128">В тексте запроса добавьте представление объекта Андроиддевицеовнеренроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b09b-128">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="1b09b-129">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнеренроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="1b09b-129">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="1b09b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b09b-130">Property</span></span>|<span data-ttu-id="1b09b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1b09b-131">Type</span></span>|<span data-ttu-id="1b09b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1b09b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b09b-133">accountId</span><span class="sxs-lookup"><span data-stu-id="1b09b-133">accountId</span></span>|<span data-ttu-id="1b09b-134">String</span><span class="sxs-lookup"><span data-stu-id="1b09b-134">String</span></span>|<span data-ttu-id="1b09b-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="1b09b-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="1b09b-136">id</span><span class="sxs-lookup"><span data-stu-id="1b09b-136">id</span></span>|<span data-ttu-id="1b09b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="1b09b-137">String</span></span>|<span data-ttu-id="1b09b-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1b09b-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="1b09b-139">displayName</span><span class="sxs-lookup"><span data-stu-id="1b09b-139">displayName</span></span>|<span data-ttu-id="1b09b-140">Строка</span><span class="sxs-lookup"><span data-stu-id="1b09b-140">String</span></span>|<span data-ttu-id="1b09b-141">Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1b09b-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="1b09b-142">description</span><span class="sxs-lookup"><span data-stu-id="1b09b-142">description</span></span>|<span data-ttu-id="1b09b-143">String</span><span class="sxs-lookup"><span data-stu-id="1b09b-143">String</span></span>|<span data-ttu-id="1b09b-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1b09b-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="1b09b-145">енроллментмоде</span><span class="sxs-lookup"><span data-stu-id="1b09b-145">enrollmentMode</span></span>|[<span data-ttu-id="1b09b-146">андроиддевицеовнеренроллментмоде</span><span class="sxs-lookup"><span data-stu-id="1b09b-146">androidDeviceOwnerEnrollmentMode</span></span>](../resources/intune-androidforwork-androiddeviceownerenrollmentmode.md)|<span data-ttu-id="1b09b-147">Режим регистрации устройств, использующих этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="1b09b-147">The enrollment mode of devices that use this enrollment profile.</span></span> <span data-ttu-id="1b09b-148">Возможные значения: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="1b09b-148">Possible values are: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`.</span></span>|
|<span data-ttu-id="1b09b-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b09b-149">createdDateTime</span></span>|<span data-ttu-id="1b09b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b09b-150">DateTimeOffset</span></span>|<span data-ttu-id="1b09b-151">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1b09b-151">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="1b09b-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b09b-152">lastModifiedDateTime</span></span>|<span data-ttu-id="1b09b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b09b-153">DateTimeOffset</span></span>|<span data-ttu-id="1b09b-154">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1b09b-154">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="1b09b-155">tokenValue</span><span class="sxs-lookup"><span data-stu-id="1b09b-155">tokenValue</span></span>|<span data-ttu-id="1b09b-156">String</span><span class="sxs-lookup"><span data-stu-id="1b09b-156">String</span></span>|<span data-ttu-id="1b09b-157">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1b09b-157">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="1b09b-158">токенкреатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="1b09b-158">tokenCreationDateTime</span></span>|<span data-ttu-id="1b09b-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b09b-159">DateTimeOffset</span></span>|<span data-ttu-id="1b09b-160">Дата и время создания последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="1b09b-160">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="1b09b-161">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1b09b-161">tokenExpirationDateTime</span></span>|<span data-ttu-id="1b09b-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b09b-162">DateTimeOffset</span></span>|<span data-ttu-id="1b09b-163">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="1b09b-163">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="1b09b-164">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1b09b-164">enrolledDeviceCount</span></span>|<span data-ttu-id="1b09b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1b09b-165">Int32</span></span>|<span data-ttu-id="1b09b-166">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="1b09b-166">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="1b09b-167">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="1b09b-167">qrCodeContent</span></span>|<span data-ttu-id="1b09b-168">String</span><span class="sxs-lookup"><span data-stu-id="1b09b-168">String</span></span>|<span data-ttu-id="1b09b-169">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="1b09b-169">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="1b09b-170">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="1b09b-170">qrCodeImage</span></span>|[<span data-ttu-id="1b09b-171">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1b09b-171">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1b09b-172">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="1b09b-172">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="1b09b-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1b09b-173">roleScopeTagIds</span></span>|<span data-ttu-id="1b09b-174">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1b09b-174">String collection</span></span>|<span data-ttu-id="1b09b-175">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1b09b-175">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="1b09b-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b09b-176">Response</span></span>
<span data-ttu-id="1b09b-177">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b09b-177">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b09b-178">Пример</span><span class="sxs-lookup"><span data-stu-id="1b09b-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b09b-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b09b-179">Request</span></span>
<span data-ttu-id="1b09b-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b09b-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="1b09b-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b09b-181">Response</span></span>
<span data-ttu-id="1b09b-182">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1b09b-182">Here is an example of the response.</span></span> <span data-ttu-id="1b09b-183">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1b09b-183">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1b09b-184">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1b09b-184">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



