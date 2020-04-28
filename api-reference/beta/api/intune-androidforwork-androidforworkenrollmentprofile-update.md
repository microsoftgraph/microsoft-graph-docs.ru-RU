---
title: Обновление объекта androidForWorkEnrollmentProfile
description: Обновление свойств объекта androidForWorkEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4473962aaa9ad4a9acccbd26e937f5efdecb5b5f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43395841"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="1a486-103">Обновление объекта androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="1a486-103">Update androidForWorkEnrollmentProfile</span></span>

<span data-ttu-id="1a486-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a486-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a486-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a486-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a486-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a486-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a486-107">Обновление свойств объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="1a486-107">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a486-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1a486-108">Prerequisites</span></span>
<span data-ttu-id="1a486-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a486-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a486-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a486-111">Permission type</span></span>|<span data-ttu-id="1a486-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a486-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a486-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a486-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a486-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a486-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a486-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a486-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a486-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a486-116">Not supported.</span></span>|
|<span data-ttu-id="1a486-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a486-117">Application</span></span>|<span data-ttu-id="1a486-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a486-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a486-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a486-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="1a486-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1a486-120">Request headers</span></span>
|<span data-ttu-id="1a486-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a486-121">Header</span></span>|<span data-ttu-id="1a486-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1a486-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a486-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a486-123">Authorization</span></span>|<span data-ttu-id="1a486-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a486-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a486-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1a486-125">Accept</span></span>|<span data-ttu-id="1a486-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a486-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a486-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a486-127">Request body</span></span>
<span data-ttu-id="1a486-128">В тексте запроса добавьте представление объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a486-128">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="1a486-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="1a486-129">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="1a486-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a486-130">Property</span></span>|<span data-ttu-id="1a486-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1a486-131">Type</span></span>|<span data-ttu-id="1a486-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1a486-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a486-133">accountId</span><span class="sxs-lookup"><span data-stu-id="1a486-133">accountId</span></span>|<span data-ttu-id="1a486-134">String</span><span class="sxs-lookup"><span data-stu-id="1a486-134">String</span></span>|<span data-ttu-id="1a486-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="1a486-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="1a486-136">id</span><span class="sxs-lookup"><span data-stu-id="1a486-136">id</span></span>|<span data-ttu-id="1a486-137">Строка</span><span class="sxs-lookup"><span data-stu-id="1a486-137">String</span></span>|<span data-ttu-id="1a486-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1a486-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="1a486-139">displayName</span><span class="sxs-lookup"><span data-stu-id="1a486-139">displayName</span></span>|<span data-ttu-id="1a486-140">Строка</span><span class="sxs-lookup"><span data-stu-id="1a486-140">String</span></span>|<span data-ttu-id="1a486-141">Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1a486-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="1a486-142">description</span><span class="sxs-lookup"><span data-stu-id="1a486-142">description</span></span>|<span data-ttu-id="1a486-143">String</span><span class="sxs-lookup"><span data-stu-id="1a486-143">String</span></span>|<span data-ttu-id="1a486-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1a486-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="1a486-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a486-145">createdDateTime</span></span>|<span data-ttu-id="1a486-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a486-146">DateTimeOffset</span></span>|<span data-ttu-id="1a486-147">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1a486-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="1a486-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a486-148">lastModifiedDateTime</span></span>|<span data-ttu-id="1a486-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a486-149">DateTimeOffset</span></span>|<span data-ttu-id="1a486-150">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1a486-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="1a486-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="1a486-151">tokenValue</span></span>|<span data-ttu-id="1a486-152">String</span><span class="sxs-lookup"><span data-stu-id="1a486-152">String</span></span>|<span data-ttu-id="1a486-153">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1a486-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="1a486-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1a486-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="1a486-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a486-155">DateTimeOffset</span></span>|<span data-ttu-id="1a486-156">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="1a486-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="1a486-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1a486-157">enrolledDeviceCount</span></span>|<span data-ttu-id="1a486-158">Int32</span><span class="sxs-lookup"><span data-stu-id="1a486-158">Int32</span></span>|<span data-ttu-id="1a486-159">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="1a486-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="1a486-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="1a486-160">qrCodeContent</span></span>|<span data-ttu-id="1a486-161">String</span><span class="sxs-lookup"><span data-stu-id="1a486-161">String</span></span>|<span data-ttu-id="1a486-162">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="1a486-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="1a486-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="1a486-163">qrCodeImage</span></span>|[<span data-ttu-id="1a486-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1a486-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1a486-165">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="1a486-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="1a486-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a486-166">Response</span></span>
<span data-ttu-id="1a486-167">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a486-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a486-168">Пример</span><span class="sxs-lookup"><span data-stu-id="1a486-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a486-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a486-169">Request</span></span>
<span data-ttu-id="1a486-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a486-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
Content-type: application/json
Content-length: 496

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="1a486-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a486-171">Response</span></span>
<span data-ttu-id="1a486-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a486-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 668

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "e6742553-2553-e674-5325-74e6532574e6",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "enrolledDeviceCount": 3,
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```



