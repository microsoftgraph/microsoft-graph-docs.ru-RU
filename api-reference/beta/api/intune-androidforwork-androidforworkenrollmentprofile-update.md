---
title: Обновление объекта androidForWorkEnrollmentProfile
description: Обновление свойств объекта androidForWorkEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 98d017ca961a012c195e1e729bf4a2527e50f5e0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398018"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="0f25e-103">Обновление объекта androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="0f25e-103">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="0f25e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0f25e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0f25e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f25e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f25e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f25e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f25e-107">Обновление свойств объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="0f25e-107">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f25e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0f25e-108">Prerequisites</span></span>
<span data-ttu-id="0f25e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0f25e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0f25e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f25e-111">Permission type</span></span>|<span data-ttu-id="0f25e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f25e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f25e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f25e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f25e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f25e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0f25e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f25e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f25e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f25e-116">Not supported.</span></span>|
|<span data-ttu-id="0f25e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f25e-117">Application</span></span>|<span data-ttu-id="0f25e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f25e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f25e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f25e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="0f25e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f25e-120">Request headers</span></span>
|<span data-ttu-id="0f25e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f25e-121">Header</span></span>|<span data-ttu-id="0f25e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0f25e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f25e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f25e-123">Authorization</span></span>|<span data-ttu-id="0f25e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0f25e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f25e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0f25e-125">Accept</span></span>|<span data-ttu-id="0f25e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f25e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f25e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f25e-127">Request body</span></span>
<span data-ttu-id="0f25e-128">В тексте запроса добавьте представление объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f25e-128">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="0f25e-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="0f25e-129">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="0f25e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f25e-130">Property</span></span>|<span data-ttu-id="0f25e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0f25e-131">Type</span></span>|<span data-ttu-id="0f25e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0f25e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f25e-133">accountId</span><span class="sxs-lookup"><span data-stu-id="0f25e-133">accountId</span></span>|<span data-ttu-id="0f25e-134">String</span><span class="sxs-lookup"><span data-stu-id="0f25e-134">String</span></span>|<span data-ttu-id="0f25e-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="0f25e-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="0f25e-136">id</span><span class="sxs-lookup"><span data-stu-id="0f25e-136">id</span></span>|<span data-ttu-id="0f25e-137">String</span><span class="sxs-lookup"><span data-stu-id="0f25e-137">String</span></span>|<span data-ttu-id="0f25e-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="0f25e-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="0f25e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0f25e-139">displayName</span></span>|<span data-ttu-id="0f25e-140">String</span><span class="sxs-lookup"><span data-stu-id="0f25e-140">String</span></span>|<span data-ttu-id="0f25e-141">Отображаемое имя профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="0f25e-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="0f25e-142">description</span><span class="sxs-lookup"><span data-stu-id="0f25e-142">description</span></span>|<span data-ttu-id="0f25e-143">String</span><span class="sxs-lookup"><span data-stu-id="0f25e-143">String</span></span>|<span data-ttu-id="0f25e-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="0f25e-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="0f25e-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f25e-145">createdDateTime</span></span>|<span data-ttu-id="0f25e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f25e-146">DateTimeOffset</span></span>|<span data-ttu-id="0f25e-147">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="0f25e-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="0f25e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f25e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="0f25e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f25e-149">DateTimeOffset</span></span>|<span data-ttu-id="0f25e-150">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="0f25e-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="0f25e-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="0f25e-151">tokenValue</span></span>|<span data-ttu-id="0f25e-152">String</span><span class="sxs-lookup"><span data-stu-id="0f25e-152">String</span></span>|<span data-ttu-id="0f25e-153">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="0f25e-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="0f25e-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0f25e-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="0f25e-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f25e-155">DateTimeOffset</span></span>|<span data-ttu-id="0f25e-156">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="0f25e-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="0f25e-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0f25e-157">enrolledDeviceCount</span></span>|<span data-ttu-id="0f25e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0f25e-158">Int32</span></span>|<span data-ttu-id="0f25e-159">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="0f25e-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="0f25e-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="0f25e-160">qrCodeContent</span></span>|<span data-ttu-id="0f25e-161">String</span><span class="sxs-lookup"><span data-stu-id="0f25e-161">String</span></span>|<span data-ttu-id="0f25e-162">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="0f25e-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="0f25e-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="0f25e-163">qrCodeImage</span></span>|[<span data-ttu-id="0f25e-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0f25e-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0f25e-165">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="0f25e-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="0f25e-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f25e-166">Response</span></span>
<span data-ttu-id="0f25e-167">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0f25e-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f25e-168">Пример</span><span class="sxs-lookup"><span data-stu-id="0f25e-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f25e-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f25e-169">Request</span></span>
<span data-ttu-id="0f25e-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f25e-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0f25e-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f25e-171">Response</span></span>
<span data-ttu-id="0f25e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0f25e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




