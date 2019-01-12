---
title: Создание androidDeviceOwnerEnrollmentProfile
description: Создание нового объекта androidDeviceOwnerEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7d99ae3099baed597f58afe8ad9b44d568c2cca5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985860"
---
# <a name="create-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="600dd-103">Создание androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="600dd-103">Create androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="600dd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="600dd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="600dd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="600dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="600dd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="600dd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="600dd-107">Создание нового объекта [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="600dd-107">Create a new [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="600dd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="600dd-108">Prerequisites</span></span>
<span data-ttu-id="600dd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="600dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="600dd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="600dd-111">Permission type</span></span>|<span data-ttu-id="600dd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="600dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="600dd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="600dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="600dd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="600dd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="600dd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="600dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="600dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="600dd-116">Not supported.</span></span>|
|<span data-ttu-id="600dd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="600dd-117">Application</span></span>|<span data-ttu-id="600dd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="600dd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="600dd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="600dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="600dd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="600dd-120">Request headers</span></span>
|<span data-ttu-id="600dd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="600dd-121">Header</span></span>|<span data-ttu-id="600dd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="600dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="600dd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="600dd-123">Authorization</span></span>|<span data-ttu-id="600dd-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="600dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="600dd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="600dd-125">Accept</span></span>|<span data-ttu-id="600dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="600dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="600dd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="600dd-127">Request body</span></span>
<span data-ttu-id="600dd-128">В тексте запроса укажите представление JSON для объекта androidDeviceOwnerEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="600dd-128">In the request body, supply a JSON representation for the androidDeviceOwnerEnrollmentProfile object.</span></span>

<span data-ttu-id="600dd-129">В следующей таблице показаны свойства, которые необходимы для создания androidDeviceOwnerEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="600dd-129">The following table shows the properties that are required when you create the androidDeviceOwnerEnrollmentProfile.</span></span>

|<span data-ttu-id="600dd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="600dd-130">Property</span></span>|<span data-ttu-id="600dd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="600dd-131">Type</span></span>|<span data-ttu-id="600dd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="600dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="600dd-133">accountId</span><span class="sxs-lookup"><span data-stu-id="600dd-133">accountId</span></span>|<span data-ttu-id="600dd-134">String</span><span class="sxs-lookup"><span data-stu-id="600dd-134">String</span></span>|<span data-ttu-id="600dd-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="600dd-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="600dd-136">id</span><span class="sxs-lookup"><span data-stu-id="600dd-136">id</span></span>|<span data-ttu-id="600dd-137">String</span><span class="sxs-lookup"><span data-stu-id="600dd-137">String</span></span>|<span data-ttu-id="600dd-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="600dd-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="600dd-139">displayName</span><span class="sxs-lookup"><span data-stu-id="600dd-139">displayName</span></span>|<span data-ttu-id="600dd-140">String</span><span class="sxs-lookup"><span data-stu-id="600dd-140">String</span></span>|<span data-ttu-id="600dd-141">Отображаемое имя профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="600dd-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="600dd-142">описание</span><span class="sxs-lookup"><span data-stu-id="600dd-142">description</span></span>|<span data-ttu-id="600dd-143">String</span><span class="sxs-lookup"><span data-stu-id="600dd-143">String</span></span>|<span data-ttu-id="600dd-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="600dd-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="600dd-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="600dd-145">createdDateTime</span></span>|<span data-ttu-id="600dd-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="600dd-146">DateTimeOffset</span></span>|<span data-ttu-id="600dd-147">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="600dd-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="600dd-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="600dd-148">lastModifiedDateTime</span></span>|<span data-ttu-id="600dd-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="600dd-149">DateTimeOffset</span></span>|<span data-ttu-id="600dd-150">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="600dd-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="600dd-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="600dd-151">tokenValue</span></span>|<span data-ttu-id="600dd-152">String</span><span class="sxs-lookup"><span data-stu-id="600dd-152">String</span></span>|<span data-ttu-id="600dd-153">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="600dd-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="600dd-154">tokenCreationDateTime</span><span class="sxs-lookup"><span data-stu-id="600dd-154">tokenCreationDateTime</span></span>|<span data-ttu-id="600dd-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="600dd-155">DateTimeOffset</span></span>|<span data-ttu-id="600dd-156">Дата и время создания недавно созданного маркер.</span><span class="sxs-lookup"><span data-stu-id="600dd-156">Date time the most recently created token was created.</span></span>|
|<span data-ttu-id="600dd-157">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="600dd-157">tokenExpirationDateTime</span></span>|<span data-ttu-id="600dd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="600dd-158">DateTimeOffset</span></span>|<span data-ttu-id="600dd-159">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="600dd-159">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="600dd-160">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="600dd-160">enrolledDeviceCount</span></span>|<span data-ttu-id="600dd-161">Int32</span><span class="sxs-lookup"><span data-stu-id="600dd-161">Int32</span></span>|<span data-ttu-id="600dd-162">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="600dd-162">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="600dd-163">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="600dd-163">qrCodeContent</span></span>|<span data-ttu-id="600dd-164">String</span><span class="sxs-lookup"><span data-stu-id="600dd-164">String</span></span>|<span data-ttu-id="600dd-165">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="600dd-165">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="600dd-166">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="600dd-166">qrCodeImage</span></span>|[<span data-ttu-id="600dd-167">mimeContent</span><span class="sxs-lookup"><span data-stu-id="600dd-167">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="600dd-168">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="600dd-168">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="600dd-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="600dd-169">Response</span></span>
<span data-ttu-id="600dd-170">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="600dd-170">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="600dd-171">Пример</span><span class="sxs-lookup"><span data-stu-id="600dd-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="600dd-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="600dd-172">Request</span></span>
<span data-ttu-id="600dd-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="600dd-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
Content-type: application/json
Content-length: 629

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
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

### <a name="response"></a><span data-ttu-id="600dd-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="600dd-174">Response</span></span>
<span data-ttu-id="600dd-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="600dd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





