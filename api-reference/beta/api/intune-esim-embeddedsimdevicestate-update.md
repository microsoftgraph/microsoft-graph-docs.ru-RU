---
title: Обновление embeddedSIMDeviceState
description: Обновление свойства объекта embeddedSIMDeviceState.
ms.openlocfilehash: 5a102bd686a65cf14bb078e1ae66df31bbe4dae5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076500"
---
# <a name="update-embeddedsimdevicestate"></a><span data-ttu-id="c9730-103">Обновление embeddedSIMDeviceState</span><span class="sxs-lookup"><span data-stu-id="c9730-103">Update embeddedSIMDeviceState</span></span>

> <span data-ttu-id="c9730-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c9730-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9730-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9730-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9730-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c9730-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9730-107">Обновление свойства объекта [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="c9730-107">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9730-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c9730-108">Prerequisites</span></span>
<span data-ttu-id="c9730-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9730-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9730-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9730-111">Permission type</span></span>|<span data-ttu-id="c9730-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9730-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9730-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9730-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9730-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9730-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9730-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9730-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9730-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9730-116">Not supported.</span></span>|
|<span data-ttu-id="c9730-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9730-117">Application</span></span>|<span data-ttu-id="c9730-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9730-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9730-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9730-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c9730-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9730-120">Request headers</span></span>
|<span data-ttu-id="c9730-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9730-121">Header</span></span>|<span data-ttu-id="c9730-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c9730-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9730-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9730-123">Authorization</span></span>|<span data-ttu-id="c9730-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c9730-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9730-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c9730-125">Accept</span></span>|<span data-ttu-id="c9730-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9730-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9730-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9730-127">Request body</span></span>
<span data-ttu-id="c9730-128">В тексте запроса укажите представление JSON для объекта [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="c9730-128">In the request body, supply a JSON representation for the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

<span data-ttu-id="c9730-129">В следующей таблице показаны свойства, которые необходимы для создания [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="c9730-129">The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>

|<span data-ttu-id="c9730-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9730-130">Property</span></span>|<span data-ttu-id="c9730-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c9730-131">Type</span></span>|<span data-ttu-id="c9730-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c9730-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9730-133">id</span><span class="sxs-lookup"><span data-stu-id="c9730-133">id</span></span>|<span data-ttu-id="c9730-134">String</span><span class="sxs-lookup"><span data-stu-id="c9730-134">String</span></span>|<span data-ttu-id="c9730-135">Уникальный идентификатор для внедренных состояние устройства диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="c9730-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="c9730-136">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="c9730-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="c9730-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9730-137">createdDateTime</span></span>|<span data-ttu-id="c9730-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9730-138">DateTimeOffset</span></span>|<span data-ttu-id="c9730-139">Время создания внедренных состояние устройства диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="c9730-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="c9730-140">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="c9730-140">Generated service side.</span></span>|
|<span data-ttu-id="c9730-141">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9730-141">modifiedDateTime</span></span>|<span data-ttu-id="c9730-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9730-142">DateTimeOffset</span></span>|<span data-ttu-id="c9730-143">Время последнего изменения внедренного состояние устройства диспетчера установки.</span><span class="sxs-lookup"><span data-stu-id="c9730-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="c9730-144">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="c9730-144">Updated service side.</span></span>|
|<span data-ttu-id="c9730-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c9730-145">lastSyncDateTime</span></span>|<span data-ttu-id="c9730-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9730-146">DateTimeOffset</span></span>|<span data-ttu-id="c9730-147">Время, внедренные устройства диспетчера установки последнего возврата.</span><span class="sxs-lookup"><span data-stu-id="c9730-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="c9730-148">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="c9730-148">Updated service side.</span></span>|
|<span data-ttu-id="c9730-149">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="c9730-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="c9730-150">String</span><span class="sxs-lookup"><span data-stu-id="c9730-150">String</span></span>|<span data-ttu-id="c9730-151">Универсальные интегральной карточки идентификатор (UICCID) Идентификация оборудования, на котором профиль — для развертывания.</span><span class="sxs-lookup"><span data-stu-id="c9730-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="c9730-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="c9730-152">deviceName</span></span>|<span data-ttu-id="c9730-153">String</span><span class="sxs-lookup"><span data-stu-id="c9730-153">String</span></span>|<span data-ttu-id="c9730-154">Имя устройства, к которому был подписки например рабочего СТОЛА ДЖО подготовить к работе</span><span class="sxs-lookup"><span data-stu-id="c9730-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="c9730-155">userName</span><span class="sxs-lookup"><span data-stu-id="c9730-155">userName</span></span>|<span data-ttu-id="c9730-156">String</span><span class="sxs-lookup"><span data-stu-id="c9730-156">String</span></span>|<span data-ttu-id="c9730-157">Имя пользователя, который был подписки подготовлен к например joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="c9730-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="c9730-158">state</span><span class="sxs-lookup"><span data-stu-id="c9730-158">state</span></span>|[<span data-ttu-id="c9730-159">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="c9730-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="c9730-160">Состояние операции профилей, применяемые к устройства.</span><span class="sxs-lookup"><span data-stu-id="c9730-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="c9730-161">Возможные значения: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span><span class="sxs-lookup"><span data-stu-id="c9730-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="c9730-162">stateDetails</span><span class="sxs-lookup"><span data-stu-id="c9730-162">stateDetails</span></span>|<span data-ttu-id="c9730-163">String</span><span class="sxs-lookup"><span data-stu-id="c9730-163">String</span></span>|<span data-ttu-id="c9730-164">Строка Описание подготовки состояния.</span><span class="sxs-lookup"><span data-stu-id="c9730-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="c9730-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9730-165">Response</span></span>
<span data-ttu-id="c9730-166">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c9730-166">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9730-167">Пример</span><span class="sxs-lookup"><span data-stu-id="c9730-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9730-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9730-168">Request</span></span>
<span data-ttu-id="c9730-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9730-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c9730-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9730-170">Response</span></span>
<span data-ttu-id="c9730-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c9730-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





