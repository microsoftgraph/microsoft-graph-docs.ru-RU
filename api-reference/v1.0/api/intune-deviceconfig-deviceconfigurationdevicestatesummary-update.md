---
title: Обновление объекта deviceConfigurationDeviceStateSummary
description: Обновление свойств объекта deviceConfigurationDeviceStateSummary.
author: tfitzmac
ms.openlocfilehash: 9dd5e96762a750b015d6eb8dea7d1778ac36f66b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354259"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="17ede-103">Обновление объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="17ede-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="17ede-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="17ede-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17ede-105">Обновление свойств объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="17ede-105">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="17ede-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="17ede-106">Prerequisites</span></span>
<span data-ttu-id="17ede-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17ede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17ede-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17ede-109">Permission type</span></span>|<span data-ttu-id="17ede-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="17ede-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17ede-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17ede-111">Delegated (work or school account)</span></span>|<span data-ttu-id="17ede-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17ede-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17ede-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17ede-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17ede-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17ede-114">Not supported.</span></span>|
|<span data-ttu-id="17ede-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17ede-115">Application</span></span>|<span data-ttu-id="17ede-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17ede-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17ede-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17ede-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="17ede-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17ede-118">Request headers</span></span>
|<span data-ttu-id="17ede-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17ede-119">Header</span></span>|<span data-ttu-id="17ede-120">Значение</span><span class="sxs-lookup"><span data-stu-id="17ede-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17ede-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17ede-121">Authorization</span></span>|<span data-ttu-id="17ede-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="17ede-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17ede-123">Accept</span><span class="sxs-lookup"><span data-stu-id="17ede-123">Accept</span></span>|<span data-ttu-id="17ede-124">application/json</span><span class="sxs-lookup"><span data-stu-id="17ede-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17ede-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17ede-125">Request body</span></span>
<span data-ttu-id="17ede-126">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17ede-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="17ede-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="17ede-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="17ede-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="17ede-128">Property</span></span>|<span data-ttu-id="17ede-129">Тип</span><span class="sxs-lookup"><span data-stu-id="17ede-129">Type</span></span>|<span data-ttu-id="17ede-130">Описание</span><span class="sxs-lookup"><span data-stu-id="17ede-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17ede-131">id</span><span class="sxs-lookup"><span data-stu-id="17ede-131">id</span></span>|<span data-ttu-id="17ede-132">Строка</span><span class="sxs-lookup"><span data-stu-id="17ede-132">String</span></span>|<span data-ttu-id="17ede-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="17ede-133">Key of the entity.</span></span>|
|<span data-ttu-id="17ede-134">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17ede-134">unknownDeviceCount</span></span>|<span data-ttu-id="17ede-135">Int32</span><span class="sxs-lookup"><span data-stu-id="17ede-135">Int32</span></span>|<span data-ttu-id="17ede-136">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="17ede-136">Number of unknown devices</span></span>|
|<span data-ttu-id="17ede-137">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17ede-137">notApplicableDeviceCount</span></span>|<span data-ttu-id="17ede-138">Int32</span><span class="sxs-lookup"><span data-stu-id="17ede-138">Int32</span></span>|<span data-ttu-id="17ede-139">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="17ede-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="17ede-140">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17ede-140">compliantDeviceCount</span></span>|<span data-ttu-id="17ede-141">Int32</span><span class="sxs-lookup"><span data-stu-id="17ede-141">Int32</span></span>|<span data-ttu-id="17ede-142">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="17ede-142">Number of compliant devices</span></span>|
|<span data-ttu-id="17ede-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17ede-143">remediatedDeviceCount</span></span>|<span data-ttu-id="17ede-144">Int32</span><span class="sxs-lookup"><span data-stu-id="17ede-144">Int32</span></span>|<span data-ttu-id="17ede-145">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="17ede-145">Number of remediated devices</span></span>|
|<span data-ttu-id="17ede-146">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17ede-146">nonCompliantDeviceCount</span></span>|<span data-ttu-id="17ede-147">Int32</span><span class="sxs-lookup"><span data-stu-id="17ede-147">Int32</span></span>|<span data-ttu-id="17ede-148">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="17ede-148">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="17ede-149">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17ede-149">errorDeviceCount</span></span>|<span data-ttu-id="17ede-150">Int32</span><span class="sxs-lookup"><span data-stu-id="17ede-150">Int32</span></span>|<span data-ttu-id="17ede-151">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="17ede-151">Number of error devices</span></span>|
|<span data-ttu-id="17ede-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17ede-152">conflictDeviceCount</span></span>|<span data-ttu-id="17ede-153">Int32</span><span class="sxs-lookup"><span data-stu-id="17ede-153">Int32</span></span>|<span data-ttu-id="17ede-154">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="17ede-154">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="17ede-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="17ede-155">Response</span></span>
<span data-ttu-id="17ede-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="17ede-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17ede-157">Пример</span><span class="sxs-lookup"><span data-stu-id="17ede-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="17ede-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="17ede-158">Request</span></span>
<span data-ttu-id="17ede-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17ede-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="17ede-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="17ede-160">Response</span></span>
<span data-ttu-id="17ede-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="17ede-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



