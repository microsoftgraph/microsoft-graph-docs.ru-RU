---
title: Обновление объекта deviceConfigurationDeviceStateSummary
description: Обновление свойств объекта deviceConfigurationDeviceStateSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 41b092aa651d8526618f8287c7a90ff9673c7508
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408553"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="e9aeb-103">Обновление объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="e9aeb-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="e9aeb-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e9aeb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9aeb-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9aeb-107">Обновление свойств объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e9aeb-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9aeb-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e9aeb-108">Prerequisites</span></span>
<span data-ttu-id="e9aeb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e9aeb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e9aeb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9aeb-111">Permission type</span></span>|<span data-ttu-id="e9aeb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9aeb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9aeb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9aeb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9aeb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9aeb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e9aeb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9aeb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9aeb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-116">Not supported.</span></span>|
|<span data-ttu-id="e9aeb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9aeb-117">Application</span></span>|<span data-ttu-id="e9aeb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9aeb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9aeb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="e9aeb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9aeb-120">Request headers</span></span>
|<span data-ttu-id="e9aeb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9aeb-121">Header</span></span>|<span data-ttu-id="e9aeb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e9aeb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9aeb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9aeb-123">Authorization</span></span>|<span data-ttu-id="e9aeb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e9aeb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9aeb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9aeb-125">Accept</span></span>|<span data-ttu-id="e9aeb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9aeb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9aeb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9aeb-127">Request body</span></span>
<span data-ttu-id="e9aeb-128">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="e9aeb-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="e9aeb-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="e9aeb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9aeb-130">Property</span></span>|<span data-ttu-id="e9aeb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e9aeb-131">Type</span></span>|<span data-ttu-id="e9aeb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e9aeb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9aeb-133">id</span><span class="sxs-lookup"><span data-stu-id="e9aeb-133">id</span></span>|<span data-ttu-id="e9aeb-134">String</span><span class="sxs-lookup"><span data-stu-id="e9aeb-134">String</span></span>|<span data-ttu-id="e9aeb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-135">Key of the entity.</span></span>|
|<span data-ttu-id="e9aeb-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e9aeb-136">unknownDeviceCount</span></span>|<span data-ttu-id="e9aeb-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e9aeb-137">Int32</span></span>|<span data-ttu-id="e9aeb-138">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-138">Number of unknown devices</span></span>|
|<span data-ttu-id="e9aeb-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e9aeb-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="e9aeb-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e9aeb-140">Int32</span></span>|<span data-ttu-id="e9aeb-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="e9aeb-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e9aeb-142">compliantDeviceCount</span></span>|<span data-ttu-id="e9aeb-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e9aeb-143">Int32</span></span>|<span data-ttu-id="e9aeb-144">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-144">Number of compliant devices</span></span>|
|<span data-ttu-id="e9aeb-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e9aeb-145">remediatedDeviceCount</span></span>|<span data-ttu-id="e9aeb-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e9aeb-146">Int32</span></span>|<span data-ttu-id="e9aeb-147">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-147">Number of remediated devices</span></span>|
|<span data-ttu-id="e9aeb-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e9aeb-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e9aeb-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e9aeb-149">Int32</span></span>|<span data-ttu-id="e9aeb-150">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="e9aeb-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e9aeb-151">errorDeviceCount</span></span>|<span data-ttu-id="e9aeb-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e9aeb-152">Int32</span></span>|<span data-ttu-id="e9aeb-153">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-153">Number of error devices</span></span>|
|<span data-ttu-id="e9aeb-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e9aeb-154">conflictDeviceCount</span></span>|<span data-ttu-id="e9aeb-155">Int32</span><span class="sxs-lookup"><span data-stu-id="e9aeb-155">Int32</span></span>|<span data-ttu-id="e9aeb-156">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="e9aeb-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9aeb-157">Response</span></span>
<span data-ttu-id="e9aeb-158">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9aeb-159">Пример</span><span class="sxs-lookup"><span data-stu-id="e9aeb-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9aeb-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9aeb-160">Request</span></span>
<span data-ttu-id="e9aeb-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e9aeb-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9aeb-162">Response</span></span>
<span data-ttu-id="e9aeb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e9aeb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




