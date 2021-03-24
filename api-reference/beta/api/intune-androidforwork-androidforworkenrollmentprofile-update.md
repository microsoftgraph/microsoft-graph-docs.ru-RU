---
title: Обновление объекта androidForWorkEnrollmentProfile
description: Обновление свойств объекта androidForWorkEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1e2011dc33af2450fe5fe63492167973269441c0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144706"
---
# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="c9caf-103">Обновление объекта androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="c9caf-103">Update androidForWorkEnrollmentProfile</span></span>

<span data-ttu-id="c9caf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9caf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9caf-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9caf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9caf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9caf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9caf-107">Обновление свойств объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="c9caf-107">Update the properties of a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9caf-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c9caf-108">Prerequisites</span></span>
<span data-ttu-id="c9caf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9caf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9caf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9caf-111">Permission type</span></span>|<span data-ttu-id="c9caf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9caf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9caf-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9caf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9caf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9caf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9caf-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9caf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9caf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9caf-116">Not supported.</span></span>|
|<span data-ttu-id="c9caf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c9caf-117">Application</span></span>|<span data-ttu-id="c9caf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9caf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9caf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9caf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="c9caf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c9caf-120">Request headers</span></span>
|<span data-ttu-id="c9caf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9caf-121">Header</span></span>|<span data-ttu-id="c9caf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c9caf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9caf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9caf-123">Authorization</span></span>|<span data-ttu-id="c9caf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9caf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9caf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c9caf-125">Accept</span></span>|<span data-ttu-id="c9caf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9caf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9caf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9caf-127">Request body</span></span>
<span data-ttu-id="c9caf-128">В тексте запроса добавьте представление объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9caf-128">In the request body, supply a JSON representation for the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="c9caf-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="c9caf-129">The following table shows the properties that are required when you create the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span></span>

|<span data-ttu-id="c9caf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9caf-130">Property</span></span>|<span data-ttu-id="c9caf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c9caf-131">Type</span></span>|<span data-ttu-id="c9caf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c9caf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9caf-133">accountId</span><span class="sxs-lookup"><span data-stu-id="c9caf-133">accountId</span></span>|<span data-ttu-id="c9caf-134">String</span><span class="sxs-lookup"><span data-stu-id="c9caf-134">String</span></span>|<span data-ttu-id="c9caf-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="c9caf-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="c9caf-136">id</span><span class="sxs-lookup"><span data-stu-id="c9caf-136">id</span></span>|<span data-ttu-id="c9caf-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c9caf-137">String</span></span>|<span data-ttu-id="c9caf-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="c9caf-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="c9caf-139">displayName</span><span class="sxs-lookup"><span data-stu-id="c9caf-139">displayName</span></span>|<span data-ttu-id="c9caf-140">Строка</span><span class="sxs-lookup"><span data-stu-id="c9caf-140">String</span></span>|<span data-ttu-id="c9caf-141">Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="c9caf-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="c9caf-142">description</span><span class="sxs-lookup"><span data-stu-id="c9caf-142">description</span></span>|<span data-ttu-id="c9caf-143">Строка</span><span class="sxs-lookup"><span data-stu-id="c9caf-143">String</span></span>|<span data-ttu-id="c9caf-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="c9caf-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="c9caf-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9caf-145">createdDateTime</span></span>|<span data-ttu-id="c9caf-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9caf-146">DateTimeOffset</span></span>|<span data-ttu-id="c9caf-147">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="c9caf-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="c9caf-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9caf-148">lastModifiedDateTime</span></span>|<span data-ttu-id="c9caf-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9caf-149">DateTimeOffset</span></span>|<span data-ttu-id="c9caf-150">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="c9caf-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="c9caf-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="c9caf-151">tokenValue</span></span>|<span data-ttu-id="c9caf-152">String</span><span class="sxs-lookup"><span data-stu-id="c9caf-152">String</span></span>|<span data-ttu-id="c9caf-153">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="c9caf-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="c9caf-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c9caf-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="c9caf-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9caf-155">DateTimeOffset</span></span>|<span data-ttu-id="c9caf-156">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="c9caf-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="c9caf-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c9caf-157">enrolledDeviceCount</span></span>|<span data-ttu-id="c9caf-158">Int32</span><span class="sxs-lookup"><span data-stu-id="c9caf-158">Int32</span></span>|<span data-ttu-id="c9caf-159">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="c9caf-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="c9caf-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="c9caf-160">qrCodeContent</span></span>|<span data-ttu-id="c9caf-161">String</span><span class="sxs-lookup"><span data-stu-id="c9caf-161">String</span></span>|<span data-ttu-id="c9caf-162">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="c9caf-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="c9caf-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="c9caf-163">qrCodeImage</span></span>|[<span data-ttu-id="c9caf-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c9caf-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c9caf-165">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="c9caf-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="c9caf-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9caf-166">Response</span></span>
<span data-ttu-id="c9caf-167">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9caf-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9caf-168">Пример</span><span class="sxs-lookup"><span data-stu-id="c9caf-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9caf-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9caf-169">Request</span></span>
<span data-ttu-id="c9caf-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9caf-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c9caf-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9caf-171">Response</span></span>
<span data-ttu-id="c9caf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9caf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




