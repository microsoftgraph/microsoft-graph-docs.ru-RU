---
title: Обновление объекта deviceConfigurationDeviceStateSummary
description: Обновление свойств объекта deviceConfigurationDeviceStateSummary.
ms.openlocfilehash: a65ce289ad7c5c95b9a5ba344493c46d3dd14822
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027098"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="eab6c-103">Обновление объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="eab6c-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="eab6c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="eab6c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eab6c-105">Обновление свойств объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="eab6c-105">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eab6c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="eab6c-106">Prerequisites</span></span>
<span data-ttu-id="eab6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eab6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eab6c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eab6c-109">Permission type</span></span>|<span data-ttu-id="eab6c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eab6c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eab6c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eab6c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eab6c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eab6c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eab6c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eab6c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eab6c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eab6c-114">Not supported.</span></span>|
|<span data-ttu-id="eab6c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eab6c-115">Application</span></span>|<span data-ttu-id="eab6c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eab6c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eab6c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eab6c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="eab6c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eab6c-118">Request headers</span></span>
|<span data-ttu-id="eab6c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eab6c-119">Header</span></span>|<span data-ttu-id="eab6c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="eab6c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eab6c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eab6c-121">Authorization</span></span>|<span data-ttu-id="eab6c-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="eab6c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eab6c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="eab6c-123">Accept</span></span>|<span data-ttu-id="eab6c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eab6c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eab6c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eab6c-125">Request body</span></span>
<span data-ttu-id="eab6c-126">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eab6c-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="eab6c-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="eab6c-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="eab6c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="eab6c-128">Property</span></span>|<span data-ttu-id="eab6c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="eab6c-129">Type</span></span>|<span data-ttu-id="eab6c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="eab6c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eab6c-131">id</span><span class="sxs-lookup"><span data-stu-id="eab6c-131">id</span></span>|<span data-ttu-id="eab6c-132">String</span><span class="sxs-lookup"><span data-stu-id="eab6c-132">String</span></span>|<span data-ttu-id="eab6c-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eab6c-133">Key of the entity.</span></span>|
|<span data-ttu-id="eab6c-134">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eab6c-134">unknownDeviceCount</span></span>|<span data-ttu-id="eab6c-135">Int32</span><span class="sxs-lookup"><span data-stu-id="eab6c-135">Int32</span></span>|<span data-ttu-id="eab6c-136">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="eab6c-136">Number of unknown devices</span></span>|
|<span data-ttu-id="eab6c-137">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eab6c-137">notApplicableDeviceCount</span></span>|<span data-ttu-id="eab6c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="eab6c-138">Int32</span></span>|<span data-ttu-id="eab6c-139">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="eab6c-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="eab6c-140">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eab6c-140">compliantDeviceCount</span></span>|<span data-ttu-id="eab6c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="eab6c-141">Int32</span></span>|<span data-ttu-id="eab6c-142">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="eab6c-142">Number of compliant devices</span></span>|
|<span data-ttu-id="eab6c-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eab6c-143">remediatedDeviceCount</span></span>|<span data-ttu-id="eab6c-144">Int32</span><span class="sxs-lookup"><span data-stu-id="eab6c-144">Int32</span></span>|<span data-ttu-id="eab6c-145">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="eab6c-145">Number of remediated devices</span></span>|
|<span data-ttu-id="eab6c-146">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eab6c-146">nonCompliantDeviceCount</span></span>|<span data-ttu-id="eab6c-147">Int32</span><span class="sxs-lookup"><span data-stu-id="eab6c-147">Int32</span></span>|<span data-ttu-id="eab6c-148">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="eab6c-148">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="eab6c-149">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eab6c-149">errorDeviceCount</span></span>|<span data-ttu-id="eab6c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="eab6c-150">Int32</span></span>|<span data-ttu-id="eab6c-151">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="eab6c-151">Number of error devices</span></span>|
|<span data-ttu-id="eab6c-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="eab6c-152">conflictDeviceCount</span></span>|<span data-ttu-id="eab6c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="eab6c-153">Int32</span></span>|<span data-ttu-id="eab6c-154">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="eab6c-154">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="eab6c-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="eab6c-155">Response</span></span>
<span data-ttu-id="eab6c-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eab6c-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eab6c-157">Пример</span><span class="sxs-lookup"><span data-stu-id="eab6c-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="eab6c-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="eab6c-158">Request</span></span>
<span data-ttu-id="eab6c-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eab6c-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eab6c-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="eab6c-160">Response</span></span>
<span data-ttu-id="eab6c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="eab6c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



