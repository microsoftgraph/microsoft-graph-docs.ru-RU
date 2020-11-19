---
title: Создание Макоссофтвареупдатекатегорисуммари
description: Создание нового объекта Макоссофтвареупдатекатегорисуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f117769a5216a5522d91e254957605d938b9f89b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49236667"
---
# <a name="create-macossoftwareupdatecategorysummary"></a><span data-ttu-id="11937-103">Создание Макоссофтвареупдатекатегорисуммари</span><span class="sxs-lookup"><span data-stu-id="11937-103">Create macOSSoftwareUpdateCategorySummary</span></span>

<span data-ttu-id="11937-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11937-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11937-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11937-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11937-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11937-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11937-107">Создание нового объекта [макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) .</span><span class="sxs-lookup"><span data-stu-id="11937-107">Create a new [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11937-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="11937-108">Prerequisites</span></span>
<span data-ttu-id="11937-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11937-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11937-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11937-111">Permission type</span></span>|<span data-ttu-id="11937-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="11937-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11937-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11937-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11937-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11937-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="11937-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11937-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11937-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11937-116">Not supported.</span></span>|
|<span data-ttu-id="11937-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="11937-117">Application</span></span>|<span data-ttu-id="11937-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11937-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="11937-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11937-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries
```

## <a name="request-headers"></a><span data-ttu-id="11937-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="11937-120">Request headers</span></span>
|<span data-ttu-id="11937-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11937-121">Header</span></span>|<span data-ttu-id="11937-122">Значение</span><span class="sxs-lookup"><span data-stu-id="11937-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11937-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11937-123">Authorization</span></span>|<span data-ttu-id="11937-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11937-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11937-125">Accept</span><span class="sxs-lookup"><span data-stu-id="11937-125">Accept</span></span>|<span data-ttu-id="11937-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11937-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11937-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11937-127">Request body</span></span>
<span data-ttu-id="11937-128">В тексте запроса добавьте представление объекта Макоссофтвареупдатекатегорисуммари в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11937-128">In the request body, supply a JSON representation for the macOSSoftwareUpdateCategorySummary object.</span></span>

<span data-ttu-id="11937-129">В следующей таблице приведены свойства, необходимые при создании Макоссофтвареупдатекатегорисуммари.</span><span class="sxs-lookup"><span data-stu-id="11937-129">The following table shows the properties that are required when you create the macOSSoftwareUpdateCategorySummary.</span></span>

|<span data-ttu-id="11937-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="11937-130">Property</span></span>|<span data-ttu-id="11937-131">Тип</span><span class="sxs-lookup"><span data-stu-id="11937-131">Type</span></span>|<span data-ttu-id="11937-132">Описание</span><span class="sxs-lookup"><span data-stu-id="11937-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11937-133">id</span><span class="sxs-lookup"><span data-stu-id="11937-133">id</span></span>|<span data-ttu-id="11937-134">String</span><span class="sxs-lookup"><span data-stu-id="11937-134">String</span></span>|<span data-ttu-id="11937-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="11937-135">Key of the entity.</span></span>|
|<span data-ttu-id="11937-136">displayName</span><span class="sxs-lookup"><span data-stu-id="11937-136">displayName</span></span>|<span data-ttu-id="11937-137">String</span><span class="sxs-lookup"><span data-stu-id="11937-137">String</span></span>|<span data-ttu-id="11937-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="11937-138">The name of the report</span></span>|
|<span data-ttu-id="11937-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="11937-139">deviceId</span></span>|<span data-ttu-id="11937-140">String</span><span class="sxs-lookup"><span data-stu-id="11937-140">String</span></span>|<span data-ttu-id="11937-141">ИДЕНТИФИКАТОР устройства.</span><span class="sxs-lookup"><span data-stu-id="11937-141">The device ID.</span></span>|
|<span data-ttu-id="11937-142">userId</span><span class="sxs-lookup"><span data-stu-id="11937-142">userId</span></span>|<span data-ttu-id="11937-143">String</span><span class="sxs-lookup"><span data-stu-id="11937-143">String</span></span>|<span data-ttu-id="11937-144">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="11937-144">The user ID.</span></span>|
|<span data-ttu-id="11937-145">упдатекатегори</span><span class="sxs-lookup"><span data-stu-id="11937-145">updateCategory</span></span>|[<span data-ttu-id="11937-146">macOSSoftwareUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="11937-146">macOSSoftwareUpdateCategory</span></span>](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|<span data-ttu-id="11937-147">Тип обновления программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="11937-147">Software update type.</span></span> <span data-ttu-id="11937-148">Возможные значения: `critical`, `configurationDataFile`, `firmware`, `other`.</span><span class="sxs-lookup"><span data-stu-id="11937-148">Possible values are: `critical`, `configurationDataFile`, `firmware`, `other`.</span></span>|
|<span data-ttu-id="11937-149">сукцессфулупдатекаунт</span><span class="sxs-lookup"><span data-stu-id="11937-149">successfulUpdateCount</span></span>|<span data-ttu-id="11937-150">Int32</span><span class="sxs-lookup"><span data-stu-id="11937-150">Int32</span></span>|<span data-ttu-id="11937-151">Количество успешных обновлений на устройстве</span><span class="sxs-lookup"><span data-stu-id="11937-151">Number of successful updates on the device</span></span>|
|<span data-ttu-id="11937-152">фаиледупдатекаунт</span><span class="sxs-lookup"><span data-stu-id="11937-152">failedUpdateCount</span></span>|<span data-ttu-id="11937-153">Int32</span><span class="sxs-lookup"><span data-stu-id="11937-153">Int32</span></span>|<span data-ttu-id="11937-154">Количество неудачных обновлений на устройстве</span><span class="sxs-lookup"><span data-stu-id="11937-154">Number of failed updates on the device</span></span>|
|<span data-ttu-id="11937-155">тоталупдатекаунт</span><span class="sxs-lookup"><span data-stu-id="11937-155">totalUpdateCount</span></span>|<span data-ttu-id="11937-156">Int32</span><span class="sxs-lookup"><span data-stu-id="11937-156">Int32</span></span>|<span data-ttu-id="11937-157">Общее количество обновлений на устройстве</span><span class="sxs-lookup"><span data-stu-id="11937-157">Number of total updates on the device</span></span>|
|<span data-ttu-id="11937-158">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="11937-158">lastUpdatedDateTime</span></span>|<span data-ttu-id="11937-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11937-159">DateTimeOffset</span></span>|<span data-ttu-id="11937-160">Дата и время последнего обновления отчета для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="11937-160">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="11937-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="11937-161">Response</span></span>
<span data-ttu-id="11937-162">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="11937-162">If successful, this method returns a `201 Created` response code and a [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11937-163">Пример</span><span class="sxs-lookup"><span data-stu-id="11937-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="11937-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="11937-164">Request</span></span>
<span data-ttu-id="11937-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11937-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries
Content-type: application/json
Content-length: 373

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateCategorySummary",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "updateCategory": "configurationDataFile",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```

### <a name="response"></a><span data-ttu-id="11937-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="11937-166">Response</span></span>
<span data-ttu-id="11937-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11937-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 422

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateCategorySummary",
  "id": "f1fda232-a232-f1fd-32a2-fdf132a2fdf1",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "updateCategory": "configurationDataFile",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```




