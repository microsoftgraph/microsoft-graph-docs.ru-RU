---
title: Обновление androidDeviceOwnerEnrollmentProfile
description: Обновление свойства объекта androidDeviceOwnerEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 966b538b161dca2bc5c85390cab5cd8bd371b236
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413831"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="8cb3f-103">Обновление androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="8cb3f-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="8cb3f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8cb3f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8cb3f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cb3f-107">Обновление свойства объекта [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8cb3f-107">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cb3f-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="8cb3f-108">Prerequisites</span></span>
<span data-ttu-id="8cb3f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8cb3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8cb3f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cb3f-111">Permission type</span></span>|<span data-ttu-id="8cb3f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cb3f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cb3f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cb3f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8cb3f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cb3f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8cb3f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cb3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cb3f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-116">Not supported.</span></span>|
|<span data-ttu-id="8cb3f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8cb3f-117">Application</span></span>|<span data-ttu-id="8cb3f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cb3f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cb3f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="8cb3f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8cb3f-120">Request headers</span></span>
|<span data-ttu-id="8cb3f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8cb3f-121">Header</span></span>|<span data-ttu-id="8cb3f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8cb3f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cb3f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cb3f-123">Authorization</span></span>|<span data-ttu-id="8cb3f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8cb3f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cb3f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8cb3f-125">Accept</span></span>|<span data-ttu-id="8cb3f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8cb3f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cb3f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8cb3f-127">Request body</span></span>
<span data-ttu-id="8cb3f-128">В тексте запроса укажите представление JSON для объекта [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8cb3f-128">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="8cb3f-129">В следующей таблице показаны свойства, которые необходимы для создания [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="8cb3f-129">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="8cb3f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cb3f-130">Property</span></span>|<span data-ttu-id="8cb3f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8cb3f-131">Type</span></span>|<span data-ttu-id="8cb3f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8cb3f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cb3f-133">accountId</span><span class="sxs-lookup"><span data-stu-id="8cb3f-133">accountId</span></span>|<span data-ttu-id="8cb3f-134">String</span><span class="sxs-lookup"><span data-stu-id="8cb3f-134">String</span></span>|<span data-ttu-id="8cb3f-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="8cb3f-136">id</span><span class="sxs-lookup"><span data-stu-id="8cb3f-136">id</span></span>|<span data-ttu-id="8cb3f-137">String</span><span class="sxs-lookup"><span data-stu-id="8cb3f-137">String</span></span>|<span data-ttu-id="8cb3f-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="8cb3f-139">displayName</span><span class="sxs-lookup"><span data-stu-id="8cb3f-139">displayName</span></span>|<span data-ttu-id="8cb3f-140">String</span><span class="sxs-lookup"><span data-stu-id="8cb3f-140">String</span></span>|<span data-ttu-id="8cb3f-141">Отображаемое имя профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="8cb3f-142">description</span><span class="sxs-lookup"><span data-stu-id="8cb3f-142">description</span></span>|<span data-ttu-id="8cb3f-143">String</span><span class="sxs-lookup"><span data-stu-id="8cb3f-143">String</span></span>|<span data-ttu-id="8cb3f-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="8cb3f-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8cb3f-145">createdDateTime</span></span>|<span data-ttu-id="8cb3f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cb3f-146">DateTimeOffset</span></span>|<span data-ttu-id="8cb3f-147">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="8cb3f-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cb3f-148">lastModifiedDateTime</span></span>|<span data-ttu-id="8cb3f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cb3f-149">DateTimeOffset</span></span>|<span data-ttu-id="8cb3f-150">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="8cb3f-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="8cb3f-151">tokenValue</span></span>|<span data-ttu-id="8cb3f-152">String</span><span class="sxs-lookup"><span data-stu-id="8cb3f-152">String</span></span>|<span data-ttu-id="8cb3f-153">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="8cb3f-154">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="8cb3f-154">tokenCreationDateTime</span></span>|<span data-ttu-id="8cb3f-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cb3f-155">DateTimeOffset</span></span>|<span data-ttu-id="8cb3f-156">Дата и время создания недавно созданного маркер.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-156">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="8cb3f-157">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8cb3f-157">tokenExpirationDateTime</span></span>|<span data-ttu-id="8cb3f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cb3f-158">DateTimeOffset</span></span>|<span data-ttu-id="8cb3f-159">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-159">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="8cb3f-160">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8cb3f-160">enrolledDeviceCount</span></span>|<span data-ttu-id="8cb3f-161">Int32</span><span class="sxs-lookup"><span data-stu-id="8cb3f-161">Int32</span></span>|<span data-ttu-id="8cb3f-162">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-162">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="8cb3f-163">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="8cb3f-163">qrCodeContent</span></span>|<span data-ttu-id="8cb3f-164">String</span><span class="sxs-lookup"><span data-stu-id="8cb3f-164">String</span></span>|<span data-ttu-id="8cb3f-165">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-165">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="8cb3f-166">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="8cb3f-166">qrCodeImage</span></span>|[<span data-ttu-id="8cb3f-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8cb3f-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8cb3f-168">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-168">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="8cb3f-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cb3f-169">Response</span></span>
<span data-ttu-id="8cb3f-170">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-170">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cb3f-171">Пример</span><span class="sxs-lookup"><span data-stu-id="8cb3f-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cb3f-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cb3f-172">Request</span></span>
<span data-ttu-id="8cb3f-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
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

### <a name="response"></a><span data-ttu-id="8cb3f-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cb3f-174">Response</span></span>
<span data-ttu-id="8cb3f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8cb3f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




