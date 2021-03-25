---
title: Обновление securityBaselineStateSummary
description: Обновление свойств объекта securityBaselineStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: de1db7428f19e07f6bf7d349b00d995d93d0a660
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154520"
---
# <a name="update-securitybaselinestatesummary"></a><span data-ttu-id="1edbe-103">Обновление securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="1edbe-103">Update securityBaselineStateSummary</span></span>

<span data-ttu-id="1edbe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1edbe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1edbe-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1edbe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1edbe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1edbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1edbe-107">Обновление свойств объекта [securityBaselineStateSummary.](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="1edbe-107">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1edbe-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1edbe-108">Prerequisites</span></span>
<span data-ttu-id="1edbe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1edbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1edbe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1edbe-111">Permission type</span></span>|<span data-ttu-id="1edbe-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1edbe-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1edbe-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1edbe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1edbe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1edbe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1edbe-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1edbe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1edbe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1edbe-116">Not supported.</span></span>|
|<span data-ttu-id="1edbe-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1edbe-117">Application</span></span>|<span data-ttu-id="1edbe-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1edbe-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1edbe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1edbe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="1edbe-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1edbe-120">Request headers</span></span>
|<span data-ttu-id="1edbe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1edbe-121">Header</span></span>|<span data-ttu-id="1edbe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1edbe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1edbe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1edbe-123">Authorization</span></span>|<span data-ttu-id="1edbe-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1edbe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1edbe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1edbe-125">Accept</span></span>|<span data-ttu-id="1edbe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1edbe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1edbe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1edbe-127">Request body</span></span>
<span data-ttu-id="1edbe-128">В теле запроса поставляем представление JSON для [объекта securityBaselineStateSummary.](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="1edbe-128">In the request body, supply a JSON representation for the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>

<span data-ttu-id="1edbe-129">В следующей таблице показаны свойства, необходимые при создании [securityBaselineStateSummary.](../resources/intune-deviceintent-securitybaselinestatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="1edbe-129">The following table shows the properties that are required when you create the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md).</span></span>

|<span data-ttu-id="1edbe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1edbe-130">Property</span></span>|<span data-ttu-id="1edbe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1edbe-131">Type</span></span>|<span data-ttu-id="1edbe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1edbe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1edbe-133">id</span><span class="sxs-lookup"><span data-stu-id="1edbe-133">id</span></span>|<span data-ttu-id="1edbe-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1edbe-134">String</span></span>|<span data-ttu-id="1edbe-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="1edbe-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="1edbe-136">secureCount</span><span class="sxs-lookup"><span data-stu-id="1edbe-136">secureCount</span></span>|<span data-ttu-id="1edbe-137">Int32</span><span class="sxs-lookup"><span data-stu-id="1edbe-137">Int32</span></span>|<span data-ttu-id="1edbe-138">Количество защищенных устройств</span><span class="sxs-lookup"><span data-stu-id="1edbe-138">Number of secure devices</span></span>|
|<span data-ttu-id="1edbe-139">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="1edbe-139">notSecureCount</span></span>|<span data-ttu-id="1edbe-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1edbe-140">Int32</span></span>|<span data-ttu-id="1edbe-141">Число небезопасных устройств</span><span class="sxs-lookup"><span data-stu-id="1edbe-141">Number of not secure devices</span></span>|
|<span data-ttu-id="1edbe-142">unknownCount</span><span class="sxs-lookup"><span data-stu-id="1edbe-142">unknownCount</span></span>|<span data-ttu-id="1edbe-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1edbe-143">Int32</span></span>|<span data-ttu-id="1edbe-144">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="1edbe-144">Number of unknown devices</span></span>|
|<span data-ttu-id="1edbe-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="1edbe-145">errorCount</span></span>|<span data-ttu-id="1edbe-146">Int32</span><span class="sxs-lookup"><span data-stu-id="1edbe-146">Int32</span></span>|<span data-ttu-id="1edbe-147">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="1edbe-147">Number of error devices</span></span>|
|<span data-ttu-id="1edbe-148">conflictCount</span><span class="sxs-lookup"><span data-stu-id="1edbe-148">conflictCount</span></span>|<span data-ttu-id="1edbe-149">Int32</span><span class="sxs-lookup"><span data-stu-id="1edbe-149">Int32</span></span>|<span data-ttu-id="1edbe-150">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="1edbe-150">Number of conflict devices</span></span>|
|<span data-ttu-id="1edbe-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="1edbe-151">notApplicableCount</span></span>|<span data-ttu-id="1edbe-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1edbe-152">Int32</span></span>|<span data-ttu-id="1edbe-153">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="1edbe-153">Number of not applicable devices</span></span>|



## <a name="response"></a><span data-ttu-id="1edbe-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="1edbe-154">Response</span></span>
<span data-ttu-id="1edbe-155">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1edbe-155">If successful, this method returns a `200 OK` response code and an updated [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1edbe-156">Пример</span><span class="sxs-lookup"><span data-stu-id="1edbe-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="1edbe-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="1edbe-157">Request</span></span>
<span data-ttu-id="1edbe-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1edbe-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1edbe-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="1edbe-159">Response</span></span>
<span data-ttu-id="1edbe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1edbe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




