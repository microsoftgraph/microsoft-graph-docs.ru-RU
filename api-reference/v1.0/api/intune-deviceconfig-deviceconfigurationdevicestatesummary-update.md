---
title: Обновление объекта deviceConfigurationDeviceStateSummary
description: Обновление свойств объекта deviceConfigurationDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 456932e8561604acaaa596e9240d6ea034b71165
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254347"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="5a942-103">Обновление объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="5a942-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="5a942-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a942-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a942-105">Обновление свойств объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="5a942-105">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a942-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5a942-106">Prerequisites</span></span>
<span data-ttu-id="5a942-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5a942-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5a942-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a942-109">Permission type</span></span>|<span data-ttu-id="5a942-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a942-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a942-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a942-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5a942-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a942-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5a942-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a942-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a942-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a942-114">Not supported.</span></span>|
|<span data-ttu-id="5a942-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a942-115">Application</span></span>|<span data-ttu-id="5a942-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a942-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a942-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a942-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="5a942-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a942-118">Request headers</span></span>
|<span data-ttu-id="5a942-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a942-119">Header</span></span>|<span data-ttu-id="5a942-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5a942-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a942-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a942-121">Authorization</span></span>|<span data-ttu-id="5a942-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5a942-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a942-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5a942-123">Accept</span></span>|<span data-ttu-id="5a942-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5a942-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a942-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a942-125">Request body</span></span>
<span data-ttu-id="5a942-126">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a942-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="5a942-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="5a942-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="5a942-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a942-128">Property</span></span>|<span data-ttu-id="5a942-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5a942-129">Type</span></span>|<span data-ttu-id="5a942-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5a942-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a942-131">id</span><span class="sxs-lookup"><span data-stu-id="5a942-131">id</span></span>|<span data-ttu-id="5a942-132">String</span><span class="sxs-lookup"><span data-stu-id="5a942-132">String</span></span>|<span data-ttu-id="5a942-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5a942-133">Key of the entity.</span></span>|
|<span data-ttu-id="5a942-134">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a942-134">unknownDeviceCount</span></span>|<span data-ttu-id="5a942-135">Int32</span><span class="sxs-lookup"><span data-stu-id="5a942-135">Int32</span></span>|<span data-ttu-id="5a942-136">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="5a942-136">Number of unknown devices</span></span>|
|<span data-ttu-id="5a942-137">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a942-137">notApplicableDeviceCount</span></span>|<span data-ttu-id="5a942-138">Int32</span><span class="sxs-lookup"><span data-stu-id="5a942-138">Int32</span></span>|<span data-ttu-id="5a942-139">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="5a942-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="5a942-140">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a942-140">compliantDeviceCount</span></span>|<span data-ttu-id="5a942-141">Int32</span><span class="sxs-lookup"><span data-stu-id="5a942-141">Int32</span></span>|<span data-ttu-id="5a942-142">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="5a942-142">Number of compliant devices</span></span>|
|<span data-ttu-id="5a942-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a942-143">remediatedDeviceCount</span></span>|<span data-ttu-id="5a942-144">Int32</span><span class="sxs-lookup"><span data-stu-id="5a942-144">Int32</span></span>|<span data-ttu-id="5a942-145">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="5a942-145">Number of remediated devices</span></span>|
|<span data-ttu-id="5a942-146">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a942-146">nonCompliantDeviceCount</span></span>|<span data-ttu-id="5a942-147">Int32</span><span class="sxs-lookup"><span data-stu-id="5a942-147">Int32</span></span>|<span data-ttu-id="5a942-148">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="5a942-148">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="5a942-149">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a942-149">errorDeviceCount</span></span>|<span data-ttu-id="5a942-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5a942-150">Int32</span></span>|<span data-ttu-id="5a942-151">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="5a942-151">Number of error devices</span></span>|
|<span data-ttu-id="5a942-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5a942-152">conflictDeviceCount</span></span>|<span data-ttu-id="5a942-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5a942-153">Int32</span></span>|<span data-ttu-id="5a942-154">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="5a942-154">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="5a942-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a942-155">Response</span></span>
<span data-ttu-id="5a942-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a942-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a942-157">Пример</span><span class="sxs-lookup"><span data-stu-id="5a942-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a942-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a942-158">Request</span></span>
<span data-ttu-id="5a942-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a942-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
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

### <a name="response"></a><span data-ttu-id="5a942-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a942-160">Response</span></span>
<span data-ttu-id="5a942-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5a942-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



