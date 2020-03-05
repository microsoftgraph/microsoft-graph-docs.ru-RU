---
title: Обновление Секуритибаселинестатесуммари
description: Обновление свойств объекта Секуритибаселинестатесуммари.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a3943589d6dda429c95359182aaa8fd4bc2d510
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470184"
---
# <a name="update-securitybaselinestatesummary"></a><span data-ttu-id="0fb59-103">Обновление Секуритибаселинестатесуммари</span><span class="sxs-lookup"><span data-stu-id="0fb59-103">Update securityBaselineStateSummary</span></span>

<span data-ttu-id="0fb59-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0fb59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fb59-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fb59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fb59-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0fb59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fb59-107">Обновление свойств объекта [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="0fb59-107">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fb59-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0fb59-108">Prerequisites</span></span>
<span data-ttu-id="0fb59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fb59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fb59-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fb59-111">Permission type</span></span>|<span data-ttu-id="0fb59-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fb59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fb59-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fb59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0fb59-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fb59-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0fb59-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fb59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fb59-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fb59-116">Not supported.</span></span>|
|<span data-ttu-id="0fb59-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fb59-117">Application</span></span>|<span data-ttu-id="0fb59-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fb59-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fb59-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fb59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="0fb59-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0fb59-120">Request headers</span></span>
|<span data-ttu-id="0fb59-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0fb59-121">Header</span></span>|<span data-ttu-id="0fb59-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0fb59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fb59-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fb59-123">Authorization</span></span>|<span data-ttu-id="0fb59-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fb59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fb59-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0fb59-125">Accept</span></span>|<span data-ttu-id="0fb59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0fb59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fb59-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0fb59-127">Request body</span></span>
<span data-ttu-id="0fb59-128">В тексте запроса добавьте представление объекта [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0fb59-128">In the request body, supply a JSON representation for the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

<span data-ttu-id="0fb59-129">В следующей таблице приведены свойства, необходимые при создании [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="0fb59-129">The following table shows the properties that are required when you create the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span></span>

|<span data-ttu-id="0fb59-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0fb59-130">Property</span></span>|<span data-ttu-id="0fb59-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0fb59-131">Type</span></span>|<span data-ttu-id="0fb59-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0fb59-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fb59-133">id</span><span class="sxs-lookup"><span data-stu-id="0fb59-133">id</span></span>|<span data-ttu-id="0fb59-134">String</span><span class="sxs-lookup"><span data-stu-id="0fb59-134">String</span></span>|<span data-ttu-id="0fb59-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="0fb59-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="0fb59-136">секурекаунт</span><span class="sxs-lookup"><span data-stu-id="0fb59-136">secureCount</span></span>|<span data-ttu-id="0fb59-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb59-137">Int32</span></span>|<span data-ttu-id="0fb59-138">Количество защищенных устройств</span><span class="sxs-lookup"><span data-stu-id="0fb59-138">Number of secure devices</span></span>|
|<span data-ttu-id="0fb59-139">нотсекурекаунт</span><span class="sxs-lookup"><span data-stu-id="0fb59-139">notSecureCount</span></span>|<span data-ttu-id="0fb59-140">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb59-140">Int32</span></span>|<span data-ttu-id="0fb59-141">Количество незащищенных устройств</span><span class="sxs-lookup"><span data-stu-id="0fb59-141">Number of not secure devices</span></span>|
|<span data-ttu-id="0fb59-142">unknownCount</span><span class="sxs-lookup"><span data-stu-id="0fb59-142">unknownCount</span></span>|<span data-ttu-id="0fb59-143">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb59-143">Int32</span></span>|<span data-ttu-id="0fb59-144">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="0fb59-144">Number of unknown devices</span></span>|
|<span data-ttu-id="0fb59-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="0fb59-145">errorCount</span></span>|<span data-ttu-id="0fb59-146">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb59-146">Int32</span></span>|<span data-ttu-id="0fb59-147">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="0fb59-147">Number of error devices</span></span>|
|<span data-ttu-id="0fb59-148">conflictCount</span><span class="sxs-lookup"><span data-stu-id="0fb59-148">conflictCount</span></span>|<span data-ttu-id="0fb59-149">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb59-149">Int32</span></span>|<span data-ttu-id="0fb59-150">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="0fb59-150">Number of conflict devices</span></span>|
|<span data-ttu-id="0fb59-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="0fb59-151">notApplicableCount</span></span>|<span data-ttu-id="0fb59-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb59-152">Int32</span></span>|<span data-ttu-id="0fb59-153">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="0fb59-153">Number of not applicable devices</span></span>|



## <a name="response"></a><span data-ttu-id="0fb59-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fb59-154">Response</span></span>
<span data-ttu-id="0fb59-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0fb59-155">If successful, this method returns a `200 OK` response code and an updated [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fb59-156">Пример</span><span class="sxs-lookup"><span data-stu-id="0fb59-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fb59-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fb59-157">Request</span></span>
<span data-ttu-id="0fb59-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fb59-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0fb59-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fb59-159">Response</span></span>
<span data-ttu-id="0fb59-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0fb59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





