---
title: Update embeddedSIMDeviceState
description: Обновление свойств встроенного объектаSIMDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6371742d475d999c639d9970c060cc1243d695cb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157613"
---
# <a name="update-embeddedsimdevicestate"></a><span data-ttu-id="837c3-103">Update embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="837c3-103">Update embeddedSIMDeviceState</span></span>

<span data-ttu-id="837c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="837c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="837c3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="837c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="837c3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="837c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="837c3-107">Обновление свойств встроенного [объектаSIMDeviceState.](../resources/intune-esim-embeddedsimdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="837c3-107">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="837c3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="837c3-108">Prerequisites</span></span>
<span data-ttu-id="837c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="837c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="837c3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="837c3-111">Permission type</span></span>|<span data-ttu-id="837c3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="837c3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="837c3-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="837c3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="837c3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="837c3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="837c3-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="837c3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="837c3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="837c3-116">Not supported.</span></span>|
|<span data-ttu-id="837c3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="837c3-117">Application</span></span>|<span data-ttu-id="837c3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="837c3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="837c3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="837c3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="837c3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="837c3-120">Request headers</span></span>
|<span data-ttu-id="837c3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="837c3-121">Header</span></span>|<span data-ttu-id="837c3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="837c3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="837c3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="837c3-123">Authorization</span></span>|<span data-ttu-id="837c3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="837c3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="837c3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="837c3-125">Accept</span></span>|<span data-ttu-id="837c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="837c3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="837c3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="837c3-127">Request body</span></span>
<span data-ttu-id="837c3-128">В корпусе запроса поставляем представление JSON для встроенного [объектаSIMDeviceState.](../resources/intune-esim-embeddedsimdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="837c3-128">In the request body, supply a JSON representation for the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

<span data-ttu-id="837c3-129">В следующей таблице показаны свойства, необходимые при создании [встроенной таблицыSIMDeviceState.](../resources/intune-esim-embeddedsimdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="837c3-129">The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>

|<span data-ttu-id="837c3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="837c3-130">Property</span></span>|<span data-ttu-id="837c3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="837c3-131">Type</span></span>|<span data-ttu-id="837c3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="837c3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="837c3-133">id</span><span class="sxs-lookup"><span data-stu-id="837c3-133">id</span></span>|<span data-ttu-id="837c3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="837c3-134">String</span></span>|<span data-ttu-id="837c3-135">Уникальный идентификатор для состояния встроенного sim-устройства.</span><span class="sxs-lookup"><span data-stu-id="837c3-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="837c3-136">Созданное в системе значение, назначенное при его создания.</span><span class="sxs-lookup"><span data-stu-id="837c3-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="837c3-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="837c3-137">createdDateTime</span></span>|<span data-ttu-id="837c3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="837c3-138">DateTimeOffset</span></span>|<span data-ttu-id="837c3-139">Время создания состояния встроенного sim-устройства.</span><span class="sxs-lookup"><span data-stu-id="837c3-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="837c3-140">Сгенерированная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="837c3-140">Generated service side.</span></span>|
|<span data-ttu-id="837c3-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="837c3-141">modifiedDateTime</span></span>|<span data-ttu-id="837c3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="837c3-142">DateTimeOffset</span></span>|<span data-ttu-id="837c3-143">Время последнего изменения состояния встроенного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="837c3-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="837c3-144">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="837c3-144">Updated service side.</span></span>|
|<span data-ttu-id="837c3-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="837c3-145">lastSyncDateTime</span></span>|<span data-ttu-id="837c3-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="837c3-146">DateTimeOffset</span></span>|<span data-ttu-id="837c3-147">Время последней регистрации встроенного sim-устройства.</span><span class="sxs-lookup"><span data-stu-id="837c3-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="837c3-148">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="837c3-148">Updated service side.</span></span>|
|<span data-ttu-id="837c3-149">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="837c3-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="837c3-150">Строка</span><span class="sxs-lookup"><span data-stu-id="837c3-150">String</span></span>|<span data-ttu-id="837c3-151">Идентификатор универсальной интегрированной схемной карты (UICCID), определяющий оборудование, на которое будет развернут профиль.</span><span class="sxs-lookup"><span data-stu-id="837c3-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="837c3-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="837c3-152">deviceName</span></span>|<span data-ttu-id="837c3-153">String</span><span class="sxs-lookup"><span data-stu-id="837c3-153">String</span></span>|<span data-ttu-id="837c3-154">Имя устройства, на которое была предусмотрена подписка, например DESKTOP-JOE</span><span class="sxs-lookup"><span data-stu-id="837c3-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="837c3-155">userName</span><span class="sxs-lookup"><span data-stu-id="837c3-155">userName</span></span>|<span data-ttu-id="837c3-156">String</span><span class="sxs-lookup"><span data-stu-id="837c3-156">String</span></span>|<span data-ttu-id="837c3-157">Имя пользователя, для которого была предусмотрена подписка, например joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="837c3-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="837c3-158">state</span><span class="sxs-lookup"><span data-stu-id="837c3-158">state</span></span>|[<span data-ttu-id="837c3-159">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="837c3-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="837c3-160">Состояние операции профиля, примененной к устройству.</span><span class="sxs-lookup"><span data-stu-id="837c3-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="837c3-161">Возможные значения: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="837c3-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="837c3-162">stateDetails</span><span class="sxs-lookup"><span data-stu-id="837c3-162">stateDetails</span></span>|<span data-ttu-id="837c3-163">Строка</span><span class="sxs-lookup"><span data-stu-id="837c3-163">String</span></span>|<span data-ttu-id="837c3-164">Строковое описание состояния подготовка.</span><span class="sxs-lookup"><span data-stu-id="837c3-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="837c3-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="837c3-165">Response</span></span>
<span data-ttu-id="837c3-166">В случае успешной работы этот метод возвращает код ответа и обновленный встроенный `200 OK` [объектSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="837c3-166">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="837c3-167">Пример</span><span class="sxs-lookup"><span data-stu-id="837c3-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="837c3-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="837c3-168">Request</span></span>
<span data-ttu-id="837c3-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="837c3-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="837c3-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="837c3-170">Response</span></span>
<span data-ttu-id="837c3-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="837c3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




