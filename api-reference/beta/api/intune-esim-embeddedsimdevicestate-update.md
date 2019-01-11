---
title: Обновление embeddedSIMDeviceState
description: Обновление свойства объекта embeddedSIMDeviceState.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cad82e5e211120d79e011647063762ae6a69ec60
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858655"
---
# <a name="update-embeddedsimdevicestate"></a><span data-ttu-id="0a3ac-103">Обновление embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="0a3ac-103">Update embeddedSIMDeviceState</span></span>

> <span data-ttu-id="0a3ac-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a3ac-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a3ac-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a3ac-107">Обновление свойства объекта [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="0a3ac-107">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0a3ac-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0a3ac-108">Prerequisites</span></span>
<span data-ttu-id="0a3ac-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a3ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a3ac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a3ac-111">Permission type</span></span>|<span data-ttu-id="0a3ac-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a3ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a3ac-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a3ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a3ac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a3ac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0a3ac-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a3ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a3ac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-116">Not supported.</span></span>|
|<span data-ttu-id="0a3ac-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0a3ac-117">Application</span></span>|<span data-ttu-id="0a3ac-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a3ac-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a3ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="0a3ac-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a3ac-120">Request headers</span></span>
|<span data-ttu-id="0a3ac-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a3ac-121">Header</span></span>|<span data-ttu-id="0a3ac-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0a3ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a3ac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a3ac-123">Authorization</span></span>|<span data-ttu-id="0a3ac-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0a3ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a3ac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0a3ac-125">Accept</span></span>|<span data-ttu-id="0a3ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a3ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a3ac-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0a3ac-127">Request body</span></span>
<span data-ttu-id="0a3ac-128">В тексте запроса укажите представление JSON для объекта [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="0a3ac-128">In the request body, supply a JSON representation for the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

<span data-ttu-id="0a3ac-129">В следующей таблице показаны свойства, которые необходимы для создания [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="0a3ac-129">The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>

|<span data-ttu-id="0a3ac-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a3ac-130">Property</span></span>|<span data-ttu-id="0a3ac-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0a3ac-131">Type</span></span>|<span data-ttu-id="0a3ac-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0a3ac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a3ac-133">id</span><span class="sxs-lookup"><span data-stu-id="0a3ac-133">id</span></span>|<span data-ttu-id="0a3ac-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0a3ac-134">String</span></span>|<span data-ttu-id="0a3ac-135">Уникальный идентификатор для внедренных состояние устройства диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="0a3ac-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="0a3ac-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a3ac-137">createdDateTime</span></span>|<span data-ttu-id="0a3ac-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a3ac-138">DateTimeOffset</span></span>|<span data-ttu-id="0a3ac-139">Время создания внедренных состояние устройства диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="0a3ac-140">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-140">Generated service side.</span></span>|
|<span data-ttu-id="0a3ac-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a3ac-141">modifiedDateTime</span></span>|<span data-ttu-id="0a3ac-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a3ac-142">DateTimeOffset</span></span>|<span data-ttu-id="0a3ac-143">Время последнего изменения внедренного состояние устройства диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="0a3ac-144">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-144">Updated service side.</span></span>|
|<span data-ttu-id="0a3ac-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0a3ac-145">lastSyncDateTime</span></span>|<span data-ttu-id="0a3ac-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a3ac-146">DateTimeOffset</span></span>|<span data-ttu-id="0a3ac-147">Время, внедренные устройства диспетчера установки последнего возврата.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="0a3ac-148">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-148">Updated service side.</span></span>|
|<span data-ttu-id="0a3ac-149">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="0a3ac-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="0a3ac-150">Строка</span><span class="sxs-lookup"><span data-stu-id="0a3ac-150">String</span></span>|<span data-ttu-id="0a3ac-151">Универсальные интегральной карточки идентификатор (UICCID) Идентификация оборудования, на котором профиль — для развертывания.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="0a3ac-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="0a3ac-152">deviceName</span></span>|<span data-ttu-id="0a3ac-153">String</span><span class="sxs-lookup"><span data-stu-id="0a3ac-153">String</span></span>|<span data-ttu-id="0a3ac-154">Имя устройства, к которому был подписки например рабочего СТОЛА ДЖО подготовить к работе</span><span class="sxs-lookup"><span data-stu-id="0a3ac-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="0a3ac-155">userName</span><span class="sxs-lookup"><span data-stu-id="0a3ac-155">userName</span></span>|<span data-ttu-id="0a3ac-156">String</span><span class="sxs-lookup"><span data-stu-id="0a3ac-156">String</span></span>|<span data-ttu-id="0a3ac-157">Имя пользователя, который был подписки подготовлен к например joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="0a3ac-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="0a3ac-158">state</span><span class="sxs-lookup"><span data-stu-id="0a3ac-158">state</span></span>|[<span data-ttu-id="0a3ac-159">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="0a3ac-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="0a3ac-160">Состояние операции профилей, применяемые к устройства.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="0a3ac-161">Возможные значения: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="0a3ac-162">stateDetails</span><span class="sxs-lookup"><span data-stu-id="0a3ac-162">stateDetails</span></span>|<span data-ttu-id="0a3ac-163">Строка</span><span class="sxs-lookup"><span data-stu-id="0a3ac-163">String</span></span>|<span data-ttu-id="0a3ac-164">Строка Описание подготовки состояния.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="0a3ac-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a3ac-165">Response</span></span>
<span data-ttu-id="0a3ac-166">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-166">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a3ac-167">Пример</span><span class="sxs-lookup"><span data-stu-id="0a3ac-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="0a3ac-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a3ac-168">Request</span></span>
<span data-ttu-id="0a3ac-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
Content-type: application/json
Content-length: 300

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```

### <a name="response"></a><span data-ttu-id="0a3ac-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a3ac-170">Response</span></span>
<span data-ttu-id="0a3ac-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0a3ac-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





