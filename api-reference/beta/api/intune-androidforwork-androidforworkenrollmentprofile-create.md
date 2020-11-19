---
title: Create androidForWorkEnrollmentProfile
description: Создание объекта androidForWorkEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff6a33bd42d9edcaff5fd39c2757337e71b32a1b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255015"
---
# <a name="create-androidforworkenrollmentprofile"></a><span data-ttu-id="0cd84-103">Create androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="0cd84-103">Create androidForWorkEnrollmentProfile</span></span>

<span data-ttu-id="0cd84-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cd84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cd84-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cd84-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cd84-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0cd84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cd84-107">Создание объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="0cd84-107">Create a new [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cd84-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0cd84-108">Prerequisites</span></span>
<span data-ttu-id="0cd84-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cd84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cd84-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cd84-111">Permission type</span></span>|<span data-ttu-id="0cd84-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cd84-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cd84-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cd84-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0cd84-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cd84-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0cd84-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cd84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cd84-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cd84-116">Not supported.</span></span>|
|<span data-ttu-id="0cd84-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0cd84-117">Application</span></span>|<span data-ttu-id="0cd84-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cd84-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cd84-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cd84-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="0cd84-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0cd84-120">Request headers</span></span>
|<span data-ttu-id="0cd84-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0cd84-121">Header</span></span>|<span data-ttu-id="0cd84-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0cd84-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cd84-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0cd84-123">Authorization</span></span>|<span data-ttu-id="0cd84-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cd84-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cd84-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0cd84-125">Accept</span></span>|<span data-ttu-id="0cd84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0cd84-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cd84-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0cd84-127">Request body</span></span>
<span data-ttu-id="0cd84-128">В тексте запроса добавьте представление объекта androidForWorkEnrollmentProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cd84-128">In the request body, supply a JSON representation for the androidForWorkEnrollmentProfile object.</span></span>

<span data-ttu-id="0cd84-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта androidForWorkEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="0cd84-129">The following table shows the properties that are required when you create the androidForWorkEnrollmentProfile.</span></span>

|<span data-ttu-id="0cd84-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cd84-130">Property</span></span>|<span data-ttu-id="0cd84-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0cd84-131">Type</span></span>|<span data-ttu-id="0cd84-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0cd84-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cd84-133">accountId</span><span class="sxs-lookup"><span data-stu-id="0cd84-133">accountId</span></span>|<span data-ttu-id="0cd84-134">String</span><span class="sxs-lookup"><span data-stu-id="0cd84-134">String</span></span>|<span data-ttu-id="0cd84-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="0cd84-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="0cd84-136">id</span><span class="sxs-lookup"><span data-stu-id="0cd84-136">id</span></span>|<span data-ttu-id="0cd84-137">String</span><span class="sxs-lookup"><span data-stu-id="0cd84-137">String</span></span>|<span data-ttu-id="0cd84-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="0cd84-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="0cd84-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0cd84-139">displayName</span></span>|<span data-ttu-id="0cd84-140">String</span><span class="sxs-lookup"><span data-stu-id="0cd84-140">String</span></span>|<span data-ttu-id="0cd84-141">Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="0cd84-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="0cd84-142">description</span><span class="sxs-lookup"><span data-stu-id="0cd84-142">description</span></span>|<span data-ttu-id="0cd84-143">String</span><span class="sxs-lookup"><span data-stu-id="0cd84-143">String</span></span>|<span data-ttu-id="0cd84-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="0cd84-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="0cd84-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0cd84-145">createdDateTime</span></span>|<span data-ttu-id="0cd84-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cd84-146">DateTimeOffset</span></span>|<span data-ttu-id="0cd84-147">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="0cd84-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="0cd84-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0cd84-148">lastModifiedDateTime</span></span>|<span data-ttu-id="0cd84-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cd84-149">DateTimeOffset</span></span>|<span data-ttu-id="0cd84-150">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="0cd84-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="0cd84-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="0cd84-151">tokenValue</span></span>|<span data-ttu-id="0cd84-152">String</span><span class="sxs-lookup"><span data-stu-id="0cd84-152">String</span></span>|<span data-ttu-id="0cd84-153">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="0cd84-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="0cd84-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0cd84-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="0cd84-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cd84-155">DateTimeOffset</span></span>|<span data-ttu-id="0cd84-156">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="0cd84-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="0cd84-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0cd84-157">enrolledDeviceCount</span></span>|<span data-ttu-id="0cd84-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0cd84-158">Int32</span></span>|<span data-ttu-id="0cd84-159">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="0cd84-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="0cd84-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="0cd84-160">qrCodeContent</span></span>|<span data-ttu-id="0cd84-161">String</span><span class="sxs-lookup"><span data-stu-id="0cd84-161">String</span></span>|<span data-ttu-id="0cd84-162">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="0cd84-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="0cd84-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="0cd84-163">qrCodeImage</span></span>|[<span data-ttu-id="0cd84-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0cd84-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0cd84-165">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="0cd84-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="0cd84-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="0cd84-166">Response</span></span>
<span data-ttu-id="0cd84-167">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0cd84-167">If successful, this method returns a `201 Created` response code and a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cd84-168">Пример</span><span class="sxs-lookup"><span data-stu-id="0cd84-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cd84-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cd84-169">Request</span></span>
<span data-ttu-id="0cd84-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0cd84-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="0cd84-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cd84-171">Response</span></span>
<span data-ttu-id="0cd84-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0cd84-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




