---
title: Создание Ембеддедсимдевицестате
description: Создание нового объекта Ембеддедсимдевицестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dd0b4ce57be5478938a2d88f7134194b93a4de2e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004979"
---
# <a name="create-embeddedsimdevicestate"></a><span data-ttu-id="8bfd0-103">Создание Ембеддедсимдевицестате</span><span class="sxs-lookup"><span data-stu-id="8bfd0-103">Create embeddedSIMDeviceState</span></span>

<span data-ttu-id="8bfd0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bfd0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8bfd0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bfd0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bfd0-107">Создание нового объекта [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="8bfd0-107">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bfd0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8bfd0-108">Prerequisites</span></span>
<span data-ttu-id="8bfd0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bfd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bfd0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bfd0-111">Permission type</span></span>|<span data-ttu-id="8bfd0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bfd0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bfd0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bfd0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8bfd0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bfd0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8bfd0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bfd0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bfd0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-116">Not supported.</span></span>|
|<span data-ttu-id="8bfd0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8bfd0-117">Application</span></span>|<span data-ttu-id="8bfd0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bfd0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bfd0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bfd0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="8bfd0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8bfd0-120">Request headers</span></span>
|<span data-ttu-id="8bfd0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8bfd0-121">Header</span></span>|<span data-ttu-id="8bfd0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8bfd0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bfd0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bfd0-123">Authorization</span></span>|<span data-ttu-id="8bfd0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bfd0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8bfd0-125">Accept</span></span>|<span data-ttu-id="8bfd0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8bfd0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bfd0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8bfd0-127">Request body</span></span>
<span data-ttu-id="8bfd0-128">В тексте запроса добавьте представление объекта Ембеддедсимдевицестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-128">In the request body, supply a JSON representation for the embeddedSIMDeviceState object.</span></span>

<span data-ttu-id="8bfd0-129">В следующей таблице приведены свойства, необходимые при создании Ембеддедсимдевицестате.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-129">The following table shows the properties that are required when you create the embeddedSIMDeviceState.</span></span>

|<span data-ttu-id="8bfd0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bfd0-130">Property</span></span>|<span data-ttu-id="8bfd0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8bfd0-131">Type</span></span>|<span data-ttu-id="8bfd0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8bfd0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bfd0-133">id</span><span class="sxs-lookup"><span data-stu-id="8bfd0-133">id</span></span>|<span data-ttu-id="8bfd0-134">String</span><span class="sxs-lookup"><span data-stu-id="8bfd0-134">String</span></span>|<span data-ttu-id="8bfd0-135">Уникальный идентификатор состояния встроенного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="8bfd0-136">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="8bfd0-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8bfd0-137">createdDateTime</span></span>|<span data-ttu-id="8bfd0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bfd0-138">DateTimeOffset</span></span>|<span data-ttu-id="8bfd0-139">Время создания встроенного состояния SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="8bfd0-140">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-140">Generated service side.</span></span>|
|<span data-ttu-id="8bfd0-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bfd0-141">modifiedDateTime</span></span>|<span data-ttu-id="8bfd0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bfd0-142">DateTimeOffset</span></span>|<span data-ttu-id="8bfd0-143">Время последнего изменения состояния внедренного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="8bfd0-144">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-144">Updated service side.</span></span>|
|<span data-ttu-id="8bfd0-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8bfd0-145">lastSyncDateTime</span></span>|<span data-ttu-id="8bfd0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bfd0-146">DateTimeOffset</span></span>|<span data-ttu-id="8bfd0-147">Время последнего возврата встроенного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="8bfd0-148">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-148">Updated service side.</span></span>|
|<span data-ttu-id="8bfd0-149">универсалинтегратедЦиркуиткардидентифиер</span><span class="sxs-lookup"><span data-stu-id="8bfd0-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="8bfd0-150">String</span><span class="sxs-lookup"><span data-stu-id="8bfd0-150">String</span></span>|<span data-ttu-id="8bfd0-151">Универсальный интегрированный идентификатор карты (УИКЦИД), определяющий оборудование, на котором будет развернут профиль.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="8bfd0-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="8bfd0-152">deviceName</span></span>|<span data-ttu-id="8bfd0-153">String</span><span class="sxs-lookup"><span data-stu-id="8bfd0-153">String</span></span>|<span data-ttu-id="8bfd0-154">Имя устройства, на которое была подготовлена подписка, например DESKTOP — Джо</span><span class="sxs-lookup"><span data-stu-id="8bfd0-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="8bfd0-155">userName</span><span class="sxs-lookup"><span data-stu-id="8bfd0-155">userName</span></span>|<span data-ttu-id="8bfd0-156">String</span><span class="sxs-lookup"><span data-stu-id="8bfd0-156">String</span></span>|<span data-ttu-id="8bfd0-157">Имя пользователя, для которого была подготовлена подписка (например, joe@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="8bfd0-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="8bfd0-158">state</span><span class="sxs-lookup"><span data-stu-id="8bfd0-158">state</span></span>|[<span data-ttu-id="8bfd0-159">ембеддедсимдевицестатевалуе</span><span class="sxs-lookup"><span data-stu-id="8bfd0-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="8bfd0-160">Состояние операции профиля, примененной к устройству.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="8bfd0-161">Возможные значения: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="8bfd0-162">статедетаилс</span><span class="sxs-lookup"><span data-stu-id="8bfd0-162">stateDetails</span></span>|<span data-ttu-id="8bfd0-163">String</span><span class="sxs-lookup"><span data-stu-id="8bfd0-163">String</span></span>|<span data-ttu-id="8bfd0-164">Строковое описание состояния подготовки.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="8bfd0-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bfd0-165">Response</span></span>
<span data-ttu-id="8bfd0-166">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-166">If successful, this method returns a `201 Created` response code and a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bfd0-167">Пример</span><span class="sxs-lookup"><span data-stu-id="8bfd0-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bfd0-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bfd0-168">Request</span></span>
<span data-ttu-id="8bfd0-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8bfd0-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bfd0-170">Response</span></span>
<span data-ttu-id="8bfd0-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8bfd0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






