---
title: Создание importedDeviceIdentity
description: Создание нового объекта importedDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e3a6ca16d9bfa4a79d723816544e9a7bcf3f77df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870527"
---
# <a name="create-importeddeviceidentity"></a><span data-ttu-id="20965-103">Создание importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="20965-103">Create importedDeviceIdentity</span></span>

> <span data-ttu-id="20965-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="20965-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20965-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20965-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20965-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="20965-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20965-107">Создание нового объекта [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="20965-107">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20965-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="20965-108">Prerequisites</span></span>
<span data-ttu-id="20965-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20965-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20965-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20965-111">Permission type</span></span>|<span data-ttu-id="20965-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20965-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20965-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20965-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20965-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20965-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="20965-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20965-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20965-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20965-116">Not supported.</span></span>|
|<span data-ttu-id="20965-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20965-117">Application</span></span>|<span data-ttu-id="20965-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20965-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20965-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20965-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="20965-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20965-120">Request headers</span></span>
|<span data-ttu-id="20965-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20965-121">Header</span></span>|<span data-ttu-id="20965-122">Значение</span><span class="sxs-lookup"><span data-stu-id="20965-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20965-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20965-123">Authorization</span></span>|<span data-ttu-id="20965-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="20965-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20965-125">Accept</span><span class="sxs-lookup"><span data-stu-id="20965-125">Accept</span></span>|<span data-ttu-id="20965-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20965-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20965-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="20965-127">Request body</span></span>
<span data-ttu-id="20965-128">В тексте запроса укажите представление JSON для объекта importedDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="20965-128">In the request body, supply a JSON representation for the importedDeviceIdentity object.</span></span>

<span data-ttu-id="20965-129">В следующей таблице показаны свойства, которые необходимы для создания importedDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="20965-129">The following table shows the properties that are required when you create the importedDeviceIdentity.</span></span>

|<span data-ttu-id="20965-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="20965-130">Property</span></span>|<span data-ttu-id="20965-131">Тип</span><span class="sxs-lookup"><span data-stu-id="20965-131">Type</span></span>|<span data-ttu-id="20965-132">Описание</span><span class="sxs-lookup"><span data-stu-id="20965-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20965-133">id</span><span class="sxs-lookup"><span data-stu-id="20965-133">id</span></span>|<span data-ttu-id="20965-134">Строка</span><span class="sxs-lookup"><span data-stu-id="20965-134">String</span></span>|<span data-ttu-id="20965-135">Идентификатор идентификатор импортированных устройства</span><span class="sxs-lookup"><span data-stu-id="20965-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="20965-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="20965-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="20965-137">Строка</span><span class="sxs-lookup"><span data-stu-id="20965-137">String</span></span>|<span data-ttu-id="20965-138">Идентификатор импортированных устройства</span><span class="sxs-lookup"><span data-stu-id="20965-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="20965-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="20965-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="20965-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="20965-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="20965-141">Тип удостоверения импортированных устройства.</span><span class="sxs-lookup"><span data-stu-id="20965-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="20965-142">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="20965-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="20965-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20965-143">lastModifiedDateTime</span></span>|<span data-ttu-id="20965-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20965-144">DateTimeOffset</span></span>|<span data-ttu-id="20965-145">Последние изменения даты и времени описания</span><span class="sxs-lookup"><span data-stu-id="20965-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="20965-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20965-146">createdDateTime</span></span>|<span data-ttu-id="20965-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20965-147">DateTimeOffset</span></span>|<span data-ttu-id="20965-148">Время создания даты устройства</span><span class="sxs-lookup"><span data-stu-id="20965-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="20965-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="20965-149">lastContactedDateTime</span></span>|<span data-ttu-id="20965-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20965-150">DateTimeOffset</span></span>|<span data-ttu-id="20965-151">Связаться с даты последнего устройства</span><span class="sxs-lookup"><span data-stu-id="20965-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="20965-152">описание</span><span class="sxs-lookup"><span data-stu-id="20965-152">description</span></span>|<span data-ttu-id="20965-153">Строка</span><span class="sxs-lookup"><span data-stu-id="20965-153">String</span></span>|<span data-ttu-id="20965-154">Описание устройства</span><span class="sxs-lookup"><span data-stu-id="20965-154">The description of the device</span></span>|
|<span data-ttu-id="20965-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="20965-155">enrollmentState</span></span>|[<span data-ttu-id="20965-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="20965-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="20965-157">Состояние устройства в Intune.</span><span class="sxs-lookup"><span data-stu-id="20965-157">The state of the device in Intune.</span></span> <span data-ttu-id="20965-158">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="20965-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="20965-159">platform</span><span class="sxs-lookup"><span data-stu-id="20965-159">platform</span></span>|[<span data-ttu-id="20965-160">Платформа</span><span class="sxs-lookup"><span data-stu-id="20965-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="20965-161">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="20965-161">The platform of the Device.</span></span> <span data-ttu-id="20965-162">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="20965-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|



## <a name="response"></a><span data-ttu-id="20965-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="20965-163">Response</span></span>
<span data-ttu-id="20965-164">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="20965-164">If successful, this method returns a `201 Created` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20965-165">Пример</span><span class="sxs-lookup"><span data-stu-id="20965-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="20965-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="20965-166">Request</span></span>
<span data-ttu-id="20965-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20965-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
Content-type: application/json
Content-length: 396

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```

### <a name="response"></a><span data-ttu-id="20965-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="20965-168">Response</span></span>
<span data-ttu-id="20965-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="20965-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios"
}
```





