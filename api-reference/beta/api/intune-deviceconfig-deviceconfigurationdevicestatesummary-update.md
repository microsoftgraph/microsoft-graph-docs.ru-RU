---
title: Обновление объекта deviceConfigurationDeviceStateSummary
description: Обновление свойств объекта deviceConfigurationDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1963e00e5f2cf6719932b1b26b388a72fff0fb28
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832533"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="67b17-103">Обновление объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="67b17-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="67b17-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="67b17-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67b17-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67b17-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67b17-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="67b17-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67b17-107">Обновление свойств объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="67b17-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="67b17-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="67b17-108">Prerequisites</span></span>
<span data-ttu-id="67b17-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67b17-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67b17-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67b17-111">Permission type</span></span>|<span data-ttu-id="67b17-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="67b17-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67b17-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67b17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67b17-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67b17-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="67b17-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67b17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67b17-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67b17-116">Not supported.</span></span>|
|<span data-ttu-id="67b17-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67b17-117">Application</span></span>|<span data-ttu-id="67b17-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67b17-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67b17-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67b17-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="67b17-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67b17-120">Request headers</span></span>
|<span data-ttu-id="67b17-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="67b17-121">Header</span></span>|<span data-ttu-id="67b17-122">Значение</span><span class="sxs-lookup"><span data-stu-id="67b17-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67b17-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="67b17-123">Authorization</span></span>|<span data-ttu-id="67b17-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="67b17-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67b17-125">Accept</span><span class="sxs-lookup"><span data-stu-id="67b17-125">Accept</span></span>|<span data-ttu-id="67b17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67b17-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67b17-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67b17-127">Request body</span></span>
<span data-ttu-id="67b17-128">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67b17-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="67b17-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="67b17-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="67b17-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="67b17-130">Property</span></span>|<span data-ttu-id="67b17-131">Тип</span><span class="sxs-lookup"><span data-stu-id="67b17-131">Type</span></span>|<span data-ttu-id="67b17-132">Описание</span><span class="sxs-lookup"><span data-stu-id="67b17-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67b17-133">id</span><span class="sxs-lookup"><span data-stu-id="67b17-133">id</span></span>|<span data-ttu-id="67b17-134">Строка</span><span class="sxs-lookup"><span data-stu-id="67b17-134">String</span></span>|<span data-ttu-id="67b17-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="67b17-135">Key of the entity.</span></span>|
|<span data-ttu-id="67b17-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="67b17-136">unknownDeviceCount</span></span>|<span data-ttu-id="67b17-137">Int32</span><span class="sxs-lookup"><span data-stu-id="67b17-137">Int32</span></span>|<span data-ttu-id="67b17-138">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="67b17-138">Number of unknown devices</span></span>|
|<span data-ttu-id="67b17-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="67b17-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="67b17-140">Int32</span><span class="sxs-lookup"><span data-stu-id="67b17-140">Int32</span></span>|<span data-ttu-id="67b17-141">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="67b17-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="67b17-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="67b17-142">compliantDeviceCount</span></span>|<span data-ttu-id="67b17-143">Int32</span><span class="sxs-lookup"><span data-stu-id="67b17-143">Int32</span></span>|<span data-ttu-id="67b17-144">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="67b17-144">Number of compliant devices</span></span>|
|<span data-ttu-id="67b17-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="67b17-145">remediatedDeviceCount</span></span>|<span data-ttu-id="67b17-146">Int32</span><span class="sxs-lookup"><span data-stu-id="67b17-146">Int32</span></span>|<span data-ttu-id="67b17-147">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="67b17-147">Number of remediated devices</span></span>|
|<span data-ttu-id="67b17-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="67b17-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="67b17-149">Int32</span><span class="sxs-lookup"><span data-stu-id="67b17-149">Int32</span></span>|<span data-ttu-id="67b17-150">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="67b17-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="67b17-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="67b17-151">errorDeviceCount</span></span>|<span data-ttu-id="67b17-152">Int32</span><span class="sxs-lookup"><span data-stu-id="67b17-152">Int32</span></span>|<span data-ttu-id="67b17-153">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="67b17-153">Number of error devices</span></span>|
|<span data-ttu-id="67b17-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="67b17-154">conflictDeviceCount</span></span>|<span data-ttu-id="67b17-155">Int32</span><span class="sxs-lookup"><span data-stu-id="67b17-155">Int32</span></span>|<span data-ttu-id="67b17-156">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="67b17-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="67b17-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="67b17-157">Response</span></span>
<span data-ttu-id="67b17-158">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="67b17-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67b17-159">Пример</span><span class="sxs-lookup"><span data-stu-id="67b17-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="67b17-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="67b17-160">Request</span></span>
<span data-ttu-id="67b17-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67b17-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 214

{
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="67b17-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="67b17-162">Response</span></span>
<span data-ttu-id="67b17-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="67b17-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





