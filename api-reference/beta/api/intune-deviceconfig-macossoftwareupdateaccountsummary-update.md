---
title: Обновление Макоссофтвареупдатеаккаунтсуммари
description: Обновление свойств объекта Макоссофтвареупдатеаккаунтсуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 29ca1b5e3028abf3fd48e77501b7e02389963240
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731836"
---
# <a name="update-macossoftwareupdateaccountsummary"></a><span data-ttu-id="85270-103">Обновление Макоссофтвареупдатеаккаунтсуммари</span><span class="sxs-lookup"><span data-stu-id="85270-103">Update macOSSoftwareUpdateAccountSummary</span></span>

<span data-ttu-id="85270-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85270-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85270-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85270-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85270-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85270-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85270-107">Обновление свойств объекта [макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="85270-107">Update the properties of a [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85270-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="85270-108">Prerequisites</span></span>
<span data-ttu-id="85270-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85270-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85270-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85270-111">Permission type</span></span>|<span data-ttu-id="85270-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85270-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85270-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85270-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85270-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85270-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85270-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85270-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85270-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85270-116">Not supported.</span></span>|
|<span data-ttu-id="85270-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85270-117">Application</span></span>|<span data-ttu-id="85270-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85270-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85270-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85270-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="85270-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="85270-120">Request headers</span></span>
|<span data-ttu-id="85270-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85270-121">Header</span></span>|<span data-ttu-id="85270-122">Значение</span><span class="sxs-lookup"><span data-stu-id="85270-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85270-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85270-123">Authorization</span></span>|<span data-ttu-id="85270-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85270-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85270-125">Accept</span><span class="sxs-lookup"><span data-stu-id="85270-125">Accept</span></span>|<span data-ttu-id="85270-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85270-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85270-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85270-127">Request body</span></span>
<span data-ttu-id="85270-128">В тексте запроса добавьте представление объекта [макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85270-128">In the request body, supply a JSON representation for the [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object.</span></span>

<span data-ttu-id="85270-129">В следующей таблице приведены свойства, необходимые при создании [макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md).</span><span class="sxs-lookup"><span data-stu-id="85270-129">The following table shows the properties that are required when you create the [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md).</span></span>

|<span data-ttu-id="85270-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="85270-130">Property</span></span>|<span data-ttu-id="85270-131">Тип</span><span class="sxs-lookup"><span data-stu-id="85270-131">Type</span></span>|<span data-ttu-id="85270-132">Описание</span><span class="sxs-lookup"><span data-stu-id="85270-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85270-133">id</span><span class="sxs-lookup"><span data-stu-id="85270-133">id</span></span>|<span data-ttu-id="85270-134">Строка</span><span class="sxs-lookup"><span data-stu-id="85270-134">String</span></span>|<span data-ttu-id="85270-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="85270-135">Key of the entity.</span></span>|
|<span data-ttu-id="85270-136">displayName</span><span class="sxs-lookup"><span data-stu-id="85270-136">displayName</span></span>|<span data-ttu-id="85270-137">Строка</span><span class="sxs-lookup"><span data-stu-id="85270-137">String</span></span>|<span data-ttu-id="85270-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="85270-138">The name of the report</span></span>|
|<span data-ttu-id="85270-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="85270-139">deviceId</span></span>|<span data-ttu-id="85270-140">String</span><span class="sxs-lookup"><span data-stu-id="85270-140">String</span></span>|<span data-ttu-id="85270-141">ИДЕНТИФИКАТОР устройства.</span><span class="sxs-lookup"><span data-stu-id="85270-141">The device ID.</span></span>|
|<span data-ttu-id="85270-142">userId</span><span class="sxs-lookup"><span data-stu-id="85270-142">userId</span></span>|<span data-ttu-id="85270-143">String</span><span class="sxs-lookup"><span data-stu-id="85270-143">String</span></span>|<span data-ttu-id="85270-144">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="85270-144">The user ID.</span></span>|
|<span data-ttu-id="85270-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="85270-145">deviceName</span></span>|<span data-ttu-id="85270-146">String</span><span class="sxs-lookup"><span data-stu-id="85270-146">String</span></span>|<span data-ttu-id="85270-147">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="85270-147">The device name.</span></span>|
|<span data-ttu-id="85270-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="85270-148">userPrincipalName</span></span>|<span data-ttu-id="85270-149">String</span><span class="sxs-lookup"><span data-stu-id="85270-149">String</span></span>|<span data-ttu-id="85270-150">Имя участника пользователя</span><span class="sxs-lookup"><span data-stu-id="85270-150">The user principal name</span></span>|
|<span data-ttu-id="85270-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="85270-151">osVersion</span></span>|<span data-ttu-id="85270-152">String</span><span class="sxs-lookup"><span data-stu-id="85270-152">String</span></span>|<span data-ttu-id="85270-153">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="85270-153">The OS version.</span></span>|
|<span data-ttu-id="85270-154">сукцессфулупдатекаунт</span><span class="sxs-lookup"><span data-stu-id="85270-154">successfulUpdateCount</span></span>|<span data-ttu-id="85270-155">Int32</span><span class="sxs-lookup"><span data-stu-id="85270-155">Int32</span></span>|<span data-ttu-id="85270-156">Количество успешных обновлений на устройстве.</span><span class="sxs-lookup"><span data-stu-id="85270-156">Number of successful updates on the device.</span></span>|
|<span data-ttu-id="85270-157">фаиледупдатекаунт</span><span class="sxs-lookup"><span data-stu-id="85270-157">failedUpdateCount</span></span>|<span data-ttu-id="85270-158">Int32</span><span class="sxs-lookup"><span data-stu-id="85270-158">Int32</span></span>|<span data-ttu-id="85270-159">Количество неудачных обновлений на устройстве.</span><span class="sxs-lookup"><span data-stu-id="85270-159">Number of failed updates on the device.</span></span>|
|<span data-ttu-id="85270-160">тоталупдатекаунт</span><span class="sxs-lookup"><span data-stu-id="85270-160">totalUpdateCount</span></span>|<span data-ttu-id="85270-161">Int32</span><span class="sxs-lookup"><span data-stu-id="85270-161">Int32</span></span>|<span data-ttu-id="85270-162">Общее количество обновлений на устройстве.</span><span class="sxs-lookup"><span data-stu-id="85270-162">Number of total updates on the device.</span></span>|
|<span data-ttu-id="85270-163">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="85270-163">lastUpdatedDateTime</span></span>|<span data-ttu-id="85270-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85270-164">DateTimeOffset</span></span>|<span data-ttu-id="85270-165">Дата и время последнего обновления отчета для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="85270-165">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="85270-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="85270-166">Response</span></span>
<span data-ttu-id="85270-167">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85270-167">If successful, this method returns a `200 OK` response code and an updated [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85270-168">Пример</span><span class="sxs-lookup"><span data-stu-id="85270-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="85270-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="85270-169">Request</span></span>
<span data-ttu-id="85270-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85270-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}
Content-type: application/json
Content-length: 453

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateAccountSummary",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "userPrincipalName": "User Principal Name value",
  "osVersion": "Os Version value",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```

### <a name="response"></a><span data-ttu-id="85270-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="85270-171">Response</span></span>
<span data-ttu-id="85270-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85270-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 502

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateAccountSummary",
  "id": "64687d05-7d05-6468-057d-6864057d6864",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "userPrincipalName": "User Principal Name value",
  "osVersion": "Os Version value",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```





