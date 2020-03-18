---
title: Обновление Секуритибаселинекатегористатесуммари
description: Обновление свойств объекта Секуритибаселинекатегористатесуммари.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: da5058853bb846b11388c7522d48ea2f0cbaec92
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764658"
---
# <a name="update-securitybaselinecategorystatesummary"></a><span data-ttu-id="449cc-103">Обновление Секуритибаселинекатегористатесуммари</span><span class="sxs-lookup"><span data-stu-id="449cc-103">Update securityBaselineCategoryStateSummary</span></span>

> <span data-ttu-id="449cc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="449cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="449cc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="449cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="449cc-106">Обновление свойств объекта [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="449cc-106">Update the properties of a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="449cc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="449cc-107">Prerequisites</span></span>
<span data-ttu-id="449cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="449cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="449cc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="449cc-110">Permission type</span></span>|<span data-ttu-id="449cc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="449cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="449cc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="449cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="449cc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="449cc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="449cc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="449cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="449cc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="449cc-115">Not supported.</span></span>|
|<span data-ttu-id="449cc-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="449cc-116">Application</span></span>|<span data-ttu-id="449cc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="449cc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="449cc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="449cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="449cc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="449cc-119">Request headers</span></span>
|<span data-ttu-id="449cc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="449cc-120">Header</span></span>|<span data-ttu-id="449cc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="449cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="449cc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="449cc-122">Authorization</span></span>|<span data-ttu-id="449cc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="449cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="449cc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="449cc-124">Accept</span></span>|<span data-ttu-id="449cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="449cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="449cc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="449cc-126">Request body</span></span>
<span data-ttu-id="449cc-127">В тексте запроса добавьте представление объекта [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="449cc-127">In the request body, supply a JSON representation for the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

<span data-ttu-id="449cc-128">В следующей таблице приведены свойства, необходимые при создании [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="449cc-128">The following table shows the properties that are required when you create the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span></span>

|<span data-ttu-id="449cc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="449cc-129">Property</span></span>|<span data-ttu-id="449cc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="449cc-130">Type</span></span>|<span data-ttu-id="449cc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="449cc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="449cc-132">id</span><span class="sxs-lookup"><span data-stu-id="449cc-132">id</span></span>|<span data-ttu-id="449cc-133">String</span><span class="sxs-lookup"><span data-stu-id="449cc-133">String</span></span>|<span data-ttu-id="449cc-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="449cc-134">Unique identifier of the entity.</span></span> <span data-ttu-id="449cc-135">Наследуется от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="449cc-135">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="449cc-136">секурекаунт</span><span class="sxs-lookup"><span data-stu-id="449cc-136">secureCount</span></span>|<span data-ttu-id="449cc-137">Int32</span><span class="sxs-lookup"><span data-stu-id="449cc-137">Int32</span></span>|<span data-ttu-id="449cc-138">Количество защищенных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="449cc-138">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="449cc-139">нотсекурекаунт</span><span class="sxs-lookup"><span data-stu-id="449cc-139">notSecureCount</span></span>|<span data-ttu-id="449cc-140">Int32</span><span class="sxs-lookup"><span data-stu-id="449cc-140">Int32</span></span>|<span data-ttu-id="449cc-141">Количество незащищенных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="449cc-141">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="449cc-142">unknownCount</span><span class="sxs-lookup"><span data-stu-id="449cc-142">unknownCount</span></span>|<span data-ttu-id="449cc-143">Int32</span><span class="sxs-lookup"><span data-stu-id="449cc-143">Int32</span></span>|<span data-ttu-id="449cc-144">Количество неизвестных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="449cc-144">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="449cc-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="449cc-145">errorCount</span></span>|<span data-ttu-id="449cc-146">Int32</span><span class="sxs-lookup"><span data-stu-id="449cc-146">Int32</span></span>|<span data-ttu-id="449cc-147">Количество устройств с ошибками, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="449cc-147">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="449cc-148">conflictCount</span><span class="sxs-lookup"><span data-stu-id="449cc-148">conflictCount</span></span>|<span data-ttu-id="449cc-149">Int32</span><span class="sxs-lookup"><span data-stu-id="449cc-149">Int32</span></span>|<span data-ttu-id="449cc-150">Количество устройств с конфликтами, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="449cc-150">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="449cc-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="449cc-151">notApplicableCount</span></span>|<span data-ttu-id="449cc-152">Int32</span><span class="sxs-lookup"><span data-stu-id="449cc-152">Int32</span></span>|<span data-ttu-id="449cc-153">Количество неприменимых устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="449cc-153">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="449cc-154">displayName</span><span class="sxs-lookup"><span data-stu-id="449cc-154">displayName</span></span>|<span data-ttu-id="449cc-155">Строка</span><span class="sxs-lookup"><span data-stu-id="449cc-155">String</span></span>|<span data-ttu-id="449cc-156">Имя категории</span><span class="sxs-lookup"><span data-stu-id="449cc-156">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="449cc-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="449cc-157">Response</span></span>
<span data-ttu-id="449cc-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="449cc-158">If successful, this method returns a `200 OK` response code and an updated [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="449cc-159">Пример</span><span class="sxs-lookup"><span data-stu-id="449cc-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="449cc-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="449cc-160">Request</span></span>
<span data-ttu-id="449cc-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="449cc-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
Content-type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="449cc-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="449cc-162">Response</span></span>
<span data-ttu-id="449cc-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="449cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "7a650997-0997-7a65-9709-657a9709657a",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```




