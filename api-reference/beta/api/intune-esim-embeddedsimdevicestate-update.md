---
title: Обновление Ембеддедсимдевицестате
description: Обновление свойств объекта Ембеддедсимдевицестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 23722d12e64d1d6fdcd4bb2ed2942420ae677e69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465914"
---
# <a name="update-embeddedsimdevicestate"></a><span data-ttu-id="91e16-103">Обновление Ембеддедсимдевицестате</span><span class="sxs-lookup"><span data-stu-id="91e16-103">Update embeddedSIMDeviceState</span></span>

<span data-ttu-id="91e16-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="91e16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91e16-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91e16-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91e16-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91e16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91e16-107">Обновление свойств объекта [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="91e16-107">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91e16-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="91e16-108">Prerequisites</span></span>
<span data-ttu-id="91e16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91e16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91e16-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91e16-111">Permission type</span></span>|<span data-ttu-id="91e16-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="91e16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91e16-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91e16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="91e16-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91e16-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="91e16-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91e16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91e16-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91e16-116">Not supported.</span></span>|
|<span data-ttu-id="91e16-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91e16-117">Application</span></span>|<span data-ttu-id="91e16-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91e16-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91e16-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91e16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="91e16-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="91e16-120">Request headers</span></span>
|<span data-ttu-id="91e16-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91e16-121">Header</span></span>|<span data-ttu-id="91e16-122">Значение</span><span class="sxs-lookup"><span data-stu-id="91e16-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91e16-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="91e16-123">Authorization</span></span>|<span data-ttu-id="91e16-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91e16-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91e16-125">Accept</span><span class="sxs-lookup"><span data-stu-id="91e16-125">Accept</span></span>|<span data-ttu-id="91e16-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91e16-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91e16-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91e16-127">Request body</span></span>
<span data-ttu-id="91e16-128">В тексте запроса добавьте представление объекта [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91e16-128">In the request body, supply a JSON representation for the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

<span data-ttu-id="91e16-129">В следующей таблице приведены свойства, необходимые при создании [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="91e16-129">The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>

|<span data-ttu-id="91e16-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="91e16-130">Property</span></span>|<span data-ttu-id="91e16-131">Тип</span><span class="sxs-lookup"><span data-stu-id="91e16-131">Type</span></span>|<span data-ttu-id="91e16-132">Описание</span><span class="sxs-lookup"><span data-stu-id="91e16-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91e16-133">id</span><span class="sxs-lookup"><span data-stu-id="91e16-133">id</span></span>|<span data-ttu-id="91e16-134">String</span><span class="sxs-lookup"><span data-stu-id="91e16-134">String</span></span>|<span data-ttu-id="91e16-135">Уникальный идентификатор состояния встроенного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="91e16-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="91e16-136">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="91e16-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="91e16-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91e16-137">createdDateTime</span></span>|<span data-ttu-id="91e16-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91e16-138">DateTimeOffset</span></span>|<span data-ttu-id="91e16-139">Время создания встроенного состояния SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="91e16-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="91e16-140">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="91e16-140">Generated service side.</span></span>|
|<span data-ttu-id="91e16-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91e16-141">modifiedDateTime</span></span>|<span data-ttu-id="91e16-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91e16-142">DateTimeOffset</span></span>|<span data-ttu-id="91e16-143">Время последнего изменения состояния внедренного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="91e16-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="91e16-144">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="91e16-144">Updated service side.</span></span>|
|<span data-ttu-id="91e16-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="91e16-145">lastSyncDateTime</span></span>|<span data-ttu-id="91e16-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91e16-146">DateTimeOffset</span></span>|<span data-ttu-id="91e16-147">Время последнего возврата встроенного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="91e16-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="91e16-148">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="91e16-148">Updated service side.</span></span>|
|<span data-ttu-id="91e16-149">универсалинтегратедЦиркуиткардидентифиер</span><span class="sxs-lookup"><span data-stu-id="91e16-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="91e16-150">String</span><span class="sxs-lookup"><span data-stu-id="91e16-150">String</span></span>|<span data-ttu-id="91e16-151">Универсальный интегрированный идентификатор карты (УИКЦИД), определяющий оборудование, на котором будет развернут профиль.</span><span class="sxs-lookup"><span data-stu-id="91e16-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="91e16-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="91e16-152">deviceName</span></span>|<span data-ttu-id="91e16-153">String</span><span class="sxs-lookup"><span data-stu-id="91e16-153">String</span></span>|<span data-ttu-id="91e16-154">Имя устройства, на которое была подготовлена подписка, например DESKTOP — Джо</span><span class="sxs-lookup"><span data-stu-id="91e16-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="91e16-155">userName</span><span class="sxs-lookup"><span data-stu-id="91e16-155">userName</span></span>|<span data-ttu-id="91e16-156">String</span><span class="sxs-lookup"><span data-stu-id="91e16-156">String</span></span>|<span data-ttu-id="91e16-157">Имя пользователя, для которого была подготовлена подписка (например, joe@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="91e16-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="91e16-158">state</span><span class="sxs-lookup"><span data-stu-id="91e16-158">state</span></span>|[<span data-ttu-id="91e16-159">ембеддедсимдевицестатевалуе</span><span class="sxs-lookup"><span data-stu-id="91e16-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="91e16-160">Состояние операции профиля, примененной к устройству.</span><span class="sxs-lookup"><span data-stu-id="91e16-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="91e16-161">Возможные значения: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="91e16-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="91e16-162">статедетаилс</span><span class="sxs-lookup"><span data-stu-id="91e16-162">stateDetails</span></span>|<span data-ttu-id="91e16-163">String</span><span class="sxs-lookup"><span data-stu-id="91e16-163">String</span></span>|<span data-ttu-id="91e16-164">Строковое описание состояния подготовки.</span><span class="sxs-lookup"><span data-stu-id="91e16-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="91e16-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="91e16-165">Response</span></span>
<span data-ttu-id="91e16-166">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="91e16-166">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91e16-167">Пример</span><span class="sxs-lookup"><span data-stu-id="91e16-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="91e16-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="91e16-168">Request</span></span>
<span data-ttu-id="91e16-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91e16-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```

### <a name="response"></a><span data-ttu-id="91e16-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="91e16-170">Response</span></span>
<span data-ttu-id="91e16-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91e16-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "908884a3-84a3-9088-a384-8890a3848890",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```





