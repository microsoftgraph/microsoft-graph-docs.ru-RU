---
title: Обновление embeddedSIMDeviceState
description: Обновление свойства объекта embeddedSIMDeviceState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f29da78f3a0a614ce5e2bdb79ab7e88e5018a403
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408707"
---
# <a name="update-embeddedsimdevicestate"></a><span data-ttu-id="1b09d-103">Обновление embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="1b09d-103">Update embeddedSIMDeviceState</span></span>

> <span data-ttu-id="1b09d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1b09d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1b09d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b09d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b09d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b09d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b09d-107">Обновление свойства объекта [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="1b09d-107">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b09d-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="1b09d-108">Prerequisites</span></span>
<span data-ttu-id="1b09d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1b09d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1b09d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b09d-111">Permission type</span></span>|<span data-ttu-id="1b09d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b09d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b09d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b09d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b09d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b09d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1b09d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b09d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b09d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b09d-116">Not supported.</span></span>|
|<span data-ttu-id="1b09d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b09d-117">Application</span></span>|<span data-ttu-id="1b09d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b09d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b09d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b09d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="1b09d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b09d-120">Request headers</span></span>
|<span data-ttu-id="1b09d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b09d-121">Header</span></span>|<span data-ttu-id="1b09d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1b09d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b09d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b09d-123">Authorization</span></span>|<span data-ttu-id="1b09d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1b09d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b09d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1b09d-125">Accept</span></span>|<span data-ttu-id="1b09d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b09d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b09d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b09d-127">Request body</span></span>
<span data-ttu-id="1b09d-128">В тексте запроса укажите представление JSON для объекта [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="1b09d-128">In the request body, supply a JSON representation for the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

<span data-ttu-id="1b09d-129">В следующей таблице показаны свойства, которые необходимы для создания [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="1b09d-129">The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>

|<span data-ttu-id="1b09d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b09d-130">Property</span></span>|<span data-ttu-id="1b09d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1b09d-131">Type</span></span>|<span data-ttu-id="1b09d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1b09d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b09d-133">id</span><span class="sxs-lookup"><span data-stu-id="1b09d-133">id</span></span>|<span data-ttu-id="1b09d-134">String</span><span class="sxs-lookup"><span data-stu-id="1b09d-134">String</span></span>|<span data-ttu-id="1b09d-135">Уникальный идентификатор для внедренных состояние устройства диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="1b09d-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="1b09d-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="1b09d-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="1b09d-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b09d-137">createdDateTime</span></span>|<span data-ttu-id="1b09d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b09d-138">DateTimeOffset</span></span>|<span data-ttu-id="1b09d-139">Время создания внедренных состояние устройства диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="1b09d-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="1b09d-140">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="1b09d-140">Generated service side.</span></span>|
|<span data-ttu-id="1b09d-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b09d-141">modifiedDateTime</span></span>|<span data-ttu-id="1b09d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b09d-142">DateTimeOffset</span></span>|<span data-ttu-id="1b09d-143">Время последнего изменения внедренного состояние устройства диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="1b09d-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="1b09d-144">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="1b09d-144">Updated service side.</span></span>|
|<span data-ttu-id="1b09d-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1b09d-145">lastSyncDateTime</span></span>|<span data-ttu-id="1b09d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b09d-146">DateTimeOffset</span></span>|<span data-ttu-id="1b09d-147">Время, внедренные устройства диспетчера установки последнего возврата.</span><span class="sxs-lookup"><span data-stu-id="1b09d-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="1b09d-148">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="1b09d-148">Updated service side.</span></span>|
|<span data-ttu-id="1b09d-149">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="1b09d-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="1b09d-150">String</span><span class="sxs-lookup"><span data-stu-id="1b09d-150">String</span></span>|<span data-ttu-id="1b09d-151">Универсальные интегральной карточки идентификатор (UICCID) Идентификация оборудования, на котором профиль — для развертывания.</span><span class="sxs-lookup"><span data-stu-id="1b09d-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="1b09d-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="1b09d-152">deviceName</span></span>|<span data-ttu-id="1b09d-153">String</span><span class="sxs-lookup"><span data-stu-id="1b09d-153">String</span></span>|<span data-ttu-id="1b09d-154">Имя устройства, к которому был подписки например рабочего СТОЛА ДЖО подготовить к работе</span><span class="sxs-lookup"><span data-stu-id="1b09d-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="1b09d-155">userName</span><span class="sxs-lookup"><span data-stu-id="1b09d-155">userName</span></span>|<span data-ttu-id="1b09d-156">String</span><span class="sxs-lookup"><span data-stu-id="1b09d-156">String</span></span>|<span data-ttu-id="1b09d-157">Имя пользователя, который был подписки подготовлен к например joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="1b09d-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="1b09d-158">state</span><span class="sxs-lookup"><span data-stu-id="1b09d-158">state</span></span>|[<span data-ttu-id="1b09d-159">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="1b09d-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="1b09d-160">Состояние операции профилей, применяемые к устройства.</span><span class="sxs-lookup"><span data-stu-id="1b09d-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="1b09d-161">Возможные значения: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="1b09d-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="1b09d-162">stateDetails</span><span class="sxs-lookup"><span data-stu-id="1b09d-162">stateDetails</span></span>|<span data-ttu-id="1b09d-163">String</span><span class="sxs-lookup"><span data-stu-id="1b09d-163">String</span></span>|<span data-ttu-id="1b09d-164">Строка Описание подготовки состояния.</span><span class="sxs-lookup"><span data-stu-id="1b09d-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="1b09d-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b09d-165">Response</span></span>
<span data-ttu-id="1b09d-166">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1b09d-166">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b09d-167">Пример</span><span class="sxs-lookup"><span data-stu-id="1b09d-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b09d-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b09d-168">Request</span></span>
<span data-ttu-id="1b09d-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b09d-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1b09d-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b09d-170">Response</span></span>
<span data-ttu-id="1b09d-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1b09d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




