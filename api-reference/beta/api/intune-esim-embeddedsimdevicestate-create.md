---
title: Создание Ембеддедсимдевицестате
description: Создание нового объекта Ембеддедсимдевицестате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ef30988902a07b730dee7687b1b9b32251b5fbcd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452125"
---
# <a name="create-embeddedsimdevicestate"></a><span data-ttu-id="80962-103">Создание Ембеддедсимдевицестате</span><span class="sxs-lookup"><span data-stu-id="80962-103">Create embeddedSIMDeviceState</span></span>

<span data-ttu-id="80962-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80962-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80962-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80962-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80962-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="80962-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80962-107">Создание нового объекта [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="80962-107">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80962-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="80962-108">Prerequisites</span></span>
<span data-ttu-id="80962-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80962-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80962-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80962-111">Permission type</span></span>|<span data-ttu-id="80962-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="80962-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80962-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80962-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80962-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80962-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80962-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80962-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80962-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80962-116">Not supported.</span></span>|
|<span data-ttu-id="80962-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80962-117">Application</span></span>|<span data-ttu-id="80962-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80962-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="80962-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80962-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="80962-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="80962-120">Request headers</span></span>
|<span data-ttu-id="80962-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="80962-121">Header</span></span>|<span data-ttu-id="80962-122">Значение</span><span class="sxs-lookup"><span data-stu-id="80962-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80962-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80962-123">Authorization</span></span>|<span data-ttu-id="80962-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80962-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80962-125">Accept</span><span class="sxs-lookup"><span data-stu-id="80962-125">Accept</span></span>|<span data-ttu-id="80962-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80962-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80962-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="80962-127">Request body</span></span>
<span data-ttu-id="80962-128">В тексте запроса добавьте представление объекта Ембеддедсимдевицестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80962-128">In the request body, supply a JSON representation for the embeddedSIMDeviceState object.</span></span>

<span data-ttu-id="80962-129">В следующей таблице приведены свойства, необходимые при создании Ембеддедсимдевицестате.</span><span class="sxs-lookup"><span data-stu-id="80962-129">The following table shows the properties that are required when you create the embeddedSIMDeviceState.</span></span>

|<span data-ttu-id="80962-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="80962-130">Property</span></span>|<span data-ttu-id="80962-131">Тип</span><span class="sxs-lookup"><span data-stu-id="80962-131">Type</span></span>|<span data-ttu-id="80962-132">Описание</span><span class="sxs-lookup"><span data-stu-id="80962-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80962-133">id</span><span class="sxs-lookup"><span data-stu-id="80962-133">id</span></span>|<span data-ttu-id="80962-134">String</span><span class="sxs-lookup"><span data-stu-id="80962-134">String</span></span>|<span data-ttu-id="80962-135">Уникальный идентификатор состояния встроенного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="80962-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="80962-136">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="80962-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="80962-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80962-137">createdDateTime</span></span>|<span data-ttu-id="80962-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80962-138">DateTimeOffset</span></span>|<span data-ttu-id="80962-139">Время создания встроенного состояния SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="80962-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="80962-140">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="80962-140">Generated service side.</span></span>|
|<span data-ttu-id="80962-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80962-141">modifiedDateTime</span></span>|<span data-ttu-id="80962-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80962-142">DateTimeOffset</span></span>|<span data-ttu-id="80962-143">Время последнего изменения состояния внедренного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="80962-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="80962-144">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="80962-144">Updated service side.</span></span>|
|<span data-ttu-id="80962-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="80962-145">lastSyncDateTime</span></span>|<span data-ttu-id="80962-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80962-146">DateTimeOffset</span></span>|<span data-ttu-id="80962-147">Время последнего возврата встроенного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="80962-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="80962-148">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="80962-148">Updated service side.</span></span>|
|<span data-ttu-id="80962-149">универсалинтегратедЦиркуиткардидентифиер</span><span class="sxs-lookup"><span data-stu-id="80962-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="80962-150">String</span><span class="sxs-lookup"><span data-stu-id="80962-150">String</span></span>|<span data-ttu-id="80962-151">Универсальный интегрированный идентификатор карты (УИКЦИД), определяющий оборудование, на котором будет развернут профиль.</span><span class="sxs-lookup"><span data-stu-id="80962-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="80962-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="80962-152">deviceName</span></span>|<span data-ttu-id="80962-153">String</span><span class="sxs-lookup"><span data-stu-id="80962-153">String</span></span>|<span data-ttu-id="80962-154">Имя устройства, на которое была подготовлена подписка, например DESKTOP — Джо</span><span class="sxs-lookup"><span data-stu-id="80962-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="80962-155">userName</span><span class="sxs-lookup"><span data-stu-id="80962-155">userName</span></span>|<span data-ttu-id="80962-156">String</span><span class="sxs-lookup"><span data-stu-id="80962-156">String</span></span>|<span data-ttu-id="80962-157">Имя пользователя, для которого была подготовлена подписка (например, joe@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="80962-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="80962-158">state</span><span class="sxs-lookup"><span data-stu-id="80962-158">state</span></span>|[<span data-ttu-id="80962-159">ембеддедсимдевицестатевалуе</span><span class="sxs-lookup"><span data-stu-id="80962-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="80962-160">Состояние операции профиля, примененной к устройству.</span><span class="sxs-lookup"><span data-stu-id="80962-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="80962-161">Возможные значения: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="80962-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="80962-162">статедетаилс</span><span class="sxs-lookup"><span data-stu-id="80962-162">stateDetails</span></span>|<span data-ttu-id="80962-163">String</span><span class="sxs-lookup"><span data-stu-id="80962-163">String</span></span>|<span data-ttu-id="80962-164">Строковое описание состояния подготовки.</span><span class="sxs-lookup"><span data-stu-id="80962-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="80962-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="80962-165">Response</span></span>
<span data-ttu-id="80962-166">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="80962-166">If successful, this method returns a `201 Created` response code and a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80962-167">Пример</span><span class="sxs-lookup"><span data-stu-id="80962-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="80962-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="80962-168">Request</span></span>
<span data-ttu-id="80962-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="80962-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="80962-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="80962-170">Response</span></span>
<span data-ttu-id="80962-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="80962-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



