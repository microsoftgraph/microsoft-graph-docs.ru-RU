---
title: Обновление macOSSoftwareUpdateAccountSummary
description: Обновление свойств объекта macOSSoftwareUpdateAccountSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b2412c54b1576308e7861cd961b211ea9fdc09dd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129729"
---
# <a name="update-macossoftwareupdateaccountsummary"></a><span data-ttu-id="b33da-103">Обновление macOSSoftwareUpdateAccountSummary</span><span class="sxs-lookup"><span data-stu-id="b33da-103">Update macOSSoftwareUpdateAccountSummary</span></span>

<span data-ttu-id="b33da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b33da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b33da-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b33da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b33da-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b33da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b33da-107">Обновление свойств объекта [macOSSoftwareUpdateAccountSummary.](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)</span><span class="sxs-lookup"><span data-stu-id="b33da-107">Update the properties of a [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b33da-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b33da-108">Prerequisites</span></span>
<span data-ttu-id="b33da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b33da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b33da-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b33da-111">Permission type</span></span>|<span data-ttu-id="b33da-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b33da-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b33da-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b33da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b33da-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b33da-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b33da-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b33da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b33da-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b33da-116">Not supported.</span></span>|
|<span data-ttu-id="b33da-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b33da-117">Application</span></span>|<span data-ttu-id="b33da-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b33da-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b33da-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b33da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="b33da-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b33da-120">Request headers</span></span>
|<span data-ttu-id="b33da-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b33da-121">Header</span></span>|<span data-ttu-id="b33da-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b33da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b33da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b33da-123">Authorization</span></span>|<span data-ttu-id="b33da-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b33da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b33da-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b33da-125">Accept</span></span>|<span data-ttu-id="b33da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b33da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b33da-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b33da-127">Request body</span></span>
<span data-ttu-id="b33da-128">В теле запроса поставляем представление JSON для [объекта macOSSoftwareUpdateAccountSummary.](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)</span><span class="sxs-lookup"><span data-stu-id="b33da-128">In the request body, supply a JSON representation for the [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object.</span></span>

<span data-ttu-id="b33da-129">В следующей таблице показаны свойства, необходимые при создании [macOSSoftwareUpdateAccountSummary.](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)</span><span class="sxs-lookup"><span data-stu-id="b33da-129">The following table shows the properties that are required when you create the [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md).</span></span>

|<span data-ttu-id="b33da-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b33da-130">Property</span></span>|<span data-ttu-id="b33da-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b33da-131">Type</span></span>|<span data-ttu-id="b33da-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b33da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b33da-133">id</span><span class="sxs-lookup"><span data-stu-id="b33da-133">id</span></span>|<span data-ttu-id="b33da-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b33da-134">String</span></span>|<span data-ttu-id="b33da-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b33da-135">Key of the entity.</span></span>|
|<span data-ttu-id="b33da-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b33da-136">displayName</span></span>|<span data-ttu-id="b33da-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b33da-137">String</span></span>|<span data-ttu-id="b33da-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="b33da-138">The name of the report</span></span>|
|<span data-ttu-id="b33da-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="b33da-139">deviceId</span></span>|<span data-ttu-id="b33da-140">String</span><span class="sxs-lookup"><span data-stu-id="b33da-140">String</span></span>|<span data-ttu-id="b33da-141">ID устройства.</span><span class="sxs-lookup"><span data-stu-id="b33da-141">The device ID.</span></span>|
|<span data-ttu-id="b33da-142">userId</span><span class="sxs-lookup"><span data-stu-id="b33da-142">userId</span></span>|<span data-ttu-id="b33da-143">String</span><span class="sxs-lookup"><span data-stu-id="b33da-143">String</span></span>|<span data-ttu-id="b33da-144">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="b33da-144">The user ID.</span></span>|
|<span data-ttu-id="b33da-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="b33da-145">deviceName</span></span>|<span data-ttu-id="b33da-146">String</span><span class="sxs-lookup"><span data-stu-id="b33da-146">String</span></span>|<span data-ttu-id="b33da-147">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="b33da-147">The device name.</span></span>|
|<span data-ttu-id="b33da-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b33da-148">userPrincipalName</span></span>|<span data-ttu-id="b33da-149">String</span><span class="sxs-lookup"><span data-stu-id="b33da-149">String</span></span>|<span data-ttu-id="b33da-150">Имя основного пользователя</span><span class="sxs-lookup"><span data-stu-id="b33da-150">The user principal name</span></span>|
|<span data-ttu-id="b33da-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="b33da-151">osVersion</span></span>|<span data-ttu-id="b33da-152">String</span><span class="sxs-lookup"><span data-stu-id="b33da-152">String</span></span>|<span data-ttu-id="b33da-153">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="b33da-153">The OS version.</span></span>|
|<span data-ttu-id="b33da-154">successfulUpdateCount</span><span class="sxs-lookup"><span data-stu-id="b33da-154">successfulUpdateCount</span></span>|<span data-ttu-id="b33da-155">Int32</span><span class="sxs-lookup"><span data-stu-id="b33da-155">Int32</span></span>|<span data-ttu-id="b33da-156">Количество успешных обновлений на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b33da-156">Number of successful updates on the device.</span></span>|
|<span data-ttu-id="b33da-157">failedUpdateCount</span><span class="sxs-lookup"><span data-stu-id="b33da-157">failedUpdateCount</span></span>|<span data-ttu-id="b33da-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b33da-158">Int32</span></span>|<span data-ttu-id="b33da-159">Количество сбойных обновлений на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b33da-159">Number of failed updates on the device.</span></span>|
|<span data-ttu-id="b33da-160">totalUpdateCount</span><span class="sxs-lookup"><span data-stu-id="b33da-160">totalUpdateCount</span></span>|<span data-ttu-id="b33da-161">Int32</span><span class="sxs-lookup"><span data-stu-id="b33da-161">Int32</span></span>|<span data-ttu-id="b33da-162">Количество обновлений на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b33da-162">Number of total updates on the device.</span></span>|
|<span data-ttu-id="b33da-163">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b33da-163">lastUpdatedDateTime</span></span>|<span data-ttu-id="b33da-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b33da-164">DateTimeOffset</span></span>|<span data-ttu-id="b33da-165">Последняя дата обновления отчета для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="b33da-165">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="b33da-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="b33da-166">Response</span></span>
<span data-ttu-id="b33da-167">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b33da-167">If successful, this method returns a `200 OK` response code and an updated [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b33da-168">Пример</span><span class="sxs-lookup"><span data-stu-id="b33da-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="b33da-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="b33da-169">Request</span></span>
<span data-ttu-id="b33da-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b33da-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b33da-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="b33da-171">Response</span></span>
<span data-ttu-id="b33da-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b33da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




