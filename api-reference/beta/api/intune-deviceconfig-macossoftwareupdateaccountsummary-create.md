---
title: Создание macOSSoftwareUpdateAccountSummary
description: Создайте новый объект macOSSoftwareUpdateAccountSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a34b35952ee240784a4b4f28705fe49354024cb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129757"
---
# <a name="create-macossoftwareupdateaccountsummary"></a><span data-ttu-id="9c1c8-103">Создание macOSSoftwareUpdateAccountSummary</span><span class="sxs-lookup"><span data-stu-id="9c1c8-103">Create macOSSoftwareUpdateAccountSummary</span></span>

<span data-ttu-id="9c1c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c1c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c1c8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c1c8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c1c8-107">Создайте новый [объект macOSSoftwareUpdateAccountSummary.](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)</span><span class="sxs-lookup"><span data-stu-id="9c1c8-107">Create a new [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c1c8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9c1c8-108">Prerequisites</span></span>
<span data-ttu-id="9c1c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c1c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c1c8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c1c8-111">Permission type</span></span>|<span data-ttu-id="9c1c8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c1c8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c1c8-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c1c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c1c8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c1c8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9c1c8-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c1c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c1c8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-116">Not supported.</span></span>|
|<span data-ttu-id="9c1c8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9c1c8-117">Application</span></span>|<span data-ttu-id="9c1c8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c1c8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c1c8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c1c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/macOSSoftwareUpdateAccountSummaries
```

## <a name="request-headers"></a><span data-ttu-id="9c1c8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9c1c8-120">Request headers</span></span>
|<span data-ttu-id="9c1c8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c1c8-121">Header</span></span>|<span data-ttu-id="9c1c8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9c1c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c1c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c1c8-123">Authorization</span></span>|<span data-ttu-id="9c1c8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c1c8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9c1c8-125">Accept</span></span>|<span data-ttu-id="9c1c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c1c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c1c8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c1c8-127">Request body</span></span>
<span data-ttu-id="9c1c8-128">В теле запроса поставляем представление JSON для объекта macOSSoftwareUpdateAccountSummary.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-128">In the request body, supply a JSON representation for the macOSSoftwareUpdateAccountSummary object.</span></span>

<span data-ttu-id="9c1c8-129">В следующей таблице показаны свойства, необходимые при создании macOSSoftwareUpdateAccountSummary.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-129">The following table shows the properties that are required when you create the macOSSoftwareUpdateAccountSummary.</span></span>

|<span data-ttu-id="9c1c8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c1c8-130">Property</span></span>|<span data-ttu-id="9c1c8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9c1c8-131">Type</span></span>|<span data-ttu-id="9c1c8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9c1c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c1c8-133">id</span><span class="sxs-lookup"><span data-stu-id="9c1c8-133">id</span></span>|<span data-ttu-id="9c1c8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9c1c8-134">String</span></span>|<span data-ttu-id="9c1c8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-135">Key of the entity.</span></span>|
|<span data-ttu-id="9c1c8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9c1c8-136">displayName</span></span>|<span data-ttu-id="9c1c8-137">Строка</span><span class="sxs-lookup"><span data-stu-id="9c1c8-137">String</span></span>|<span data-ttu-id="9c1c8-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="9c1c8-138">The name of the report</span></span>|
|<span data-ttu-id="9c1c8-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="9c1c8-139">deviceId</span></span>|<span data-ttu-id="9c1c8-140">String</span><span class="sxs-lookup"><span data-stu-id="9c1c8-140">String</span></span>|<span data-ttu-id="9c1c8-141">ID устройства.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-141">The device ID.</span></span>|
|<span data-ttu-id="9c1c8-142">userId</span><span class="sxs-lookup"><span data-stu-id="9c1c8-142">userId</span></span>|<span data-ttu-id="9c1c8-143">String</span><span class="sxs-lookup"><span data-stu-id="9c1c8-143">String</span></span>|<span data-ttu-id="9c1c8-144">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-144">The user ID.</span></span>|
|<span data-ttu-id="9c1c8-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="9c1c8-145">deviceName</span></span>|<span data-ttu-id="9c1c8-146">String</span><span class="sxs-lookup"><span data-stu-id="9c1c8-146">String</span></span>|<span data-ttu-id="9c1c8-147">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-147">The device name.</span></span>|
|<span data-ttu-id="9c1c8-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9c1c8-148">userPrincipalName</span></span>|<span data-ttu-id="9c1c8-149">String</span><span class="sxs-lookup"><span data-stu-id="9c1c8-149">String</span></span>|<span data-ttu-id="9c1c8-150">Имя основного пользователя</span><span class="sxs-lookup"><span data-stu-id="9c1c8-150">The user principal name</span></span>|
|<span data-ttu-id="9c1c8-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="9c1c8-151">osVersion</span></span>|<span data-ttu-id="9c1c8-152">String</span><span class="sxs-lookup"><span data-stu-id="9c1c8-152">String</span></span>|<span data-ttu-id="9c1c8-153">Версия ОС.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-153">The OS version.</span></span>|
|<span data-ttu-id="9c1c8-154">successfulUpdateCount</span><span class="sxs-lookup"><span data-stu-id="9c1c8-154">successfulUpdateCount</span></span>|<span data-ttu-id="9c1c8-155">Int32</span><span class="sxs-lookup"><span data-stu-id="9c1c8-155">Int32</span></span>|<span data-ttu-id="9c1c8-156">Количество успешных обновлений на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-156">Number of successful updates on the device.</span></span>|
|<span data-ttu-id="9c1c8-157">failedUpdateCount</span><span class="sxs-lookup"><span data-stu-id="9c1c8-157">failedUpdateCount</span></span>|<span data-ttu-id="9c1c8-158">Int32</span><span class="sxs-lookup"><span data-stu-id="9c1c8-158">Int32</span></span>|<span data-ttu-id="9c1c8-159">Количество сбойных обновлений на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-159">Number of failed updates on the device.</span></span>|
|<span data-ttu-id="9c1c8-160">totalUpdateCount</span><span class="sxs-lookup"><span data-stu-id="9c1c8-160">totalUpdateCount</span></span>|<span data-ttu-id="9c1c8-161">Int32</span><span class="sxs-lookup"><span data-stu-id="9c1c8-161">Int32</span></span>|<span data-ttu-id="9c1c8-162">Количество обновлений на устройстве.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-162">Number of total updates on the device.</span></span>|
|<span data-ttu-id="9c1c8-163">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c1c8-163">lastUpdatedDateTime</span></span>|<span data-ttu-id="9c1c8-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c1c8-164">DateTimeOffset</span></span>|<span data-ttu-id="9c1c8-165">Последняя дата обновления отчета для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-165">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="9c1c8-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c1c8-166">Response</span></span>
<span data-ttu-id="9c1c8-167">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-167">If successful, this method returns a `201 Created` response code and a [macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c1c8-168">Пример</span><span class="sxs-lookup"><span data-stu-id="9c1c8-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c1c8-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c1c8-169">Request</span></span>
<span data-ttu-id="9c1c8-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9c1c8-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c1c8-171">Response</span></span>
<span data-ttu-id="9c1c8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9c1c8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




