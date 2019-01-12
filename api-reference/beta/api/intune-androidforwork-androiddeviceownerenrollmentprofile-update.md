---
title: Обновление androidDeviceOwnerEnrollmentProfile
description: Обновление свойства объекта androidDeviceOwnerEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f4b8e87f44259e2bf3db9460f71a376b107d28d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921285"
---
# <a name="update-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="43a65-103">Обновление androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="43a65-103">Update androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="43a65-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="43a65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43a65-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43a65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43a65-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="43a65-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43a65-107">Обновление свойства объекта [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="43a65-107">Update the properties of a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="43a65-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="43a65-108">Prerequisites</span></span>
<span data-ttu-id="43a65-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43a65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43a65-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43a65-111">Permission type</span></span>|<span data-ttu-id="43a65-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43a65-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43a65-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43a65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43a65-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43a65-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43a65-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43a65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43a65-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43a65-116">Not supported.</span></span>|
|<span data-ttu-id="43a65-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43a65-117">Application</span></span>|<span data-ttu-id="43a65-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43a65-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43a65-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43a65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="43a65-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43a65-120">Request headers</span></span>
|<span data-ttu-id="43a65-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43a65-121">Header</span></span>|<span data-ttu-id="43a65-122">Значение</span><span class="sxs-lookup"><span data-stu-id="43a65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43a65-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43a65-123">Authorization</span></span>|<span data-ttu-id="43a65-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="43a65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43a65-125">Accept</span><span class="sxs-lookup"><span data-stu-id="43a65-125">Accept</span></span>|<span data-ttu-id="43a65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43a65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43a65-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="43a65-127">Request body</span></span>
<span data-ttu-id="43a65-128">В тексте запроса укажите представление JSON для объекта [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="43a65-128">In the request body, supply a JSON representation for the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

<span data-ttu-id="43a65-129">В следующей таблице показаны свойства, которые необходимы для создания [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="43a65-129">The following table shows the properties that are required when you create the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>

|<span data-ttu-id="43a65-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="43a65-130">Property</span></span>|<span data-ttu-id="43a65-131">Тип</span><span class="sxs-lookup"><span data-stu-id="43a65-131">Type</span></span>|<span data-ttu-id="43a65-132">Описание</span><span class="sxs-lookup"><span data-stu-id="43a65-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43a65-133">accountId</span><span class="sxs-lookup"><span data-stu-id="43a65-133">accountId</span></span>|<span data-ttu-id="43a65-134">String</span><span class="sxs-lookup"><span data-stu-id="43a65-134">String</span></span>|<span data-ttu-id="43a65-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="43a65-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="43a65-136">id</span><span class="sxs-lookup"><span data-stu-id="43a65-136">id</span></span>|<span data-ttu-id="43a65-137">String</span><span class="sxs-lookup"><span data-stu-id="43a65-137">String</span></span>|<span data-ttu-id="43a65-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="43a65-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="43a65-139">displayName</span><span class="sxs-lookup"><span data-stu-id="43a65-139">displayName</span></span>|<span data-ttu-id="43a65-140">String</span><span class="sxs-lookup"><span data-stu-id="43a65-140">String</span></span>|<span data-ttu-id="43a65-141">Отображаемое имя профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="43a65-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="43a65-142">описание</span><span class="sxs-lookup"><span data-stu-id="43a65-142">description</span></span>|<span data-ttu-id="43a65-143">String</span><span class="sxs-lookup"><span data-stu-id="43a65-143">String</span></span>|<span data-ttu-id="43a65-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="43a65-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="43a65-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43a65-145">createdDateTime</span></span>|<span data-ttu-id="43a65-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43a65-146">DateTimeOffset</span></span>|<span data-ttu-id="43a65-147">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="43a65-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="43a65-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43a65-148">lastModifiedDateTime</span></span>|<span data-ttu-id="43a65-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43a65-149">DateTimeOffset</span></span>|<span data-ttu-id="43a65-150">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="43a65-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="43a65-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="43a65-151">tokenValue</span></span>|<span data-ttu-id="43a65-152">String</span><span class="sxs-lookup"><span data-stu-id="43a65-152">String</span></span>|<span data-ttu-id="43a65-153">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="43a65-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="43a65-154">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="43a65-154">tokenCreationDateTime</span></span>|<span data-ttu-id="43a65-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43a65-155">DateTimeOffset</span></span>|<span data-ttu-id="43a65-156">Дата и время создания недавно созданного маркер.</span><span class="sxs-lookup"><span data-stu-id="43a65-156">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="43a65-157">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="43a65-157">tokenExpirationDateTime</span></span>|<span data-ttu-id="43a65-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43a65-158">DateTimeOffset</span></span>|<span data-ttu-id="43a65-159">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="43a65-159">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="43a65-160">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="43a65-160">enrolledDeviceCount</span></span>|<span data-ttu-id="43a65-161">Int32</span><span class="sxs-lookup"><span data-stu-id="43a65-161">Int32</span></span>|<span data-ttu-id="43a65-162">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="43a65-162">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="43a65-163">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="43a65-163">qrCodeContent</span></span>|<span data-ttu-id="43a65-164">String</span><span class="sxs-lookup"><span data-stu-id="43a65-164">String</span></span>|<span data-ttu-id="43a65-165">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="43a65-165">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="43a65-166">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="43a65-166">qrCodeImage</span></span>|[<span data-ttu-id="43a65-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="43a65-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="43a65-168">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="43a65-168">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="43a65-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="43a65-169">Response</span></span>
<span data-ttu-id="43a65-170">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="43a65-170">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43a65-171">Пример</span><span class="sxs-lookup"><span data-stu-id="43a65-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="43a65-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="43a65-172">Request</span></span>
<span data-ttu-id="43a65-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43a65-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
Content-type: application/json
Content-length: 555

{
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="43a65-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="43a65-174">Response</span></span>
<span data-ttu-id="43a65-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="43a65-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





