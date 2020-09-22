---
title: Создание Секуритибаселинекатегористатесуммари
description: Создание нового объекта Секуритибаселинекатегористатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b375538d5d5492e5f3c3942f44645ee12399b3af
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088211"
---
# <a name="create-securitybaselinecategorystatesummary"></a><span data-ttu-id="de0dd-103">Создание Секуритибаселинекатегористатесуммари</span><span class="sxs-lookup"><span data-stu-id="de0dd-103">Create securityBaselineCategoryStateSummary</span></span>

<span data-ttu-id="de0dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de0dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de0dd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de0dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de0dd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de0dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de0dd-107">Создание нового объекта [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="de0dd-107">Create a new [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de0dd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="de0dd-108">Prerequisites</span></span>
<span data-ttu-id="de0dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de0dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de0dd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de0dd-111">Permission type</span></span>|<span data-ttu-id="de0dd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de0dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de0dd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de0dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de0dd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de0dd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de0dd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de0dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de0dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de0dd-116">Not supported.</span></span>|
|<span data-ttu-id="de0dd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de0dd-117">Application</span></span>|<span data-ttu-id="de0dd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de0dd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de0dd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de0dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="de0dd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="de0dd-120">Request headers</span></span>
|<span data-ttu-id="de0dd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de0dd-121">Header</span></span>|<span data-ttu-id="de0dd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="de0dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de0dd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de0dd-123">Authorization</span></span>|<span data-ttu-id="de0dd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de0dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de0dd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="de0dd-125">Accept</span></span>|<span data-ttu-id="de0dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de0dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de0dd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de0dd-127">Request body</span></span>
<span data-ttu-id="de0dd-128">В тексте запроса добавьте представление объекта Секуритибаселинекатегористатесуммари в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de0dd-128">In the request body, supply a JSON representation for the securityBaselineCategoryStateSummary object.</span></span>

<span data-ttu-id="de0dd-129">В следующей таблице приведены свойства, необходимые при создании Секуритибаселинекатегористатесуммари.</span><span class="sxs-lookup"><span data-stu-id="de0dd-129">The following table shows the properties that are required when you create the securityBaselineCategoryStateSummary.</span></span>

|<span data-ttu-id="de0dd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="de0dd-130">Property</span></span>|<span data-ttu-id="de0dd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="de0dd-131">Type</span></span>|<span data-ttu-id="de0dd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="de0dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de0dd-133">id</span><span class="sxs-lookup"><span data-stu-id="de0dd-133">id</span></span>|<span data-ttu-id="de0dd-134">Строка</span><span class="sxs-lookup"><span data-stu-id="de0dd-134">String</span></span>|<span data-ttu-id="de0dd-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="de0dd-135">Unique identifier of the entity.</span></span> <span data-ttu-id="de0dd-136">Наследуется от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="de0dd-136">Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="de0dd-137">секурекаунт</span><span class="sxs-lookup"><span data-stu-id="de0dd-137">secureCount</span></span>|<span data-ttu-id="de0dd-138">Int32</span><span class="sxs-lookup"><span data-stu-id="de0dd-138">Int32</span></span>|<span data-ttu-id="de0dd-139">Количество защищенных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="de0dd-139">Number of secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="de0dd-140">нотсекурекаунт</span><span class="sxs-lookup"><span data-stu-id="de0dd-140">notSecureCount</span></span>|<span data-ttu-id="de0dd-141">Int32</span><span class="sxs-lookup"><span data-stu-id="de0dd-141">Int32</span></span>|<span data-ttu-id="de0dd-142">Количество незащищенных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="de0dd-142">Number of not secure devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="de0dd-143">unknownCount</span><span class="sxs-lookup"><span data-stu-id="de0dd-143">unknownCount</span></span>|<span data-ttu-id="de0dd-144">Int32</span><span class="sxs-lookup"><span data-stu-id="de0dd-144">Int32</span></span>|<span data-ttu-id="de0dd-145">Количество неизвестных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="de0dd-145">Number of unknown devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="de0dd-146">errorCount</span><span class="sxs-lookup"><span data-stu-id="de0dd-146">errorCount</span></span>|<span data-ttu-id="de0dd-147">Int32</span><span class="sxs-lookup"><span data-stu-id="de0dd-147">Int32</span></span>|<span data-ttu-id="de0dd-148">Количество устройств с ошибками, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="de0dd-148">Number of error devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="de0dd-149">conflictCount</span><span class="sxs-lookup"><span data-stu-id="de0dd-149">conflictCount</span></span>|<span data-ttu-id="de0dd-150">Int32</span><span class="sxs-lookup"><span data-stu-id="de0dd-150">Int32</span></span>|<span data-ttu-id="de0dd-151">Количество устройств с конфликтами, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="de0dd-151">Number of conflict devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="de0dd-152">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="de0dd-152">notApplicableCount</span></span>|<span data-ttu-id="de0dd-153">Int32</span><span class="sxs-lookup"><span data-stu-id="de0dd-153">Int32</span></span>|<span data-ttu-id="de0dd-154">Количество неприменимых устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="de0dd-154">Number of not applicable devices Inherited from [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span></span>|
|<span data-ttu-id="de0dd-155">displayName</span><span class="sxs-lookup"><span data-stu-id="de0dd-155">displayName</span></span>|<span data-ttu-id="de0dd-156">Строка</span><span class="sxs-lookup"><span data-stu-id="de0dd-156">String</span></span>|<span data-ttu-id="de0dd-157">Имя категории</span><span class="sxs-lookup"><span data-stu-id="de0dd-157">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="de0dd-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="de0dd-158">Response</span></span>
<span data-ttu-id="de0dd-159">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de0dd-159">If successful, this method returns a `201 Created` response code and a [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de0dd-160">Пример</span><span class="sxs-lookup"><span data-stu-id="de0dd-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="de0dd-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="de0dd-161">Request</span></span>
<span data-ttu-id="de0dd-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de0dd-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
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

### <a name="response"></a><span data-ttu-id="de0dd-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="de0dd-163">Response</span></span>
<span data-ttu-id="de0dd-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de0dd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






