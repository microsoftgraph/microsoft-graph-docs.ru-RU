---
title: Обновление Макоссофтвареупдатестатесуммари
description: Обновление свойств объекта Макоссофтвареупдатестатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 325dff0ef7f2cdcfce5894c831dda97a93a72b13
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49213471"
---
# <a name="update-macossoftwareupdatestatesummary"></a><span data-ttu-id="f3509-103">Обновление Макоссофтвареупдатестатесуммари</span><span class="sxs-lookup"><span data-stu-id="f3509-103">Update macOSSoftwareUpdateStateSummary</span></span>

<span data-ttu-id="f3509-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3509-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3509-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3509-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3509-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3509-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3509-107">Обновление свойств объекта [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="f3509-107">Update the properties of a [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3509-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f3509-108">Prerequisites</span></span>
<span data-ttu-id="f3509-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3509-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3509-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3509-111">Permission type</span></span>|<span data-ttu-id="f3509-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3509-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3509-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3509-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3509-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3509-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3509-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3509-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3509-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3509-116">Not supported.</span></span>|
|<span data-ttu-id="f3509-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f3509-117">Application</span></span>|<span data-ttu-id="f3509-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3509-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3509-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3509-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries/{macOSSoftwareUpdateStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="f3509-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f3509-120">Request headers</span></span>
|<span data-ttu-id="f3509-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3509-121">Header</span></span>|<span data-ttu-id="f3509-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3509-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3509-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3509-123">Authorization</span></span>|<span data-ttu-id="f3509-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3509-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3509-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3509-125">Accept</span></span>|<span data-ttu-id="f3509-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3509-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3509-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3509-127">Request body</span></span>
<span data-ttu-id="f3509-128">В тексте запроса добавьте представление объекта [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3509-128">In the request body, supply a JSON representation for the [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object.</span></span>

<span data-ttu-id="f3509-129">В следующей таблице приведены свойства, необходимые при создании [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f3509-129">The following table shows the properties that are required when you create the [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md).</span></span>

|<span data-ttu-id="f3509-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3509-130">Property</span></span>|<span data-ttu-id="f3509-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f3509-131">Type</span></span>|<span data-ttu-id="f3509-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f3509-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3509-133">id</span><span class="sxs-lookup"><span data-stu-id="f3509-133">id</span></span>|<span data-ttu-id="f3509-134">String</span><span class="sxs-lookup"><span data-stu-id="f3509-134">String</span></span>|<span data-ttu-id="f3509-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f3509-135">Key of the entity.</span></span>|
|<span data-ttu-id="f3509-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f3509-136">displayName</span></span>|<span data-ttu-id="f3509-137">String</span><span class="sxs-lookup"><span data-stu-id="f3509-137">String</span></span>|<span data-ttu-id="f3509-138">Понятное имя обновления программного обеспечения</span><span class="sxs-lookup"><span data-stu-id="f3509-138">Human readable name of the software update</span></span>|
|<span data-ttu-id="f3509-139">productKey</span><span class="sxs-lookup"><span data-stu-id="f3509-139">productKey</span></span>|<span data-ttu-id="f3509-140">String</span><span class="sxs-lookup"><span data-stu-id="f3509-140">String</span></span>|<span data-ttu-id="f3509-141">Ключ продукта обновления программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="f3509-141">Product key of the software update.</span></span>|
|<span data-ttu-id="f3509-142">упдатекатегори</span><span class="sxs-lookup"><span data-stu-id="f3509-142">updateCategory</span></span>|[<span data-ttu-id="f3509-143">macOSSoftwareUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="f3509-143">macOSSoftwareUpdateCategory</span></span>](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|<span data-ttu-id="f3509-144">Категория обновлений программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="f3509-144">Software update category.</span></span> <span data-ttu-id="f3509-145">Возможные значения: `critical`, `configurationDataFile`, `firmware`, `other`.</span><span class="sxs-lookup"><span data-stu-id="f3509-145">Possible values are: `critical`, `configurationDataFile`, `firmware`, `other`.</span></span>|
|<span data-ttu-id="f3509-146">упдатеверсион</span><span class="sxs-lookup"><span data-stu-id="f3509-146">updateVersion</span></span>|<span data-ttu-id="f3509-147">String</span><span class="sxs-lookup"><span data-stu-id="f3509-147">String</span></span>|<span data-ttu-id="f3509-148">Версия обновления программного обеспечения</span><span class="sxs-lookup"><span data-stu-id="f3509-148">Version of the software update</span></span>|
|<span data-ttu-id="f3509-149">state</span><span class="sxs-lookup"><span data-stu-id="f3509-149">state</span></span>|[<span data-ttu-id="f3509-150">macOSSoftwareUpdateState</span><span class="sxs-lookup"><span data-stu-id="f3509-150">macOSSoftwareUpdateState</span></span>](../resources/intune-deviceconfig-macossoftwareupdatestate.md)|<span data-ttu-id="f3509-151">Состояние обновления программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="f3509-151">State of the software update.</span></span> <span data-ttu-id="f3509-152">Возможные значения: `success` , `downloading` ,,,,, `downloaded` `installing` `idle` `available` `scheduled` ,,, `downloadFailed` `downloadInsufficientSpace` `downloadInsufficientPower` , `downloadInsufficientNetwork` , `installInsufficientSpace` , `installInsufficientPower` , `installFailed` , `commandFailed` .</span><span class="sxs-lookup"><span data-stu-id="f3509-152">Possible values are: `success`, `downloading`, `downloaded`, `installing`, `idle`, `available`, `scheduled`, `downloadFailed`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installInsufficientSpace`, `installInsufficientPower`, `installFailed`, `commandFailed`.</span></span>|
|<span data-ttu-id="f3509-153">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3509-153">lastUpdatedDateTime</span></span>|<span data-ttu-id="f3509-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3509-154">DateTimeOffset</span></span>|<span data-ttu-id="f3509-155">Дата и время последнего обновления отчета для этого устройства и ключа продукта.</span><span class="sxs-lookup"><span data-stu-id="f3509-155">Last date time the report for this device and product key was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="f3509-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3509-156">Response</span></span>
<span data-ttu-id="f3509-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f3509-157">If successful, this method returns a `200 OK` response code and an updated [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3509-158">Пример</span><span class="sxs-lookup"><span data-stu-id="f3509-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3509-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3509-159">Request</span></span>
<span data-ttu-id="f3509-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3509-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries/{macOSSoftwareUpdateStateSummaryId}
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateStateSummary",
  "displayName": "Display Name value",
  "productKey": "Product Key value",
  "updateCategory": "configurationDataFile",
  "updateVersion": "Update Version value",
  "state": "downloading",
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```

### <a name="response"></a><span data-ttu-id="f3509-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3509-161">Response</span></span>
<span data-ttu-id="f3509-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3509-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 380

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateStateSummary",
  "id": "9527a1df-a1df-9527-dfa1-2795dfa12795",
  "displayName": "Display Name value",
  "productKey": "Product Key value",
  "updateCategory": "configurationDataFile",
  "updateVersion": "Update Version value",
  "state": "downloading",
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```




