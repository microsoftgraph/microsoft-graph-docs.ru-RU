---
title: Обновление объекта androidForWorkEnrollmentProfile
description: Обновление свойств объекта androidForWorkEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5c65c01996ce482d7456396fd831a9ab2aa465b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916210"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="e7b0c-103">Обновление объекта androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e7b0c-103">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="e7b0c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7b0c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7b0c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7b0c-107">Обновление свойств объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e7b0c-107">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7b0c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e7b0c-108">Prerequisites</span></span>
<span data-ttu-id="e7b0c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7b0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7b0c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7b0c-111">Permission type</span></span>|<span data-ttu-id="e7b0c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7b0c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7b0c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7b0c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7b0c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7b0c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7b0c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7b0c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7b0c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-116">Not supported.</span></span>|
|<span data-ttu-id="e7b0c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7b0c-117">Application</span></span>|<span data-ttu-id="e7b0c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7b0c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7b0c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="e7b0c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7b0c-120">Request headers</span></span>
|<span data-ttu-id="e7b0c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7b0c-121">Header</span></span>|<span data-ttu-id="e7b0c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e7b0c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7b0c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7b0c-123">Authorization</span></span>|<span data-ttu-id="e7b0c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e7b0c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7b0c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e7b0c-125">Accept</span></span>|<span data-ttu-id="e7b0c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7b0c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7b0c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7b0c-127">Request body</span></span>
<span data-ttu-id="e7b0c-128">В тексте запроса добавьте представление объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-128">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="e7b0c-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e7b0c-129">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="e7b0c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7b0c-130">Property</span></span>|<span data-ttu-id="e7b0c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e7b0c-131">Type</span></span>|<span data-ttu-id="e7b0c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e7b0c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7b0c-133">accountId</span><span class="sxs-lookup"><span data-stu-id="e7b0c-133">accountId</span></span>|<span data-ttu-id="e7b0c-134">String</span><span class="sxs-lookup"><span data-stu-id="e7b0c-134">String</span></span>|<span data-ttu-id="e7b0c-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="e7b0c-136">id</span><span class="sxs-lookup"><span data-stu-id="e7b0c-136">id</span></span>|<span data-ttu-id="e7b0c-137">String</span><span class="sxs-lookup"><span data-stu-id="e7b0c-137">String</span></span>|<span data-ttu-id="e7b0c-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="e7b0c-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e7b0c-139">displayName</span></span>|<span data-ttu-id="e7b0c-140">String</span><span class="sxs-lookup"><span data-stu-id="e7b0c-140">String</span></span>|<span data-ttu-id="e7b0c-141">Отображаемое имя профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="e7b0c-142">описание</span><span class="sxs-lookup"><span data-stu-id="e7b0c-142">description</span></span>|<span data-ttu-id="e7b0c-143">String</span><span class="sxs-lookup"><span data-stu-id="e7b0c-143">String</span></span>|<span data-ttu-id="e7b0c-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="e7b0c-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7b0c-145">createdDateTime</span></span>|<span data-ttu-id="e7b0c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7b0c-146">DateTimeOffset</span></span>|<span data-ttu-id="e7b0c-147">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="e7b0c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7b0c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="e7b0c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7b0c-149">DateTimeOffset</span></span>|<span data-ttu-id="e7b0c-150">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="e7b0c-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="e7b0c-151">tokenValue</span></span>|<span data-ttu-id="e7b0c-152">String</span><span class="sxs-lookup"><span data-stu-id="e7b0c-152">String</span></span>|<span data-ttu-id="e7b0c-153">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="e7b0c-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e7b0c-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="e7b0c-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7b0c-155">DateTimeOffset</span></span>|<span data-ttu-id="e7b0c-156">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="e7b0c-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e7b0c-157">enrolledDeviceCount</span></span>|<span data-ttu-id="e7b0c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e7b0c-158">Int32</span></span>|<span data-ttu-id="e7b0c-159">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="e7b0c-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="e7b0c-160">qrCodeContent</span></span>|<span data-ttu-id="e7b0c-161">String</span><span class="sxs-lookup"><span data-stu-id="e7b0c-161">String</span></span>|<span data-ttu-id="e7b0c-162">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="e7b0c-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="e7b0c-163">qrCodeImage</span></span>|[<span data-ttu-id="e7b0c-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e7b0c-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e7b0c-165">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="e7b0c-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7b0c-166">Response</span></span>
<span data-ttu-id="e7b0c-167">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7b0c-168">Пример</span><span class="sxs-lookup"><span data-stu-id="e7b0c-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7b0c-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7b0c-169">Request</span></span>
<span data-ttu-id="e7b0c-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e7b0c-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7b0c-171">Response</span></span>
<span data-ttu-id="e7b0c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e7b0c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





