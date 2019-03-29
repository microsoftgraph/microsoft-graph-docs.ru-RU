---
title: Создание Андроиддевицеовнеренроллментпрофиле
description: Создание нового объекта Андроиддевицеовнеренроллментпрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2034ac39671f5e949c93bc9e2b6468aa7895959
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984844"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="6c04c-103">Создание Андроиддевицеовнеренроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="6c04c-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="6c04c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c04c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c04c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c04c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c04c-106">Создание нового объекта [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6c04c-106">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c04c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6c04c-107">Prerequisites</span></span>
<span data-ttu-id="6c04c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c04c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c04c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c04c-110">Permission type</span></span>|<span data-ttu-id="6c04c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c04c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c04c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c04c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c04c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c04c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c04c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c04c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c04c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c04c-115">Not supported.</span></span>|
|<span data-ttu-id="6c04c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c04c-116">Application</span></span>|<span data-ttu-id="6c04c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c04c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c04c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c04c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="6c04c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c04c-119">Request headers</span></span>
|<span data-ttu-id="6c04c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c04c-120">Header</span></span>|<span data-ttu-id="6c04c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6c04c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c04c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c04c-122">Authorization</span></span>|<span data-ttu-id="6c04c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c04c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c04c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6c04c-124">Accept</span></span>|<span data-ttu-id="6c04c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c04c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c04c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c04c-126">Request body</span></span>
<span data-ttu-id="6c04c-127">В тексте запроса добавьте представление объекта Андроиддевицеовнеренроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c04c-127">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="6c04c-128">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнеренроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="6c04c-128">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="6c04c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c04c-129">Property</span></span>|<span data-ttu-id="6c04c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6c04c-130">Type</span></span>|<span data-ttu-id="6c04c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6c04c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c04c-132">accountId</span><span class="sxs-lookup"><span data-stu-id="6c04c-132">accountId</span></span>|<span data-ttu-id="6c04c-133">String</span><span class="sxs-lookup"><span data-stu-id="6c04c-133">String</span></span>|<span data-ttu-id="6c04c-134">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="6c04c-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="6c04c-135">id</span><span class="sxs-lookup"><span data-stu-id="6c04c-135">id</span></span>|<span data-ttu-id="6c04c-136">Строка</span><span class="sxs-lookup"><span data-stu-id="6c04c-136">String</span></span>|<span data-ttu-id="6c04c-137">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="6c04c-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="6c04c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="6c04c-138">displayName</span></span>|<span data-ttu-id="6c04c-139">Строка</span><span class="sxs-lookup"><span data-stu-id="6c04c-139">String</span></span>|<span data-ttu-id="6c04c-140">Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="6c04c-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="6c04c-141">description</span><span class="sxs-lookup"><span data-stu-id="6c04c-141">description</span></span>|<span data-ttu-id="6c04c-142">String</span><span class="sxs-lookup"><span data-stu-id="6c04c-142">String</span></span>|<span data-ttu-id="6c04c-143">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="6c04c-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="6c04c-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c04c-144">createdDateTime</span></span>|<span data-ttu-id="6c04c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c04c-145">DateTimeOffset</span></span>|<span data-ttu-id="6c04c-146">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="6c04c-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="6c04c-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c04c-147">lastModifiedDateTime</span></span>|<span data-ttu-id="6c04c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c04c-148">DateTimeOffset</span></span>|<span data-ttu-id="6c04c-149">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="6c04c-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="6c04c-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="6c04c-150">tokenValue</span></span>|<span data-ttu-id="6c04c-151">String</span><span class="sxs-lookup"><span data-stu-id="6c04c-151">String</span></span>|<span data-ttu-id="6c04c-152">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="6c04c-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="6c04c-153">Токенкреатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="6c04c-153">tokenCreationDateTime</span></span>|<span data-ttu-id="6c04c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c04c-154">DateTimeOffset</span></span>|<span data-ttu-id="6c04c-155">Дата и время создания последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="6c04c-155">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="6c04c-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6c04c-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="6c04c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c04c-157">DateTimeOffset</span></span>|<span data-ttu-id="6c04c-158">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="6c04c-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="6c04c-159">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6c04c-159">enrolledDeviceCount</span></span>|<span data-ttu-id="6c04c-160">Int32</span><span class="sxs-lookup"><span data-stu-id="6c04c-160">Int32</span></span>|<span data-ttu-id="6c04c-161">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="6c04c-161">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="6c04c-162">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="6c04c-162">qrCodeContent</span></span>|<span data-ttu-id="6c04c-163">String</span><span class="sxs-lookup"><span data-stu-id="6c04c-163">String</span></span>|<span data-ttu-id="6c04c-164">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="6c04c-164">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="6c04c-165">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="6c04c-165">qrCodeImage</span></span>|[<span data-ttu-id="6c04c-166">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6c04c-166">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6c04c-167">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="6c04c-167">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="6c04c-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c04c-168">Response</span></span>
<span data-ttu-id="6c04c-169">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c04c-169">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c04c-170">Пример</span><span class="sxs-lookup"><span data-stu-id="6c04c-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c04c-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c04c-171">Request</span></span>
<span data-ttu-id="6c04c-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c04c-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
Content-type: application/json
Content-length: 565

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
  }
}
```

### <a name="response"></a><span data-ttu-id="6c04c-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c04c-173">Response</span></span>
<span data-ttu-id="6c04c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c04c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 737

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
  }
}
```




