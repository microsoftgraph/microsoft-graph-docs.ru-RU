---
title: Обновление Секуритибаселинедевицестате
description: Обновление свойств объекта Секуритибаселинедевицестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 18efc12260a92a258edde460d2ebe3875f50e86d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040882"
---
# <a name="update-securitybaselinedevicestate"></a><span data-ttu-id="e83c5-103">Обновление Секуритибаселинедевицестате</span><span class="sxs-lookup"><span data-stu-id="e83c5-103">Update securityBaselineDeviceState</span></span>

<span data-ttu-id="e83c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e83c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e83c5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e83c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e83c5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e83c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e83c5-107">Обновление свойств объекта [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="e83c5-107">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e83c5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e83c5-108">Prerequisites</span></span>
<span data-ttu-id="e83c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e83c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e83c5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e83c5-111">Permission type</span></span>|<span data-ttu-id="e83c5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e83c5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e83c5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e83c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e83c5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e83c5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e83c5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e83c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e83c5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e83c5-116">Not supported.</span></span>|
|<span data-ttu-id="e83c5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e83c5-117">Application</span></span>|<span data-ttu-id="e83c5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e83c5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e83c5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e83c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="e83c5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e83c5-120">Request headers</span></span>
|<span data-ttu-id="e83c5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e83c5-121">Header</span></span>|<span data-ttu-id="e83c5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e83c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e83c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e83c5-123">Authorization</span></span>|<span data-ttu-id="e83c5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e83c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e83c5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e83c5-125">Accept</span></span>|<span data-ttu-id="e83c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e83c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e83c5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e83c5-127">Request body</span></span>
<span data-ttu-id="e83c5-128">В тексте запроса добавьте представление объекта [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e83c5-128">In the request body, supply a JSON representation for the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

<span data-ttu-id="e83c5-129">В следующей таблице приведены свойства, необходимые при создании [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="e83c5-129">The following table shows the properties that are required when you create the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>

|<span data-ttu-id="e83c5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e83c5-130">Property</span></span>|<span data-ttu-id="e83c5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e83c5-131">Type</span></span>|<span data-ttu-id="e83c5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e83c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e83c5-133">id</span><span class="sxs-lookup"><span data-stu-id="e83c5-133">id</span></span>|<span data-ttu-id="e83c5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e83c5-134">String</span></span>|<span data-ttu-id="e83c5-135">Уникальный идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="e83c5-135">Unique identifier of the entity</span></span>|
|<span data-ttu-id="e83c5-136">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="e83c5-136">managedDeviceId</span></span>|<span data-ttu-id="e83c5-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e83c5-137">String</span></span>|<span data-ttu-id="e83c5-138">Идентификатор устройства Intune</span><span class="sxs-lookup"><span data-stu-id="e83c5-138">Intune device id</span></span>|
|<span data-ttu-id="e83c5-139">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e83c5-139">deviceDisplayName</span></span>|<span data-ttu-id="e83c5-140">String</span><span class="sxs-lookup"><span data-stu-id="e83c5-140">String</span></span>|<span data-ttu-id="e83c5-141">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="e83c5-141">Display name of the device</span></span>|
|<span data-ttu-id="e83c5-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e83c5-142">userPrincipalName</span></span>|<span data-ttu-id="e83c5-143">String</span><span class="sxs-lookup"><span data-stu-id="e83c5-143">String</span></span>|<span data-ttu-id="e83c5-144">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="e83c5-144">User Principal Name</span></span>|
|<span data-ttu-id="e83c5-145">state</span><span class="sxs-lookup"><span data-stu-id="e83c5-145">state</span></span>|[<span data-ttu-id="e83c5-146">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="e83c5-146">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="e83c5-147">Состояние соответствия нормативным требованиям безопасности.</span><span class="sxs-lookup"><span data-stu-id="e83c5-147">Security baseline compliance state.</span></span> <span data-ttu-id="e83c5-148">Возможные значения: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="e83c5-148">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="e83c5-149">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e83c5-149">lastReportedDateTime</span></span>|<span data-ttu-id="e83c5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e83c5-150">DateTimeOffset</span></span>|<span data-ttu-id="e83c5-151">Дата и время последнего изменения отчета о политике</span><span class="sxs-lookup"><span data-stu-id="e83c5-151">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="e83c5-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="e83c5-152">Response</span></span>
<span data-ttu-id="e83c5-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e83c5-153">If successful, this method returns a `200 OK` response code and an updated [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e83c5-154">Пример</span><span class="sxs-lookup"><span data-stu-id="e83c5-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="e83c5-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="e83c5-155">Request</span></span>
<span data-ttu-id="e83c5-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e83c5-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
Content-type: application/json
Content-length: 310

{
  "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
  "managedDeviceId": "Managed Device Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "state": "secure",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e83c5-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="e83c5-157">Response</span></span>
<span data-ttu-id="e83c5-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e83c5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
  "id": "182749bf-49bf-1827-bf49-2718bf492718",
  "managedDeviceId": "Managed Device Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "state": "secure",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```






