---
title: Обновление importedDeviceIdentityResult
description: Обновление свойства объекта importedDeviceIdentityResult.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 09b43ba66bfc299169ae1b206fc96301d62c6a09
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930350"
---
# <a name="update-importeddeviceidentityresult"></a><span data-ttu-id="b407b-103">Обновление importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="b407b-103">Update importedDeviceIdentityResult</span></span>

> <span data-ttu-id="b407b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b407b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b407b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b407b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b407b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b407b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b407b-107">Обновление свойства объекта [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="b407b-107">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b407b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b407b-108">Prerequisites</span></span>
<span data-ttu-id="b407b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b407b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b407b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b407b-111">Permission type</span></span>|<span data-ttu-id="b407b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b407b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b407b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b407b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b407b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b407b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b407b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b407b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b407b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b407b-116">Not supported.</span></span>|
|<span data-ttu-id="b407b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b407b-117">Application</span></span>|<span data-ttu-id="b407b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b407b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b407b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b407b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="b407b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b407b-120">Request headers</span></span>
|<span data-ttu-id="b407b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b407b-121">Header</span></span>|<span data-ttu-id="b407b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b407b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b407b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b407b-123">Authorization</span></span>|<span data-ttu-id="b407b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b407b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b407b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b407b-125">Accept</span></span>|<span data-ttu-id="b407b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b407b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b407b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b407b-127">Request body</span></span>
<span data-ttu-id="b407b-128">В тексте запроса укажите представление JSON для объекта [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .</span><span class="sxs-lookup"><span data-stu-id="b407b-128">In the request body, supply a JSON representation for the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>

<span data-ttu-id="b407b-129">В следующей таблице показаны свойства, которые необходимы для создания [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span><span class="sxs-lookup"><span data-stu-id="b407b-129">The following table shows the properties that are required when you create the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>

|<span data-ttu-id="b407b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b407b-130">Property</span></span>|<span data-ttu-id="b407b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b407b-131">Type</span></span>|<span data-ttu-id="b407b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b407b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b407b-133">id</span><span class="sxs-lookup"><span data-stu-id="b407b-133">id</span></span>|<span data-ttu-id="b407b-134">String</span><span class="sxs-lookup"><span data-stu-id="b407b-134">String</span></span>|<span data-ttu-id="b407b-135">Идентификатор identity импортированных устройства унаследованные от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="b407b-135">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="b407b-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b407b-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="b407b-137">String</span><span class="sxs-lookup"><span data-stu-id="b407b-137">String</span></span>|<span data-ttu-id="b407b-138">Импортированные устройства идентификатор наследуется от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="b407b-138">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="b407b-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="b407b-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="b407b-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="b407b-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="b407b-141">Тип импорта наследуется идентификатор устройства из [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="b407b-141">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="b407b-142">Возможные значения: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="b407b-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="b407b-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b407b-143">lastModifiedDateTime</span></span>|<span data-ttu-id="b407b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b407b-144">DateTimeOffset</span></span>|<span data-ttu-id="b407b-145">Последние изменения даты и времени описания унаследованные от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="b407b-145">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="b407b-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b407b-146">createdDateTime</span></span>|<span data-ttu-id="b407b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b407b-147">DateTimeOffset</span></span>|<span data-ttu-id="b407b-148">Созданные Дата и время устройства унаследованные от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="b407b-148">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="b407b-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="b407b-149">lastContactedDateTime</span></span>|<span data-ttu-id="b407b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b407b-150">DateTimeOffset</span></span>|<span data-ttu-id="b407b-151">Связаться с даты последнего устройства, унаследованные от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="b407b-151">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="b407b-152">описание</span><span class="sxs-lookup"><span data-stu-id="b407b-152">description</span></span>|<span data-ttu-id="b407b-153">String</span><span class="sxs-lookup"><span data-stu-id="b407b-153">String</span></span>|<span data-ttu-id="b407b-154">Описание устройства унаследованные от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="b407b-154">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="b407b-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="b407b-155">enrollmentState</span></span>|[<span data-ttu-id="b407b-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="b407b-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="b407b-157">Состояние устройства в Intune наследуется от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="b407b-157">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="b407b-158">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="b407b-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="b407b-159">platform</span><span class="sxs-lookup"><span data-stu-id="b407b-159">platform</span></span>|[<span data-ttu-id="b407b-160">Платформа</span><span class="sxs-lookup"><span data-stu-id="b407b-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="b407b-161">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="b407b-161">The platform of the Device.</span></span> <span data-ttu-id="b407b-162">Наследуется от [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="b407b-162">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="b407b-163">Возможные значения: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="b407b-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="b407b-164">status</span><span class="sxs-lookup"><span data-stu-id="b407b-164">status</span></span>|<span data-ttu-id="b407b-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="b407b-165">Boolean</span></span>|<span data-ttu-id="b407b-166">Состояние импортированных устройств удостоверений</span><span class="sxs-lookup"><span data-stu-id="b407b-166">Status of imported device identity</span></span>|



## <a name="response"></a><span data-ttu-id="b407b-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="b407b-167">Response</span></span>
<span data-ttu-id="b407b-168">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b407b-168">If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b407b-169">Пример</span><span class="sxs-lookup"><span data-stu-id="b407b-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="b407b-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="b407b-170">Request</span></span>
<span data-ttu-id="b407b-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b407b-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 354

{
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a><span data-ttu-id="b407b-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="b407b-172">Response</span></span>
<span data-ttu-id="b407b-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b407b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```





