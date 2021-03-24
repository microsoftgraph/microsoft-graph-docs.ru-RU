---
title: Создание встроенных элементовSIMDeviceState
description: Создайте новый встроенный объектSIMDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b0627c0c011c193168b53c0efbe0274d7b0d2e91
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126075"
---
# <a name="create-embeddedsimdevicestate"></a><span data-ttu-id="c40dc-103">Создание встроенных элементовSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="c40dc-103">Create embeddedSIMDeviceState</span></span>

<span data-ttu-id="c40dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c40dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c40dc-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c40dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c40dc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c40dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c40dc-107">Создайте новый [встроенный объектSIMDeviceState.](../resources/intune-esim-embeddedsimdevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="c40dc-107">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c40dc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c40dc-108">Prerequisites</span></span>
<span data-ttu-id="c40dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c40dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c40dc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c40dc-111">Permission type</span></span>|<span data-ttu-id="c40dc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c40dc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c40dc-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c40dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c40dc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c40dc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c40dc-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c40dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c40dc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c40dc-116">Not supported.</span></span>|
|<span data-ttu-id="c40dc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c40dc-117">Application</span></span>|<span data-ttu-id="c40dc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c40dc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c40dc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c40dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="c40dc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c40dc-120">Request headers</span></span>
|<span data-ttu-id="c40dc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c40dc-121">Header</span></span>|<span data-ttu-id="c40dc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c40dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c40dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c40dc-123">Authorization</span></span>|<span data-ttu-id="c40dc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c40dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c40dc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c40dc-125">Accept</span></span>|<span data-ttu-id="c40dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c40dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c40dc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c40dc-127">Request body</span></span>
<span data-ttu-id="c40dc-128">В корпусе запроса поставляем представление JSON для встроенного объектаSIMDeviceState.</span><span class="sxs-lookup"><span data-stu-id="c40dc-128">In the request body, supply a JSON representation for the embeddedSIMDeviceState object.</span></span>

<span data-ttu-id="c40dc-129">В следующей таблице показаны свойства, необходимые при создании встроенной таблицыSIMDeviceState.</span><span class="sxs-lookup"><span data-stu-id="c40dc-129">The following table shows the properties that are required when you create the embeddedSIMDeviceState.</span></span>

|<span data-ttu-id="c40dc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c40dc-130">Property</span></span>|<span data-ttu-id="c40dc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c40dc-131">Type</span></span>|<span data-ttu-id="c40dc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c40dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c40dc-133">id</span><span class="sxs-lookup"><span data-stu-id="c40dc-133">id</span></span>|<span data-ttu-id="c40dc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c40dc-134">String</span></span>|<span data-ttu-id="c40dc-135">Уникальный идентификатор для состояния встроенного sim-устройства.</span><span class="sxs-lookup"><span data-stu-id="c40dc-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="c40dc-136">Созданное в системе значение, назначенное при его создания.</span><span class="sxs-lookup"><span data-stu-id="c40dc-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="c40dc-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c40dc-137">createdDateTime</span></span>|<span data-ttu-id="c40dc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c40dc-138">DateTimeOffset</span></span>|<span data-ttu-id="c40dc-139">Время создания состояния встроенного sim-устройства.</span><span class="sxs-lookup"><span data-stu-id="c40dc-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="c40dc-140">Сгенерированная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="c40dc-140">Generated service side.</span></span>|
|<span data-ttu-id="c40dc-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c40dc-141">modifiedDateTime</span></span>|<span data-ttu-id="c40dc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c40dc-142">DateTimeOffset</span></span>|<span data-ttu-id="c40dc-143">Время последнего изменения состояния встроенного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="c40dc-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="c40dc-144">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="c40dc-144">Updated service side.</span></span>|
|<span data-ttu-id="c40dc-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c40dc-145">lastSyncDateTime</span></span>|<span data-ttu-id="c40dc-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c40dc-146">DateTimeOffset</span></span>|<span data-ttu-id="c40dc-147">Время последней регистрации встроенного sim-устройства.</span><span class="sxs-lookup"><span data-stu-id="c40dc-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="c40dc-148">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="c40dc-148">Updated service side.</span></span>|
|<span data-ttu-id="c40dc-149">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="c40dc-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="c40dc-150">Строка</span><span class="sxs-lookup"><span data-stu-id="c40dc-150">String</span></span>|<span data-ttu-id="c40dc-151">Идентификатор универсальной интегрированной схемной карты (UICCID), определяющий оборудование, на которое будет развернут профиль.</span><span class="sxs-lookup"><span data-stu-id="c40dc-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="c40dc-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="c40dc-152">deviceName</span></span>|<span data-ttu-id="c40dc-153">String</span><span class="sxs-lookup"><span data-stu-id="c40dc-153">String</span></span>|<span data-ttu-id="c40dc-154">Имя устройства, на которое была предусмотрена подписка, например DESKTOP-JOE</span><span class="sxs-lookup"><span data-stu-id="c40dc-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="c40dc-155">userName</span><span class="sxs-lookup"><span data-stu-id="c40dc-155">userName</span></span>|<span data-ttu-id="c40dc-156">String</span><span class="sxs-lookup"><span data-stu-id="c40dc-156">String</span></span>|<span data-ttu-id="c40dc-157">Имя пользователя, для которого была предусмотрена подписка, например joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="c40dc-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="c40dc-158">state</span><span class="sxs-lookup"><span data-stu-id="c40dc-158">state</span></span>|[<span data-ttu-id="c40dc-159">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="c40dc-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="c40dc-160">Состояние операции профиля, примененной к устройству.</span><span class="sxs-lookup"><span data-stu-id="c40dc-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="c40dc-161">Возможные значения: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="c40dc-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="c40dc-162">stateDetails</span><span class="sxs-lookup"><span data-stu-id="c40dc-162">stateDetails</span></span>|<span data-ttu-id="c40dc-163">Строка</span><span class="sxs-lookup"><span data-stu-id="c40dc-163">String</span></span>|<span data-ttu-id="c40dc-164">Строковое описание состояния подготовка.</span><span class="sxs-lookup"><span data-stu-id="c40dc-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="c40dc-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="c40dc-165">Response</span></span>
<span data-ttu-id="c40dc-166">В случае успешной работы этот метод возвращает код ответа и встроенный `201 Created` [объектSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c40dc-166">If successful, this method returns a `201 Created` response code and a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c40dc-167">Пример</span><span class="sxs-lookup"><span data-stu-id="c40dc-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="c40dc-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="c40dc-168">Request</span></span>
<span data-ttu-id="c40dc-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c40dc-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
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

### <a name="response"></a><span data-ttu-id="c40dc-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="c40dc-170">Response</span></span>
<span data-ttu-id="c40dc-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c40dc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




