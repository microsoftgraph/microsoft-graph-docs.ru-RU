---
title: Создание Секуритибаселинедевицестате
description: Создание нового объекта Секуритибаселинедевицестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bdd9637aae1b66f71077a4008e3bcc5b3d4cc0c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058944"
---
# <a name="create-securitybaselinedevicestate"></a><span data-ttu-id="874b3-103">Создание Секуритибаселинедевицестате</span><span class="sxs-lookup"><span data-stu-id="874b3-103">Create securityBaselineDeviceState</span></span>

<span data-ttu-id="874b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="874b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="874b3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="874b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="874b3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="874b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="874b3-107">Создание нового объекта [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="874b3-107">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="874b3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="874b3-108">Prerequisites</span></span>
<span data-ttu-id="874b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="874b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="874b3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="874b3-111">Permission type</span></span>|<span data-ttu-id="874b3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="874b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="874b3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="874b3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="874b3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="874b3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="874b3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="874b3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="874b3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="874b3-116">Not supported.</span></span>|
|<span data-ttu-id="874b3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="874b3-117">Application</span></span>|<span data-ttu-id="874b3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="874b3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="874b3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="874b3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="874b3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="874b3-120">Request headers</span></span>
|<span data-ttu-id="874b3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="874b3-121">Header</span></span>|<span data-ttu-id="874b3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="874b3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="874b3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="874b3-123">Authorization</span></span>|<span data-ttu-id="874b3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="874b3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="874b3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="874b3-125">Accept</span></span>|<span data-ttu-id="874b3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="874b3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="874b3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="874b3-127">Request body</span></span>
<span data-ttu-id="874b3-128">В тексте запроса добавьте представление объекта Секуритибаселинедевицестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="874b3-128">In the request body, supply a JSON representation for the securityBaselineDeviceState object.</span></span>

<span data-ttu-id="874b3-129">В следующей таблице приведены свойства, необходимые при создании Секуритибаселинедевицестате.</span><span class="sxs-lookup"><span data-stu-id="874b3-129">The following table shows the properties that are required when you create the securityBaselineDeviceState.</span></span>

|<span data-ttu-id="874b3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="874b3-130">Property</span></span>|<span data-ttu-id="874b3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="874b3-131">Type</span></span>|<span data-ttu-id="874b3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="874b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="874b3-133">id</span><span class="sxs-lookup"><span data-stu-id="874b3-133">id</span></span>|<span data-ttu-id="874b3-134">String</span><span class="sxs-lookup"><span data-stu-id="874b3-134">String</span></span>|<span data-ttu-id="874b3-135">Уникальный идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="874b3-135">Unique identifier of the entity</span></span>|
|<span data-ttu-id="874b3-136">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="874b3-136">managedDeviceId</span></span>|<span data-ttu-id="874b3-137">String</span><span class="sxs-lookup"><span data-stu-id="874b3-137">String</span></span>|<span data-ttu-id="874b3-138">Идентификатор устройства Intune</span><span class="sxs-lookup"><span data-stu-id="874b3-138">Intune device id</span></span>|
|<span data-ttu-id="874b3-139">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="874b3-139">deviceDisplayName</span></span>|<span data-ttu-id="874b3-140">String</span><span class="sxs-lookup"><span data-stu-id="874b3-140">String</span></span>|<span data-ttu-id="874b3-141">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="874b3-141">Display name of the device</span></span>|
|<span data-ttu-id="874b3-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="874b3-142">userPrincipalName</span></span>|<span data-ttu-id="874b3-143">String</span><span class="sxs-lookup"><span data-stu-id="874b3-143">String</span></span>|<span data-ttu-id="874b3-144">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="874b3-144">User Principal Name</span></span>|
|<span data-ttu-id="874b3-145">state</span><span class="sxs-lookup"><span data-stu-id="874b3-145">state</span></span>|[<span data-ttu-id="874b3-146">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="874b3-146">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="874b3-147">Состояние соответствия нормативным требованиям безопасности.</span><span class="sxs-lookup"><span data-stu-id="874b3-147">Security baseline compliance state.</span></span> <span data-ttu-id="874b3-148">Возможные значения: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="874b3-148">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="874b3-149">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="874b3-149">lastReportedDateTime</span></span>|<span data-ttu-id="874b3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="874b3-150">DateTimeOffset</span></span>|<span data-ttu-id="874b3-151">Дата и время последнего изменения отчета о политике</span><span class="sxs-lookup"><span data-stu-id="874b3-151">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="874b3-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="874b3-152">Response</span></span>
<span data-ttu-id="874b3-153">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="874b3-153">If successful, this method returns a `201 Created` response code and a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="874b3-154">Пример</span><span class="sxs-lookup"><span data-stu-id="874b3-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="874b3-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="874b3-155">Request</span></span>
<span data-ttu-id="874b3-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="874b3-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
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

### <a name="response"></a><span data-ttu-id="874b3-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="874b3-157">Response</span></span>
<span data-ttu-id="874b3-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="874b3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






