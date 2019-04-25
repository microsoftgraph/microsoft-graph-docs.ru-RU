---
title: Обновление Ембеддедсимдевицестате
description: Обновление свойств объекта Ембеддедсимдевицестате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1fbf7679467e228531bb7bc57eb9e11f5a2c9eff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532389"
---
# <a name="update-embeddedsimdevicestate"></a><span data-ttu-id="e5d22-103">Обновление Ембеддедсимдевицестате</span><span class="sxs-lookup"><span data-stu-id="e5d22-103">Update embeddedSIMDeviceState</span></span>

> <span data-ttu-id="e5d22-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5d22-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5d22-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5d22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5d22-106">Обновление свойств объекта [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="e5d22-106">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5d22-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e5d22-107">Prerequisites</span></span>
<span data-ttu-id="e5d22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5d22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5d22-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5d22-110">Permission type</span></span>|<span data-ttu-id="e5d22-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5d22-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5d22-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5d22-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5d22-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5d22-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5d22-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5d22-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5d22-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5d22-115">Not supported.</span></span>|
|<span data-ttu-id="e5d22-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5d22-116">Application</span></span>|<span data-ttu-id="e5d22-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5d22-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5d22-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5d22-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="e5d22-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5d22-119">Request headers</span></span>
|<span data-ttu-id="e5d22-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5d22-120">Header</span></span>|<span data-ttu-id="e5d22-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e5d22-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5d22-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5d22-122">Authorization</span></span>|<span data-ttu-id="e5d22-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5d22-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5d22-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e5d22-124">Accept</span></span>|<span data-ttu-id="e5d22-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5d22-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5d22-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5d22-126">Request body</span></span>
<span data-ttu-id="e5d22-127">В тексте запроса добавьте представление объекта [Ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5d22-127">In the request body, supply a JSON representation for the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

<span data-ttu-id="e5d22-128">В следующей таблице приведены свойства, необходимые при создании [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="e5d22-128">The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>

|<span data-ttu-id="e5d22-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5d22-129">Property</span></span>|<span data-ttu-id="e5d22-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e5d22-130">Type</span></span>|<span data-ttu-id="e5d22-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e5d22-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5d22-132">id</span><span class="sxs-lookup"><span data-stu-id="e5d22-132">id</span></span>|<span data-ttu-id="e5d22-133">String</span><span class="sxs-lookup"><span data-stu-id="e5d22-133">String</span></span>|<span data-ttu-id="e5d22-134">Уникальный идентификатор состояния встроенного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="e5d22-134">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="e5d22-135">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="e5d22-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="e5d22-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5d22-136">createdDateTime</span></span>|<span data-ttu-id="e5d22-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5d22-137">DateTimeOffset</span></span>|<span data-ttu-id="e5d22-138">Время создания встроенного состояния SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="e5d22-138">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="e5d22-139">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="e5d22-139">Generated service side.</span></span>|
|<span data-ttu-id="e5d22-140">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5d22-140">modifiedDateTime</span></span>|<span data-ttu-id="e5d22-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5d22-141">DateTimeOffset</span></span>|<span data-ttu-id="e5d22-142">Время последнего изменения состояния внедренного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="e5d22-142">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="e5d22-143">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="e5d22-143">Updated service side.</span></span>|
|<span data-ttu-id="e5d22-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e5d22-144">lastSyncDateTime</span></span>|<span data-ttu-id="e5d22-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5d22-145">DateTimeOffset</span></span>|<span data-ttu-id="e5d22-146">Время последнего возврата встроенного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="e5d22-146">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="e5d22-147">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="e5d22-147">Updated service side.</span></span>|
|<span data-ttu-id="e5d22-148">УниверсалинтегратедЦиркуиткардидентифиер</span><span class="sxs-lookup"><span data-stu-id="e5d22-148">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="e5d22-149">String</span><span class="sxs-lookup"><span data-stu-id="e5d22-149">String</span></span>|<span data-ttu-id="e5d22-150">Универсальный интегрированный идентификатор карты (УИКЦИД), определяющий оборудование, на котором будет развернут профиль.</span><span class="sxs-lookup"><span data-stu-id="e5d22-150">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="e5d22-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="e5d22-151">deviceName</span></span>|<span data-ttu-id="e5d22-152">String</span><span class="sxs-lookup"><span data-stu-id="e5d22-152">String</span></span>|<span data-ttu-id="e5d22-153">Имя устройства, на которое была подготовлена подписка, например DESKTOP — Джо</span><span class="sxs-lookup"><span data-stu-id="e5d22-153">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="e5d22-154">userName</span><span class="sxs-lookup"><span data-stu-id="e5d22-154">userName</span></span>|<span data-ttu-id="e5d22-155">String</span><span class="sxs-lookup"><span data-stu-id="e5d22-155">String</span></span>|<span data-ttu-id="e5d22-156">Имя пользователя, для которого была подготовлена подписка (например, joe@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="e5d22-156">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="e5d22-157">state</span><span class="sxs-lookup"><span data-stu-id="e5d22-157">state</span></span>|[<span data-ttu-id="e5d22-158">Ембеддедсимдевицестатевалуе</span><span class="sxs-lookup"><span data-stu-id="e5d22-158">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="e5d22-159">Состояние операции профиля, примененной к устройству.</span><span class="sxs-lookup"><span data-stu-id="e5d22-159">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="e5d22-160">Возможные значения: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="e5d22-160">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="e5d22-161">Статедетаилс</span><span class="sxs-lookup"><span data-stu-id="e5d22-161">stateDetails</span></span>|<span data-ttu-id="e5d22-162">String</span><span class="sxs-lookup"><span data-stu-id="e5d22-162">String</span></span>|<span data-ttu-id="e5d22-163">Строковое описание состояния подготовки.</span><span class="sxs-lookup"><span data-stu-id="e5d22-163">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="e5d22-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5d22-164">Response</span></span>
<span data-ttu-id="e5d22-165">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5d22-165">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5d22-166">Пример</span><span class="sxs-lookup"><span data-stu-id="e5d22-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5d22-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5d22-167">Request</span></span>
<span data-ttu-id="e5d22-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5d22-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e5d22-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5d22-169">Response</span></span>
<span data-ttu-id="e5d22-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5d22-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





