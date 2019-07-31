---
title: Обновление объекта androidForWorkEnrollmentProfile
description: Обновление свойств объекта androidForWorkEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: abd3fc0112f54989c0e1264150fe59ca1367e628
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952739"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="8ba1c-103">Обновление объекта androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="8ba1c-103">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="8ba1c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ba1c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ba1c-106">Обновление свойств объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="8ba1c-106">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ba1c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8ba1c-107">Prerequisites</span></span>
<span data-ttu-id="8ba1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ba1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ba1c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ba1c-110">Permission type</span></span>|<span data-ttu-id="8ba1c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ba1c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ba1c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ba1c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8ba1c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ba1c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ba1c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ba1c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ba1c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-115">Not supported.</span></span>|
|<span data-ttu-id="8ba1c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ba1c-116">Application</span></span>|<span data-ttu-id="8ba1c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ba1c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ba1c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="8ba1c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ba1c-119">Request headers</span></span>
|<span data-ttu-id="8ba1c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ba1c-120">Header</span></span>|<span data-ttu-id="8ba1c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8ba1c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ba1c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ba1c-122">Authorization</span></span>|<span data-ttu-id="8ba1c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ba1c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8ba1c-124">Accept</span></span>|<span data-ttu-id="8ba1c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8ba1c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ba1c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ba1c-126">Request body</span></span>
<span data-ttu-id="8ba1c-127">В тексте запроса добавьте представление объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-127">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="8ba1c-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="8ba1c-128">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="8ba1c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ba1c-129">Property</span></span>|<span data-ttu-id="8ba1c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8ba1c-130">Type</span></span>|<span data-ttu-id="8ba1c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8ba1c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ba1c-132">accountId</span><span class="sxs-lookup"><span data-stu-id="8ba1c-132">accountId</span></span>|<span data-ttu-id="8ba1c-133">String</span><span class="sxs-lookup"><span data-stu-id="8ba1c-133">String</span></span>|<span data-ttu-id="8ba1c-134">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-134">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="8ba1c-135">id</span><span class="sxs-lookup"><span data-stu-id="8ba1c-135">id</span></span>|<span data-ttu-id="8ba1c-136">Строка</span><span class="sxs-lookup"><span data-stu-id="8ba1c-136">String</span></span>|<span data-ttu-id="8ba1c-137">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-137">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="8ba1c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="8ba1c-138">displayName</span></span>|<span data-ttu-id="8ba1c-139">Строка</span><span class="sxs-lookup"><span data-stu-id="8ba1c-139">String</span></span>|<span data-ttu-id="8ba1c-140">Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="8ba1c-141">description</span><span class="sxs-lookup"><span data-stu-id="8ba1c-141">description</span></span>|<span data-ttu-id="8ba1c-142">String</span><span class="sxs-lookup"><span data-stu-id="8ba1c-142">String</span></span>|<span data-ttu-id="8ba1c-143">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="8ba1c-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ba1c-144">createdDateTime</span></span>|<span data-ttu-id="8ba1c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ba1c-145">DateTimeOffset</span></span>|<span data-ttu-id="8ba1c-146">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="8ba1c-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ba1c-147">lastModifiedDateTime</span></span>|<span data-ttu-id="8ba1c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ba1c-148">DateTimeOffset</span></span>|<span data-ttu-id="8ba1c-149">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-149">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="8ba1c-150">tokenValue</span><span class="sxs-lookup"><span data-stu-id="8ba1c-150">tokenValue</span></span>|<span data-ttu-id="8ba1c-151">String</span><span class="sxs-lookup"><span data-stu-id="8ba1c-151">String</span></span>|<span data-ttu-id="8ba1c-152">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-152">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="8ba1c-153">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8ba1c-153">tokenExpirationDateTime</span></span>|<span data-ttu-id="8ba1c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ba1c-154">DateTimeOffset</span></span>|<span data-ttu-id="8ba1c-155">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-155">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="8ba1c-156">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8ba1c-156">enrolledDeviceCount</span></span>|<span data-ttu-id="8ba1c-157">Int32</span><span class="sxs-lookup"><span data-stu-id="8ba1c-157">Int32</span></span>|<span data-ttu-id="8ba1c-158">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-158">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="8ba1c-159">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="8ba1c-159">qrCodeContent</span></span>|<span data-ttu-id="8ba1c-160">String</span><span class="sxs-lookup"><span data-stu-id="8ba1c-160">String</span></span>|<span data-ttu-id="8ba1c-161">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-161">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="8ba1c-162">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="8ba1c-162">qrCodeImage</span></span>|[<span data-ttu-id="8ba1c-163">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8ba1c-163">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8ba1c-164">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-164">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="8ba1c-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ba1c-165">Response</span></span>
<span data-ttu-id="8ba1c-166">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-166">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ba1c-167">Пример</span><span class="sxs-lookup"><span data-stu-id="8ba1c-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ba1c-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ba1c-168">Request</span></span>
<span data-ttu-id="8ba1c-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8ba1c-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ba1c-170">Response</span></span>
<span data-ttu-id="8ba1c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ba1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





