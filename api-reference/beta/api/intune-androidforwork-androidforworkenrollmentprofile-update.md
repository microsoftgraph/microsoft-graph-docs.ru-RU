---
title: Обновление объекта androidForWorkEnrollmentProfile
description: Обновление свойств объекта androidForWorkEnrollmentProfile.
ms.openlocfilehash: f0af5db7115de09657d08d093836527e3198cad0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080769"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="6175b-103">Обновление объекта androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="6175b-103">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="6175b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6175b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6175b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6175b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6175b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6175b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6175b-107">Обновление свойств объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="6175b-107">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6175b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6175b-108">Prerequisites</span></span>
<span data-ttu-id="6175b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6175b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6175b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6175b-111">Permission type</span></span>|<span data-ttu-id="6175b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6175b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6175b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6175b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6175b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6175b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6175b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6175b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6175b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6175b-116">Not supported.</span></span>|
|<span data-ttu-id="6175b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6175b-117">Application</span></span>|<span data-ttu-id="6175b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6175b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6175b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6175b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="6175b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6175b-120">Request headers</span></span>
|<span data-ttu-id="6175b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6175b-121">Header</span></span>|<span data-ttu-id="6175b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6175b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6175b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6175b-123">Authorization</span></span>|<span data-ttu-id="6175b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6175b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6175b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6175b-125">Accept</span></span>|<span data-ttu-id="6175b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6175b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6175b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6175b-127">Request body</span></span>
<span data-ttu-id="6175b-128">В тексте запроса добавьте представление объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6175b-128">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="6175b-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="6175b-129">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="6175b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6175b-130">Property</span></span>|<span data-ttu-id="6175b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6175b-131">Type</span></span>|<span data-ttu-id="6175b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6175b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6175b-133">accountId</span><span class="sxs-lookup"><span data-stu-id="6175b-133">accountId</span></span>|<span data-ttu-id="6175b-134">String</span><span class="sxs-lookup"><span data-stu-id="6175b-134">String</span></span>|<span data-ttu-id="6175b-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="6175b-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="6175b-136">id</span><span class="sxs-lookup"><span data-stu-id="6175b-136">id</span></span>|<span data-ttu-id="6175b-137">String</span><span class="sxs-lookup"><span data-stu-id="6175b-137">String</span></span>|<span data-ttu-id="6175b-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="6175b-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="6175b-139">displayName</span><span class="sxs-lookup"><span data-stu-id="6175b-139">displayName</span></span>|<span data-ttu-id="6175b-140">String</span><span class="sxs-lookup"><span data-stu-id="6175b-140">String</span></span>|<span data-ttu-id="6175b-141">Отображаемое имя профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="6175b-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="6175b-142">описание</span><span class="sxs-lookup"><span data-stu-id="6175b-142">description</span></span>|<span data-ttu-id="6175b-143">String</span><span class="sxs-lookup"><span data-stu-id="6175b-143">String</span></span>|<span data-ttu-id="6175b-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="6175b-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="6175b-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6175b-145">createdDateTime</span></span>|<span data-ttu-id="6175b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6175b-146">DateTimeOffset</span></span>|<span data-ttu-id="6175b-147">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="6175b-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="6175b-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6175b-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6175b-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6175b-149">DateTimeOffset</span></span>|<span data-ttu-id="6175b-150">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="6175b-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="6175b-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="6175b-151">tokenValue</span></span>|<span data-ttu-id="6175b-152">String</span><span class="sxs-lookup"><span data-stu-id="6175b-152">String</span></span>|<span data-ttu-id="6175b-153">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="6175b-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="6175b-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6175b-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="6175b-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6175b-155">DateTimeOffset</span></span>|<span data-ttu-id="6175b-156">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="6175b-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="6175b-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6175b-157">enrolledDeviceCount</span></span>|<span data-ttu-id="6175b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="6175b-158">Int32</span></span>|<span data-ttu-id="6175b-159">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="6175b-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="6175b-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="6175b-160">qrCodeContent</span></span>|<span data-ttu-id="6175b-161">String</span><span class="sxs-lookup"><span data-stu-id="6175b-161">String</span></span>|<span data-ttu-id="6175b-162">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="6175b-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="6175b-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="6175b-163">qrCodeImage</span></span>|[<span data-ttu-id="6175b-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6175b-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6175b-165">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="6175b-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="6175b-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="6175b-166">Response</span></span>
<span data-ttu-id="6175b-167">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6175b-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6175b-168">Пример</span><span class="sxs-lookup"><span data-stu-id="6175b-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="6175b-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="6175b-169">Request</span></span>
<span data-ttu-id="6175b-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6175b-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
Content-type: application/json
Content-length: 490

{
  "accountId": "Account Id value",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="6175b-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="6175b-171">Response</span></span>
<span data-ttu-id="6175b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6175b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





