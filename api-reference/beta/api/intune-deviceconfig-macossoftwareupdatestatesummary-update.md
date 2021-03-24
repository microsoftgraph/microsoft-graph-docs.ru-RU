---
title: Обновление macOSSoftwareUpdateStateSummary
description: Обновление свойств объекта macOSSoftwareUpdateStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 405f1590c2f21a2de14a9611136f17c2b24ce0ba
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132606"
---
# <a name="update-macossoftwareupdatestatesummary"></a><span data-ttu-id="9c125-103">Обновление macOSSoftwareUpdateStateSummary</span><span class="sxs-lookup"><span data-stu-id="9c125-103">Update macOSSoftwareUpdateStateSummary</span></span>

<span data-ttu-id="9c125-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c125-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c125-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c125-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c125-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c125-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c125-107">Обновление свойств объекта [macOSSoftwareUpdateStateSummary.](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9c125-107">Update the properties of a [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c125-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9c125-108">Prerequisites</span></span>
<span data-ttu-id="9c125-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c125-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c125-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c125-111">Permission type</span></span>|<span data-ttu-id="9c125-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c125-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c125-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c125-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c125-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c125-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9c125-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c125-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c125-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c125-116">Not supported.</span></span>|
|<span data-ttu-id="9c125-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9c125-117">Application</span></span>|<span data-ttu-id="9c125-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c125-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c125-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c125-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries/{macOSSoftwareUpdateStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="9c125-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9c125-120">Request headers</span></span>
|<span data-ttu-id="9c125-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c125-121">Header</span></span>|<span data-ttu-id="9c125-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9c125-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c125-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c125-123">Authorization</span></span>|<span data-ttu-id="9c125-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c125-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c125-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9c125-125">Accept</span></span>|<span data-ttu-id="9c125-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c125-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c125-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c125-127">Request body</span></span>
<span data-ttu-id="9c125-128">В теле запроса укажи представление JSON для [объекта macOSSoftwareUpdateStateSummary.](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9c125-128">In the request body, supply a JSON representation for the [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object.</span></span>

<span data-ttu-id="9c125-129">В следующей таблице показаны свойства, необходимые при создании [macOSSoftwareUpdateStateSummary.](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9c125-129">The following table shows the properties that are required when you create the [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md).</span></span>

|<span data-ttu-id="9c125-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c125-130">Property</span></span>|<span data-ttu-id="9c125-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9c125-131">Type</span></span>|<span data-ttu-id="9c125-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9c125-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c125-133">id</span><span class="sxs-lookup"><span data-stu-id="9c125-133">id</span></span>|<span data-ttu-id="9c125-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9c125-134">String</span></span>|<span data-ttu-id="9c125-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9c125-135">Key of the entity.</span></span>|
|<span data-ttu-id="9c125-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9c125-136">displayName</span></span>|<span data-ttu-id="9c125-137">Строка</span><span class="sxs-lookup"><span data-stu-id="9c125-137">String</span></span>|<span data-ttu-id="9c125-138">Понятное для человека имя обновления программного обеспечения</span><span class="sxs-lookup"><span data-stu-id="9c125-138">Human readable name of the software update</span></span>|
|<span data-ttu-id="9c125-139">productKey</span><span class="sxs-lookup"><span data-stu-id="9c125-139">productKey</span></span>|<span data-ttu-id="9c125-140">String</span><span class="sxs-lookup"><span data-stu-id="9c125-140">String</span></span>|<span data-ttu-id="9c125-141">Ключ продукта обновления программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="9c125-141">Product key of the software update.</span></span>|
|<span data-ttu-id="9c125-142">updateCategory</span><span class="sxs-lookup"><span data-stu-id="9c125-142">updateCategory</span></span>|[<span data-ttu-id="9c125-143">macOSSoftwareUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="9c125-143">macOSSoftwareUpdateCategory</span></span>](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|<span data-ttu-id="9c125-144">Категория обновления программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="9c125-144">Software update category.</span></span> <span data-ttu-id="9c125-145">Возможные значения: `critical`, `configurationDataFile`, `firmware`, `other`.</span><span class="sxs-lookup"><span data-stu-id="9c125-145">Possible values are: `critical`, `configurationDataFile`, `firmware`, `other`.</span></span>|
|<span data-ttu-id="9c125-146">updateVersion</span><span class="sxs-lookup"><span data-stu-id="9c125-146">updateVersion</span></span>|<span data-ttu-id="9c125-147">Строка</span><span class="sxs-lookup"><span data-stu-id="9c125-147">String</span></span>|<span data-ttu-id="9c125-148">Версия обновления программного обеспечения</span><span class="sxs-lookup"><span data-stu-id="9c125-148">Version of the software update</span></span>|
|<span data-ttu-id="9c125-149">state</span><span class="sxs-lookup"><span data-stu-id="9c125-149">state</span></span>|[<span data-ttu-id="9c125-150">macOSSoftwareUpdateState</span><span class="sxs-lookup"><span data-stu-id="9c125-150">macOSSoftwareUpdateState</span></span>](../resources/intune-deviceconfig-macossoftwareupdatestate.md)|<span data-ttu-id="9c125-151">Состояние обновления программного обеспечения.</span><span class="sxs-lookup"><span data-stu-id="9c125-151">State of the software update.</span></span> <span data-ttu-id="9c125-152">Возможные значения: `success` `downloading` , , , , , `downloaded` , `installing` , `idle` `available` `scheduled` `downloadFailed` `downloadInsufficientSpace` , `downloadInsufficientPower` `downloadInsufficientNetwork` `installInsufficientSpace` `installInsufficientPower` `installFailed` `commandFailed` , .</span><span class="sxs-lookup"><span data-stu-id="9c125-152">Possible values are: `success`, `downloading`, `downloaded`, `installing`, `idle`, `available`, `scheduled`, `downloadFailed`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installInsufficientSpace`, `installInsufficientPower`, `installFailed`, `commandFailed`.</span></span>|
|<span data-ttu-id="9c125-153">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c125-153">lastUpdatedDateTime</span></span>|<span data-ttu-id="9c125-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c125-154">DateTimeOffset</span></span>|<span data-ttu-id="9c125-155">Последний раз, когда отчет для этого устройства и ключ продукта был обновлен.</span><span class="sxs-lookup"><span data-stu-id="9c125-155">Last date time the report for this device and product key was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="9c125-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c125-156">Response</span></span>
<span data-ttu-id="9c125-157">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9c125-157">If successful, this method returns a `200 OK` response code and an updated [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c125-158">Пример</span><span class="sxs-lookup"><span data-stu-id="9c125-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c125-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c125-159">Request</span></span>
<span data-ttu-id="9c125-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c125-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9c125-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c125-161">Response</span></span>
<span data-ttu-id="9c125-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9c125-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




