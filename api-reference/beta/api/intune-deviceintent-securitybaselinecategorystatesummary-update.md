---
title: Обновление Секуритибаселинекатегористатесуммари
description: Обновление свойств объекта Секуритибаселинекатегористатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 96e6449f4d64e1a6e61912abe452afe2ef11d255
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726103"
---
# <a name="update-securitybaselinecategorystatesummary"></a><span data-ttu-id="4734c-103">Обновление Секуритибаселинекатегористатесуммари</span><span class="sxs-lookup"><span data-stu-id="4734c-103">Update securityBaselineCategoryStateSummary</span></span>

<span data-ttu-id="4734c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4734c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4734c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4734c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4734c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4734c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4734c-107">Обновление свойств объекта [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="4734c-107">Update the properties of a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4734c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4734c-108">Prerequisites</span></span>
<span data-ttu-id="4734c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4734c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4734c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4734c-111">Permission type</span></span>|<span data-ttu-id="4734c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4734c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4734c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4734c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4734c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4734c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4734c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4734c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4734c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4734c-116">Not supported.</span></span>|
|<span data-ttu-id="4734c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4734c-117">Application</span></span>|<span data-ttu-id="4734c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4734c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4734c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4734c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries/{securityBaselineCategoryStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="4734c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4734c-120">Request headers</span></span>
|<span data-ttu-id="4734c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4734c-121">Header</span></span>|<span data-ttu-id="4734c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4734c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4734c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4734c-123">Authorization</span></span>|<span data-ttu-id="4734c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4734c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4734c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4734c-125">Accept</span></span>|<span data-ttu-id="4734c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4734c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4734c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4734c-127">Request body</span></span>
<span data-ttu-id="4734c-128">В тексте запроса добавьте представление объекта [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4734c-128">In the request body, supply a JSON representation for the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

<span data-ttu-id="4734c-129">В следующей таблице приведены свойства, необходимые при создании [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4734c-129">The following table shows the properties that are required when you create the [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).</span></span>

|<span data-ttu-id="4734c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4734c-130">Property</span></span>|<span data-ttu-id="4734c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4734c-131">Type</span></span>|<span data-ttu-id="4734c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4734c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4734c-133">id</span><span class="sxs-lookup"><span data-stu-id="4734c-133">id</span></span>|<span data-ttu-id="4734c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4734c-134">String</span></span>|<span data-ttu-id="4734c-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="4734c-135">Unique identifier of the entity.</span></span> <span data-ttu-id="4734c-136">Наследуется от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="4734c-136">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="4734c-137">секурекаунт</span><span class="sxs-lookup"><span data-stu-id="4734c-137">secureCount</span></span>|<span data-ttu-id="4734c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="4734c-138">Int32</span></span>|<span data-ttu-id="4734c-139">Количество защищенных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="4734c-139">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="4734c-140">нотсекурекаунт</span><span class="sxs-lookup"><span data-stu-id="4734c-140">notSecureCount</span></span>|<span data-ttu-id="4734c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="4734c-141">Int32</span></span>|<span data-ttu-id="4734c-142">Количество незащищенных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="4734c-142">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="4734c-143">unknownCount</span><span class="sxs-lookup"><span data-stu-id="4734c-143">unknownCount</span></span>|<span data-ttu-id="4734c-144">Int32</span><span class="sxs-lookup"><span data-stu-id="4734c-144">Int32</span></span>|<span data-ttu-id="4734c-145">Количество неизвестных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="4734c-145">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="4734c-146">errorCount</span><span class="sxs-lookup"><span data-stu-id="4734c-146">errorCount</span></span>|<span data-ttu-id="4734c-147">Int32</span><span class="sxs-lookup"><span data-stu-id="4734c-147">Int32</span></span>|<span data-ttu-id="4734c-148">Количество устройств с ошибками, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="4734c-148">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="4734c-149">conflictCount</span><span class="sxs-lookup"><span data-stu-id="4734c-149">conflictCount</span></span>|<span data-ttu-id="4734c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="4734c-150">Int32</span></span>|<span data-ttu-id="4734c-151">Количество устройств с конфликтами, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="4734c-151">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="4734c-152">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="4734c-152">notApplicableCount</span></span>|<span data-ttu-id="4734c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4734c-153">Int32</span></span>|<span data-ttu-id="4734c-154">Количество неприменимых устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="4734c-154">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="4734c-155">displayName</span><span class="sxs-lookup"><span data-stu-id="4734c-155">displayName</span></span>|<span data-ttu-id="4734c-156">Строка</span><span class="sxs-lookup"><span data-stu-id="4734c-156">String</span></span>|<span data-ttu-id="4734c-157">Имя категории</span><span class="sxs-lookup"><span data-stu-id="4734c-157">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="4734c-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="4734c-158">Response</span></span>
<span data-ttu-id="4734c-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4734c-159">If successful, this method returns a `200 OK` response code and an updated [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4734c-160">Пример</span><span class="sxs-lookup"><span data-stu-id="4734c-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="4734c-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="4734c-161">Request</span></span>
<span data-ttu-id="4734c-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4734c-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4734c-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="4734c-163">Response</span></span>
<span data-ttu-id="4734c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4734c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





