---
title: Создание Андроиддевицеовнеренроллментпрофиле
description: Создание нового объекта Андроиддевицеовнеренроллментпрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 888c20a0e8b409137501695b9363019d61c732b1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142401"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="10bea-103">Создание Андроиддевицеовнеренроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="10bea-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="10bea-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10bea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10bea-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10bea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10bea-106">Создание нового объекта [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="10bea-106">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10bea-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="10bea-107">Prerequisites</span></span>
<span data-ttu-id="10bea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="10bea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="10bea-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10bea-110">Permission type</span></span>|<span data-ttu-id="10bea-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10bea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10bea-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10bea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10bea-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10bea-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="10bea-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10bea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10bea-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10bea-115">Not supported.</span></span>|
|<span data-ttu-id="10bea-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10bea-116">Application</span></span>|<span data-ttu-id="10bea-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10bea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10bea-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10bea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="10bea-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10bea-119">Request headers</span></span>
|<span data-ttu-id="10bea-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10bea-120">Header</span></span>|<span data-ttu-id="10bea-121">Значение</span><span class="sxs-lookup"><span data-stu-id="10bea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10bea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="10bea-122">Authorization</span></span>|<span data-ttu-id="10bea-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="10bea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10bea-124">Accept</span><span class="sxs-lookup"><span data-stu-id="10bea-124">Accept</span></span>|<span data-ttu-id="10bea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10bea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10bea-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10bea-126">Request body</span></span>
<span data-ttu-id="10bea-127">В тексте запроса добавьте представление объекта Андроиддевицеовнеренроллментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10bea-127">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="10bea-128">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнеренроллментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="10bea-128">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="10bea-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="10bea-129">Property</span></span>|<span data-ttu-id="10bea-130">Тип</span><span class="sxs-lookup"><span data-stu-id="10bea-130">Type</span></span>|<span data-ttu-id="10bea-131">Описание</span><span class="sxs-lookup"><span data-stu-id="10bea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10bea-132">accountId</span><span class="sxs-lookup"><span data-stu-id="10bea-132">accountId</span></span>|<span data-ttu-id="10bea-133">String</span><span class="sxs-lookup"><span data-stu-id="10bea-133">String</span></span>|<span data-ttu-id="10bea-134">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="10bea-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="10bea-135">id</span><span class="sxs-lookup"><span data-stu-id="10bea-135">id</span></span>|<span data-ttu-id="10bea-136">String</span><span class="sxs-lookup"><span data-stu-id="10bea-136">String</span></span>|<span data-ttu-id="10bea-137">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="10bea-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="10bea-138">displayName</span><span class="sxs-lookup"><span data-stu-id="10bea-138">displayName</span></span>|<span data-ttu-id="10bea-139">String</span><span class="sxs-lookup"><span data-stu-id="10bea-139">String</span></span>|<span data-ttu-id="10bea-140">Отображаемое имя профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="10bea-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="10bea-141">description</span><span class="sxs-lookup"><span data-stu-id="10bea-141">description</span></span>|<span data-ttu-id="10bea-142">String</span><span class="sxs-lookup"><span data-stu-id="10bea-142">String</span></span>|<span data-ttu-id="10bea-143">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="10bea-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="10bea-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10bea-144">createdDateTime</span></span>|<span data-ttu-id="10bea-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10bea-145">DateTimeOffset</span></span>|<span data-ttu-id="10bea-146">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="10bea-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="10bea-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10bea-147">lastModifiedDateTime</span></span>|<span data-ttu-id="10bea-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10bea-148">DateTimeOffset</span></span>|<span data-ttu-id="10bea-149">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="10bea-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="10bea-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="10bea-150">tokenValue</span></span>|<span data-ttu-id="10bea-151">String</span><span class="sxs-lookup"><span data-stu-id="10bea-151">String</span></span>|<span data-ttu-id="10bea-152">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="10bea-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="10bea-153">Токенкреатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="10bea-153">tokenCreationDateTime</span></span>|<span data-ttu-id="10bea-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10bea-154">DateTimeOffset</span></span>|<span data-ttu-id="10bea-155">Дата и время создания последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="10bea-155">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="10bea-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="10bea-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="10bea-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10bea-157">DateTimeOffset</span></span>|<span data-ttu-id="10bea-158">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="10bea-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="10bea-159">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="10bea-159">enrolledDeviceCount</span></span>|<span data-ttu-id="10bea-160">Int32</span><span class="sxs-lookup"><span data-stu-id="10bea-160">Int32</span></span>|<span data-ttu-id="10bea-161">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="10bea-161">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="10bea-162">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="10bea-162">qrCodeContent</span></span>|<span data-ttu-id="10bea-163">String</span><span class="sxs-lookup"><span data-stu-id="10bea-163">String</span></span>|<span data-ttu-id="10bea-164">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="10bea-164">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="10bea-165">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="10bea-165">qrCodeImage</span></span>|[<span data-ttu-id="10bea-166">mimeContent</span><span class="sxs-lookup"><span data-stu-id="10bea-166">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="10bea-167">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="10bea-167">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="10bea-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="10bea-168">Response</span></span>
<span data-ttu-id="10bea-169">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнеренроллментпрофиле](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10bea-169">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10bea-170">Пример</span><span class="sxs-lookup"><span data-stu-id="10bea-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="10bea-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="10bea-171">Request</span></span>
<span data-ttu-id="10bea-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10bea-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="10bea-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="10bea-173">Response</span></span>
<span data-ttu-id="10bea-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="10bea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




