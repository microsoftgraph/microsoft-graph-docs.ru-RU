---
title: Создание Ембеддедсимдевицестате
description: Создание нового объекта Ембеддедсимдевицестате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a2d7561f116287d73b2a0e4f781bf6fa49930ea
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532347"
---
# <a name="create-embeddedsimdevicestate"></a><span data-ttu-id="a9731-103">Создание Ембеддедсимдевицестате</span><span class="sxs-lookup"><span data-stu-id="a9731-103">Create embeddedSIMDeviceState</span></span>

> <span data-ttu-id="a9731-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9731-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9731-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9731-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9731-106">Создание нового объекта [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="a9731-106">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9731-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a9731-107">Prerequisites</span></span>
<span data-ttu-id="a9731-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9731-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9731-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9731-110">Permission type</span></span>|<span data-ttu-id="a9731-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9731-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9731-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9731-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a9731-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9731-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9731-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9731-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9731-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9731-115">Not supported.</span></span>|
|<span data-ttu-id="a9731-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9731-116">Application</span></span>|<span data-ttu-id="a9731-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9731-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9731-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9731-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="a9731-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9731-119">Request headers</span></span>
|<span data-ttu-id="a9731-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9731-120">Header</span></span>|<span data-ttu-id="a9731-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a9731-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9731-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9731-122">Authorization</span></span>|<span data-ttu-id="a9731-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9731-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9731-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a9731-124">Accept</span></span>|<span data-ttu-id="a9731-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a9731-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9731-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9731-126">Request body</span></span>
<span data-ttu-id="a9731-127">В тексте запроса добавьте представление объекта Ембеддедсимдевицестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9731-127">In the request body, supply a JSON representation for the embeddedSIMDeviceState object.</span></span>

<span data-ttu-id="a9731-128">В следующей таблице приведены свойства, необходимые при создании Ембеддедсимдевицестате.</span><span class="sxs-lookup"><span data-stu-id="a9731-128">The following table shows the properties that are required when you create the embeddedSIMDeviceState.</span></span>

|<span data-ttu-id="a9731-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9731-129">Property</span></span>|<span data-ttu-id="a9731-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a9731-130">Type</span></span>|<span data-ttu-id="a9731-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a9731-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9731-132">id</span><span class="sxs-lookup"><span data-stu-id="a9731-132">id</span></span>|<span data-ttu-id="a9731-133">String</span><span class="sxs-lookup"><span data-stu-id="a9731-133">String</span></span>|<span data-ttu-id="a9731-134">Уникальный идентификатор состояния встроенного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="a9731-134">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="a9731-135">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="a9731-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="a9731-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9731-136">createdDateTime</span></span>|<span data-ttu-id="a9731-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9731-137">DateTimeOffset</span></span>|<span data-ttu-id="a9731-138">Время создания встроенного состояния SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="a9731-138">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="a9731-139">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="a9731-139">Generated service side.</span></span>|
|<span data-ttu-id="a9731-140">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9731-140">modifiedDateTime</span></span>|<span data-ttu-id="a9731-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9731-141">DateTimeOffset</span></span>|<span data-ttu-id="a9731-142">Время последнего изменения состояния внедренного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="a9731-142">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="a9731-143">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="a9731-143">Updated service side.</span></span>|
|<span data-ttu-id="a9731-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a9731-144">lastSyncDateTime</span></span>|<span data-ttu-id="a9731-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9731-145">DateTimeOffset</span></span>|<span data-ttu-id="a9731-146">Время последнего возврата встроенного SIM-устройства.</span><span class="sxs-lookup"><span data-stu-id="a9731-146">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="a9731-147">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="a9731-147">Updated service side.</span></span>|
|<span data-ttu-id="a9731-148">УниверсалинтегратедЦиркуиткардидентифиер</span><span class="sxs-lookup"><span data-stu-id="a9731-148">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="a9731-149">String</span><span class="sxs-lookup"><span data-stu-id="a9731-149">String</span></span>|<span data-ttu-id="a9731-150">Универсальный интегрированный идентификатор карты (УИКЦИД), определяющий оборудование, на котором будет развернут профиль.</span><span class="sxs-lookup"><span data-stu-id="a9731-150">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="a9731-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="a9731-151">deviceName</span></span>|<span data-ttu-id="a9731-152">String</span><span class="sxs-lookup"><span data-stu-id="a9731-152">String</span></span>|<span data-ttu-id="a9731-153">Имя устройства, на которое была подготовлена подписка, например DESKTOP — Джо</span><span class="sxs-lookup"><span data-stu-id="a9731-153">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="a9731-154">userName</span><span class="sxs-lookup"><span data-stu-id="a9731-154">userName</span></span>|<span data-ttu-id="a9731-155">String</span><span class="sxs-lookup"><span data-stu-id="a9731-155">String</span></span>|<span data-ttu-id="a9731-156">Имя пользователя, для которого была подготовлена подписка (например, joe@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="a9731-156">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="a9731-157">state</span><span class="sxs-lookup"><span data-stu-id="a9731-157">state</span></span>|[<span data-ttu-id="a9731-158">Ембеддедсимдевицестатевалуе</span><span class="sxs-lookup"><span data-stu-id="a9731-158">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="a9731-159">Состояние операции профиля, примененной к устройству.</span><span class="sxs-lookup"><span data-stu-id="a9731-159">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="a9731-160">Возможные значения: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="a9731-160">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="a9731-161">Статедетаилс</span><span class="sxs-lookup"><span data-stu-id="a9731-161">stateDetails</span></span>|<span data-ttu-id="a9731-162">String</span><span class="sxs-lookup"><span data-stu-id="a9731-162">String</span></span>|<span data-ttu-id="a9731-163">Строковое описание состояния подготовки.</span><span class="sxs-lookup"><span data-stu-id="a9731-163">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="a9731-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9731-164">Response</span></span>
<span data-ttu-id="a9731-165">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a9731-165">If successful, this method returns a `201 Created` response code and a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9731-166">Пример</span><span class="sxs-lookup"><span data-stu-id="a9731-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9731-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9731-167">Request</span></span>
<span data-ttu-id="a9731-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9731-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a9731-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9731-169">Response</span></span>
<span data-ttu-id="a9731-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9731-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





