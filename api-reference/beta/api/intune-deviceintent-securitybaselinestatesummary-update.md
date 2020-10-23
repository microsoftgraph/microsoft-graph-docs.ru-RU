---
title: Обновление Секуритибаселинестатесуммари
description: Обновление свойств объекта Секуритибаселинестатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2cbad348157ddeac184ec6663d3558535418d2a1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729989"
---
# <a name="update-securitybaselinestatesummary"></a><span data-ttu-id="9cf09-103">Обновление Секуритибаселинестатесуммари</span><span class="sxs-lookup"><span data-stu-id="9cf09-103">Update securityBaselineStateSummary</span></span>

<span data-ttu-id="9cf09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cf09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9cf09-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cf09-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cf09-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9cf09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cf09-107">Обновление свойств объекта [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="9cf09-107">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cf09-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9cf09-108">Prerequisites</span></span>
<span data-ttu-id="9cf09-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cf09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cf09-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cf09-111">Permission type</span></span>|<span data-ttu-id="9cf09-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9cf09-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cf09-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cf09-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9cf09-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cf09-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9cf09-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cf09-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cf09-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cf09-116">Not supported.</span></span>|
|<span data-ttu-id="9cf09-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9cf09-117">Application</span></span>|<span data-ttu-id="9cf09-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cf09-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cf09-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cf09-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="9cf09-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9cf09-120">Request headers</span></span>
|<span data-ttu-id="9cf09-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9cf09-121">Header</span></span>|<span data-ttu-id="9cf09-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9cf09-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cf09-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9cf09-123">Authorization</span></span>|<span data-ttu-id="9cf09-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9cf09-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cf09-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9cf09-125">Accept</span></span>|<span data-ttu-id="9cf09-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9cf09-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cf09-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9cf09-127">Request body</span></span>
<span data-ttu-id="9cf09-128">В тексте запроса добавьте представление объекта [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9cf09-128">In the request body, supply a JSON representation for the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

<span data-ttu-id="9cf09-129">В следующей таблице приведены свойства, необходимые при создании [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="9cf09-129">The following table shows the properties that are required when you create the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span></span>

|<span data-ttu-id="9cf09-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cf09-130">Property</span></span>|<span data-ttu-id="9cf09-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9cf09-131">Type</span></span>|<span data-ttu-id="9cf09-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9cf09-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cf09-133">id</span><span class="sxs-lookup"><span data-stu-id="9cf09-133">id</span></span>|<span data-ttu-id="9cf09-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9cf09-134">String</span></span>|<span data-ttu-id="9cf09-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="9cf09-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="9cf09-136">секурекаунт</span><span class="sxs-lookup"><span data-stu-id="9cf09-136">secureCount</span></span>|<span data-ttu-id="9cf09-137">Int32</span><span class="sxs-lookup"><span data-stu-id="9cf09-137">Int32</span></span>|<span data-ttu-id="9cf09-138">Количество защищенных устройств</span><span class="sxs-lookup"><span data-stu-id="9cf09-138">Number of secure devices</span></span>|
|<span data-ttu-id="9cf09-139">нотсекурекаунт</span><span class="sxs-lookup"><span data-stu-id="9cf09-139">notSecureCount</span></span>|<span data-ttu-id="9cf09-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9cf09-140">Int32</span></span>|<span data-ttu-id="9cf09-141">Количество незащищенных устройств</span><span class="sxs-lookup"><span data-stu-id="9cf09-141">Number of not secure devices</span></span>|
|<span data-ttu-id="9cf09-142">unknownCount</span><span class="sxs-lookup"><span data-stu-id="9cf09-142">unknownCount</span></span>|<span data-ttu-id="9cf09-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9cf09-143">Int32</span></span>|<span data-ttu-id="9cf09-144">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="9cf09-144">Number of unknown devices</span></span>|
|<span data-ttu-id="9cf09-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="9cf09-145">errorCount</span></span>|<span data-ttu-id="9cf09-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9cf09-146">Int32</span></span>|<span data-ttu-id="9cf09-147">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="9cf09-147">Number of error devices</span></span>|
|<span data-ttu-id="9cf09-148">conflictCount</span><span class="sxs-lookup"><span data-stu-id="9cf09-148">conflictCount</span></span>|<span data-ttu-id="9cf09-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9cf09-149">Int32</span></span>|<span data-ttu-id="9cf09-150">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="9cf09-150">Number of conflict devices</span></span>|
|<span data-ttu-id="9cf09-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="9cf09-151">notApplicableCount</span></span>|<span data-ttu-id="9cf09-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9cf09-152">Int32</span></span>|<span data-ttu-id="9cf09-153">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="9cf09-153">Number of not applicable devices</span></span>|



## <a name="response"></a><span data-ttu-id="9cf09-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="9cf09-154">Response</span></span>
<span data-ttu-id="9cf09-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9cf09-155">If successful, this method returns a `200 OK` response code and an updated [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cf09-156">Пример</span><span class="sxs-lookup"><span data-stu-id="9cf09-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cf09-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cf09-157">Request</span></span>
<span data-ttu-id="9cf09-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9cf09-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
Content-type: application/json
Content-length: 213

{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2
}
```

### <a name="response"></a><span data-ttu-id="9cf09-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cf09-159">Response</span></span>
<span data-ttu-id="9cf09-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9cf09-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 262

{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "a4da796f-796f-a4da-6f79-daa46f79daa4",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2
}
```





