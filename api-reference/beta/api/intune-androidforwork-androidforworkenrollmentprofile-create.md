---
title: Create androidForWorkEnrollmentProfile
description: Создание объекта androidForWorkEnrollmentProfile.
author: tfitzmac
ms.openlocfilehash: 794179968afc4f39c809373b3425c076f7a591a3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355978"
---
# <a name="create-androidforworkenrollmentprofile"></a><span data-ttu-id="f1b57-103">Create androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="f1b57-103">Create androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="f1b57-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f1b57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1b57-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1b57-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1b57-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f1b57-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1b57-107">Создание объекта [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f1b57-107">Create a new [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1b57-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f1b57-108">Prerequisites</span></span>
<span data-ttu-id="f1b57-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1b57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1b57-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1b57-111">Permission type</span></span>|<span data-ttu-id="f1b57-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1b57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1b57-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1b57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1b57-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1b57-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1b57-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1b57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1b57-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1b57-116">Not supported.</span></span>|
|<span data-ttu-id="f1b57-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1b57-117">Application</span></span>|<span data-ttu-id="f1b57-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1b57-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1b57-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1b57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="f1b57-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1b57-120">Request headers</span></span>
|<span data-ttu-id="f1b57-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1b57-121">Header</span></span>|<span data-ttu-id="f1b57-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f1b57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1b57-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1b57-123">Authorization</span></span>|<span data-ttu-id="f1b57-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f1b57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1b57-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f1b57-125">Accept</span></span>|<span data-ttu-id="f1b57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1b57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1b57-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1b57-127">Request body</span></span>
<span data-ttu-id="f1b57-128">В тексте запроса добавьте представление объекта androidForWorkEnrollmentProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1b57-128">In the request body, supply a JSON representation for the androidForWorkEnrollmentProfile object.</span></span>

<span data-ttu-id="f1b57-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта androidForWorkEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="f1b57-129">The following table shows the properties that are required when you create the androidForWorkEnrollmentProfile.</span></span>

|<span data-ttu-id="f1b57-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1b57-130">Property</span></span>|<span data-ttu-id="f1b57-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f1b57-131">Type</span></span>|<span data-ttu-id="f1b57-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f1b57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1b57-133">accountId</span><span class="sxs-lookup"><span data-stu-id="f1b57-133">accountId</span></span>|<span data-ttu-id="f1b57-134">String</span><span class="sxs-lookup"><span data-stu-id="f1b57-134">String</span></span>|<span data-ttu-id="f1b57-135">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="f1b57-135">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="f1b57-136">id</span><span class="sxs-lookup"><span data-stu-id="f1b57-136">id</span></span>|<span data-ttu-id="f1b57-137">String</span><span class="sxs-lookup"><span data-stu-id="f1b57-137">String</span></span>|<span data-ttu-id="f1b57-138">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="f1b57-138">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="f1b57-139">displayName</span><span class="sxs-lookup"><span data-stu-id="f1b57-139">displayName</span></span>|<span data-ttu-id="f1b57-140">String</span><span class="sxs-lookup"><span data-stu-id="f1b57-140">String</span></span>|<span data-ttu-id="f1b57-141">Отображаемое имя профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="f1b57-141">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="f1b57-142">описание</span><span class="sxs-lookup"><span data-stu-id="f1b57-142">description</span></span>|<span data-ttu-id="f1b57-143">String</span><span class="sxs-lookup"><span data-stu-id="f1b57-143">String</span></span>|<span data-ttu-id="f1b57-144">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="f1b57-144">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="f1b57-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1b57-145">createdDateTime</span></span>|<span data-ttu-id="f1b57-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1b57-146">DateTimeOffset</span></span>|<span data-ttu-id="f1b57-147">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="f1b57-147">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="f1b57-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1b57-148">lastModifiedDateTime</span></span>|<span data-ttu-id="f1b57-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1b57-149">DateTimeOffset</span></span>|<span data-ttu-id="f1b57-150">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="f1b57-150">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="f1b57-151">tokenValue</span><span class="sxs-lookup"><span data-stu-id="f1b57-151">tokenValue</span></span>|<span data-ttu-id="f1b57-152">String</span><span class="sxs-lookup"><span data-stu-id="f1b57-152">String</span></span>|<span data-ttu-id="f1b57-153">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="f1b57-153">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="f1b57-154">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f1b57-154">tokenExpirationDateTime</span></span>|<span data-ttu-id="f1b57-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1b57-155">DateTimeOffset</span></span>|<span data-ttu-id="f1b57-156">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="f1b57-156">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="f1b57-157">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f1b57-157">enrolledDeviceCount</span></span>|<span data-ttu-id="f1b57-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f1b57-158">Int32</span></span>|<span data-ttu-id="f1b57-159">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="f1b57-159">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="f1b57-160">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="f1b57-160">qrCodeContent</span></span>|<span data-ttu-id="f1b57-161">String</span><span class="sxs-lookup"><span data-stu-id="f1b57-161">String</span></span>|<span data-ttu-id="f1b57-162">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="f1b57-162">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="f1b57-163">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="f1b57-163">qrCodeImage</span></span>|[<span data-ttu-id="f1b57-164">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f1b57-164">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f1b57-165">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="f1b57-165">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="f1b57-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1b57-166">Response</span></span>
<span data-ttu-id="f1b57-167">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f1b57-167">If successful, this method returns a `201 Created` response code and a [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1b57-168">Пример</span><span class="sxs-lookup"><span data-stu-id="f1b57-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1b57-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1b57-169">Request</span></span>
<span data-ttu-id="f1b57-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1b57-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles
Content-type: application/json
Content-length: 560

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
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

### <a name="response"></a><span data-ttu-id="f1b57-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1b57-171">Response</span></span>
<span data-ttu-id="f1b57-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f1b57-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





