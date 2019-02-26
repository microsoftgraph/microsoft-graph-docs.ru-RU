---
title: Обновление объекта deviceConfigurationDeviceStateSummary
description: Обновление свойств объекта deviceConfigurationDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 816612ef041bf71dbd2e9f2ebf7b3b212892322b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156121"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="682f6-103">Обновление объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="682f6-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="682f6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="682f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="682f6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="682f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="682f6-106">Обновление свойств объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="682f6-106">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="682f6-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="682f6-107">Prerequisites</span></span>
<span data-ttu-id="682f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="682f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="682f6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="682f6-110">Permission type</span></span>|<span data-ttu-id="682f6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="682f6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="682f6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="682f6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="682f6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="682f6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="682f6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="682f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="682f6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="682f6-115">Not supported.</span></span>|
|<span data-ttu-id="682f6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="682f6-116">Application</span></span>|<span data-ttu-id="682f6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="682f6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="682f6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="682f6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="682f6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="682f6-119">Request headers</span></span>
|<span data-ttu-id="682f6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="682f6-120">Header</span></span>|<span data-ttu-id="682f6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="682f6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="682f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="682f6-122">Authorization</span></span>|<span data-ttu-id="682f6-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="682f6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="682f6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="682f6-124">Accept</span></span>|<span data-ttu-id="682f6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="682f6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="682f6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="682f6-126">Request body</span></span>
<span data-ttu-id="682f6-127">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="682f6-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="682f6-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="682f6-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="682f6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="682f6-129">Property</span></span>|<span data-ttu-id="682f6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="682f6-130">Type</span></span>|<span data-ttu-id="682f6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="682f6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="682f6-132">id</span><span class="sxs-lookup"><span data-stu-id="682f6-132">id</span></span>|<span data-ttu-id="682f6-133">String</span><span class="sxs-lookup"><span data-stu-id="682f6-133">String</span></span>|<span data-ttu-id="682f6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="682f6-134">Key of the entity.</span></span>|
|<span data-ttu-id="682f6-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="682f6-135">unknownDeviceCount</span></span>|<span data-ttu-id="682f6-136">Int32</span><span class="sxs-lookup"><span data-stu-id="682f6-136">Int32</span></span>|<span data-ttu-id="682f6-137">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="682f6-137">Number of unknown devices</span></span>|
|<span data-ttu-id="682f6-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="682f6-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="682f6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="682f6-139">Int32</span></span>|<span data-ttu-id="682f6-140">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="682f6-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="682f6-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="682f6-141">compliantDeviceCount</span></span>|<span data-ttu-id="682f6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="682f6-142">Int32</span></span>|<span data-ttu-id="682f6-143">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="682f6-143">Number of compliant devices</span></span>|
|<span data-ttu-id="682f6-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="682f6-144">remediatedDeviceCount</span></span>|<span data-ttu-id="682f6-145">Int32</span><span class="sxs-lookup"><span data-stu-id="682f6-145">Int32</span></span>|<span data-ttu-id="682f6-146">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="682f6-146">Number of remediated devices</span></span>|
|<span data-ttu-id="682f6-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="682f6-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="682f6-148">Int32</span><span class="sxs-lookup"><span data-stu-id="682f6-148">Int32</span></span>|<span data-ttu-id="682f6-149">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="682f6-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="682f6-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="682f6-150">errorDeviceCount</span></span>|<span data-ttu-id="682f6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="682f6-151">Int32</span></span>|<span data-ttu-id="682f6-152">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="682f6-152">Number of error devices</span></span>|
|<span data-ttu-id="682f6-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="682f6-153">conflictDeviceCount</span></span>|<span data-ttu-id="682f6-154">Int32</span><span class="sxs-lookup"><span data-stu-id="682f6-154">Int32</span></span>|<span data-ttu-id="682f6-155">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="682f6-155">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="682f6-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="682f6-156">Response</span></span>
<span data-ttu-id="682f6-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="682f6-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="682f6-158">Пример</span><span class="sxs-lookup"><span data-stu-id="682f6-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="682f6-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="682f6-159">Request</span></span>
<span data-ttu-id="682f6-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="682f6-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="682f6-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="682f6-161">Response</span></span>
<span data-ttu-id="682f6-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="682f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```




