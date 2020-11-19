---
title: Обновление Макоссофтвареупдатекатегорисуммари
description: Обновление свойств объекта Макоссофтвареупдатекатегорисуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 69c75261058fa1ebdc60c726d77e093f49ea0b24
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49236451"
---
# <a name="update-macossoftwareupdatecategorysummary"></a><span data-ttu-id="8de99-103">Обновление Макоссофтвареупдатекатегорисуммари</span><span class="sxs-lookup"><span data-stu-id="8de99-103">Update macOSSoftwareUpdateCategorySummary</span></span>

<span data-ttu-id="8de99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8de99-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8de99-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8de99-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8de99-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8de99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8de99-107">Обновление свойств объекта [макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) .</span><span class="sxs-lookup"><span data-stu-id="8de99-107">Update the properties of a [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8de99-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8de99-108">Prerequisites</span></span>
<span data-ttu-id="8de99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8de99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8de99-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8de99-111">Permission type</span></span>|<span data-ttu-id="8de99-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8de99-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8de99-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8de99-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8de99-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8de99-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8de99-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8de99-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8de99-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8de99-116">Not supported.</span></span>|
|<span data-ttu-id="8de99-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8de99-117">Application</span></span>|<span data-ttu-id="8de99-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8de99-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8de99-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8de99-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="8de99-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8de99-120">Request headers</span></span>
|<span data-ttu-id="8de99-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8de99-121">Header</span></span>|<span data-ttu-id="8de99-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8de99-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8de99-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8de99-123">Authorization</span></span>|<span data-ttu-id="8de99-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8de99-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8de99-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8de99-125">Accept</span></span>|<span data-ttu-id="8de99-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8de99-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8de99-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8de99-127">Request body</span></span>
<span data-ttu-id="8de99-128">В тексте запроса добавьте представление объекта [макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8de99-128">In the request body, supply a JSON representation for the [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object.</span></span>

<span data-ttu-id="8de99-129">В следующей таблице приведены свойства, необходимые при создании [макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md).</span><span class="sxs-lookup"><span data-stu-id="8de99-129">The following table shows the properties that are required when you create the [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md).</span></span>

|<span data-ttu-id="8de99-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8de99-130">Property</span></span>|<span data-ttu-id="8de99-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8de99-131">Type</span></span>|<span data-ttu-id="8de99-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8de99-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8de99-133">id</span><span class="sxs-lookup"><span data-stu-id="8de99-133">id</span></span>|<span data-ttu-id="8de99-134">String</span><span class="sxs-lookup"><span data-stu-id="8de99-134">String</span></span>|<span data-ttu-id="8de99-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8de99-135">Key of the entity.</span></span>|
|<span data-ttu-id="8de99-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8de99-136">displayName</span></span>|<span data-ttu-id="8de99-137">String</span><span class="sxs-lookup"><span data-stu-id="8de99-137">String</span></span>|<span data-ttu-id="8de99-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="8de99-138">The name of the report</span></span>|
|<span data-ttu-id="8de99-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="8de99-139">deviceId</span></span>|<span data-ttu-id="8de99-140">String</span><span class="sxs-lookup"><span data-stu-id="8de99-140">String</span></span>|<span data-ttu-id="8de99-141">ИДЕНТИФИКАТОР устройства.</span><span class="sxs-lookup"><span data-stu-id="8de99-141">The device ID.</span></span>|
|<span data-ttu-id="8de99-142">userId</span><span class="sxs-lookup"><span data-stu-id="8de99-142">userId</span></span>|<span data-ttu-id="8de99-143">String</span><span class="sxs-lookup"><span data-stu-id="8de99-143">String</span></span>|<span data-ttu-id="8de99-144">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="8de99-144">The user ID.</span></span>|
|<span data-ttu-id="8de99-145">упдатекатегори</span><span class="sxs-lookup"><span data-stu-id="8de99-145">updateCategory</span></span>|[<span data-ttu-id="8de99-146">macOSSoftwareUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="8de99-146">macOSSoftwareUpdateCategory</span></span>](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|<span data-ttu-id="8de99-147">Тип обновления программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="8de99-147">Software update type.</span></span> <span data-ttu-id="8de99-148">Возможные значения: `critical`, `configurationDataFile`, `firmware`, `other`.</span><span class="sxs-lookup"><span data-stu-id="8de99-148">Possible values are: `critical`, `configurationDataFile`, `firmware`, `other`.</span></span>|
|<span data-ttu-id="8de99-149">сукцессфулупдатекаунт</span><span class="sxs-lookup"><span data-stu-id="8de99-149">successfulUpdateCount</span></span>|<span data-ttu-id="8de99-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8de99-150">Int32</span></span>|<span data-ttu-id="8de99-151">Количество успешных обновлений на устройстве</span><span class="sxs-lookup"><span data-stu-id="8de99-151">Number of successful updates on the device</span></span>|
|<span data-ttu-id="8de99-152">фаиледупдатекаунт</span><span class="sxs-lookup"><span data-stu-id="8de99-152">failedUpdateCount</span></span>|<span data-ttu-id="8de99-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8de99-153">Int32</span></span>|<span data-ttu-id="8de99-154">Количество неудачных обновлений на устройстве</span><span class="sxs-lookup"><span data-stu-id="8de99-154">Number of failed updates on the device</span></span>|
|<span data-ttu-id="8de99-155">тоталупдатекаунт</span><span class="sxs-lookup"><span data-stu-id="8de99-155">totalUpdateCount</span></span>|<span data-ttu-id="8de99-156">Int32</span><span class="sxs-lookup"><span data-stu-id="8de99-156">Int32</span></span>|<span data-ttu-id="8de99-157">Общее количество обновлений на устройстве</span><span class="sxs-lookup"><span data-stu-id="8de99-157">Number of total updates on the device</span></span>|
|<span data-ttu-id="8de99-158">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8de99-158">lastUpdatedDateTime</span></span>|<span data-ttu-id="8de99-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8de99-159">DateTimeOffset</span></span>|<span data-ttu-id="8de99-160">Дата и время последнего обновления отчета для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="8de99-160">Last date time the report for this device was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="8de99-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="8de99-161">Response</span></span>
<span data-ttu-id="8de99-162">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8de99-162">If successful, this method returns a `200 OK` response code and an updated [macOSSoftwareUpdateCategorySummary](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8de99-163">Пример</span><span class="sxs-lookup"><span data-stu-id="8de99-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="8de99-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="8de99-164">Request</span></span>
<span data-ttu-id="8de99-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8de99-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}
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

### <a name="response"></a><span data-ttu-id="8de99-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="8de99-166">Response</span></span>
<span data-ttu-id="8de99-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8de99-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




