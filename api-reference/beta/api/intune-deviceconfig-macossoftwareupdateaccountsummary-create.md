---
title: Создание Макоссофтвареупдатеаккаунтсуммари
description: Создание нового объекта Макоссофтвареупдатеаккаунтсуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf31e6c06010d678b43b08786beb42ae92514589
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705198"
---
# <a name="create-macossoftwareupdateaccountsummary"></a><span data-ttu-id="f53e9-103">Создание Макоссофтвареупдатеаккаунтсуммари</span><span class="sxs-lookup"><span data-stu-id="f53e9-103">Create macOSSoftwareUpdateAccountSummary</span></span>

<span data-ttu-id="f53e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f53e9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f53e9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f53e9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f53e9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f53e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f53e9-107">Создание нового объекта [макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="f53e9-107">Create a new [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f53e9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f53e9-108">Prerequisites</span></span>
<span data-ttu-id="f53e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f53e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f53e9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f53e9-111">Permission type</span></span>|<span data-ttu-id="f53e9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f53e9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f53e9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f53e9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f53e9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f53e9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f53e9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f53e9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f53e9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f53e9-116">Not supported.</span></span>|
|<span data-ttu-id="f53e9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f53e9-117">Application</span></span>|<span data-ttu-id="f53e9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f53e9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f53e9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f53e9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/macOSSoftwareUpdateAccountSummaries
```

## <a name="request-headers"></a><span data-ttu-id="f53e9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f53e9-120">Request headers</span></span>
|<span data-ttu-id="f53e9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f53e9-121">Header</span></span>|<span data-ttu-id="f53e9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f53e9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f53e9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f53e9-123">Authorization</span></span>|<span data-ttu-id="f53e9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f53e9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f53e9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f53e9-125">Accept</span></span>|<span data-ttu-id="f53e9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f53e9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f53e9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f53e9-127">Request body</span></span>
<span data-ttu-id="f53e9-128">В тексте запроса добавьте представление объекта Макоссофтвареупдатеаккаунтсуммари в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f53e9-128">In the request body, supply a JSON representation for the macOSSoftwareUpdateAccountSummary object.</span></span>

<span data-ttu-id="f53e9-129">В следующей таблице приведены свойства, необходимые при создании Макоссофтвареупдатеаккаунтсуммари.</span><span class="sxs-lookup"><span data-stu-id="f53e9-129">The following table shows the properties that are required when you create the macOSSoftwareUpdateAccountSummary.</span></span>

|<span data-ttu-id="f53e9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f53e9-130">Property</span></span>|<span data-ttu-id="f53e9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f53e9-131">Type</span></span>|<span data-ttu-id="f53e9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f53e9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f53e9-133">id</span><span class="sxs-lookup"><span data-stu-id="f53e9-133">id</span></span>|<span data-ttu-id="f53e9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f53e9-134">String</span></span>|<span data-ttu-id="f53e9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f53e9-135">Key of the entity.</span></span>|
|<span data-ttu-id="f53e9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f53e9-136">displayName</span></span>|<span data-ttu-id="f53e9-137">Строка</span><span class="sxs-lookup"><span data-stu-id="f53e9-137">String</span></span>|<span data-ttu-id="f53e9-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="f53e9-138">The name of the report</span></span>|
|<span data-ttu-id="f53e9-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="f53e9-139">deviceId</span></span>|<span data-ttu-id="f53e9-140">String</span><span class="sxs-lookup"><span data-stu-id="f53e9-140">String</span></span>|<span data-ttu-id="f53e9-141">ИДЕНТИФИКАТОР устройства.</span><span class="sxs-lookup"><span data-stu-id="f53e9-141">The device ID.</span></span>|
|<span data-ttu-id="f53e9-142">userId</span><span class="sxs-lookup"><span data-stu-id="f53e9-142">userId</span></span>|<span data-ttu-id="f53e9-143">String</span><span class="sxs-lookup"><span data-stu-id="f53e9-143">String</span></span>|<span data-ttu-id="f53e9-144">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="f53e9-144">The user ID.</span></span>|
|<span data-ttu-id="f53e9-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="f53e9-145">deviceName</span></span>|<span data-ttu-id="f53e9-146">String</span><span class="sxs-lookup"><span data-stu-id="f53e9-146">String</span></span>|<span data-ttu-id="f53e9-147">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="f53e9-147">The device name.</span></span>|
|<span data-ttu-id="f53e9-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f53e9-148">userPrincipalName</span></span>|<span data-ttu-id="f53e9-149">String</span><span class="sxs-lookup"><span data-stu-id="f53e9-149">String</span></span>|<span data-ttu-id="f53e9-150">Имя участника пользователя</span><span class="sxs-lookup"><span data-stu-id="f53e9-150">The user principal name</span></span>|
|<span data-ttu-id="f53e9-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="f53e9-151">osVersion</span></span>|<span data-ttu-id="f53e9-152">String</span><span class="sxs-lookup"><span data-stu-id="f53e9-152">String</span></span>|<span data-ttu-id="f53e9-153">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="f53e9-153">The OS version.</span></span>|
|<span data-ttu-id="f53e9-154">сукцессфулупдатекаунт</span><span class="sxs-lookup"><span data-stu-id="f53e9-154">successfulUpdateCount</span></span>|<span data-ttu-id="f53e9-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f53e9-155">Int32</span></span>|<span data-ttu-id="f53e9-156">Количество успешных обновлений на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f53e9-156">Number of successful updates on the device.</span></span>|
|<span data-ttu-id="f53e9-157">фаиледупдатекаунт</span><span class="sxs-lookup"><span data-stu-id="f53e9-157">failedUpdateCount</span></span>|<span data-ttu-id="f53e9-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f53e9-158">Int32</span></span>|<span data-ttu-id="f53e9-159">Количество неудачных обновлений на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f53e9-159">Number of failed updates on the device.</span></span>|
|<span data-ttu-id="f53e9-160">тоталупдатекаунт</span><span class="sxs-lookup"><span data-stu-id="f53e9-160">totalUpdateCount</span></span>|<span data-ttu-id="f53e9-161">Int32</span><span class="sxs-lookup"><span data-stu-id="f53e9-161">Int32</span></span>|<span data-ttu-id="f53e9-162">Общее количество обновлений на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f53e9-162">Number of total updates on the device.</span></span>|
|<span data-ttu-id="f53e9-163">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f53e9-163">lastUpdatedDateTime</span></span>|<span data-ttu-id="f53e9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f53e9-164">DateTimeOffset</span></span>|<span data-ttu-id="f53e9-165">Дата и время последнего обновления отчета для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="f53e9-165">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="f53e9-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="f53e9-166">Response</span></span>
<span data-ttu-id="f53e9-167">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f53e9-167">If successful, this method returns a `201 Created` response code and a [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f53e9-168">Пример</span><span class="sxs-lookup"><span data-stu-id="f53e9-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="f53e9-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="f53e9-169">Request</span></span>
<span data-ttu-id="f53e9-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f53e9-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries
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

### <a name="response"></a><span data-ttu-id="f53e9-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="f53e9-171">Response</span></span>
<span data-ttu-id="f53e9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f53e9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





