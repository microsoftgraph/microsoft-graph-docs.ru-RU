---
title: Создание Секуритибаселинедевицестате
description: Создание нового объекта Секуритибаселинедевицестате.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 03caf18e233369e8294337163f5ab0e8c123ab4b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814899"
---
# <a name="create-securitybaselinedevicestate"></a><span data-ttu-id="15513-103">Создание Секуритибаселинедевицестате</span><span class="sxs-lookup"><span data-stu-id="15513-103">Create securityBaselineDeviceState</span></span>

> <span data-ttu-id="15513-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15513-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15513-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15513-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15513-106">Создание нового объекта [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="15513-106">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15513-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="15513-107">Prerequisites</span></span>
<span data-ttu-id="15513-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15513-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15513-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15513-110">Permission type</span></span>|<span data-ttu-id="15513-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15513-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15513-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15513-112">Delegated (work or school account)</span></span>|<span data-ttu-id="15513-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15513-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15513-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15513-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15513-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15513-115">Not supported.</span></span>|
|<span data-ttu-id="15513-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="15513-116">Application</span></span>|<span data-ttu-id="15513-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15513-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15513-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15513-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="15513-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="15513-119">Request headers</span></span>
|<span data-ttu-id="15513-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15513-120">Header</span></span>|<span data-ttu-id="15513-121">Значение</span><span class="sxs-lookup"><span data-stu-id="15513-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15513-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="15513-122">Authorization</span></span>|<span data-ttu-id="15513-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15513-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15513-124">Accept</span><span class="sxs-lookup"><span data-stu-id="15513-124">Accept</span></span>|<span data-ttu-id="15513-125">application/json</span><span class="sxs-lookup"><span data-stu-id="15513-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15513-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15513-126">Request body</span></span>
<span data-ttu-id="15513-127">В тексте запроса добавьте представление объекта Секуритибаселинедевицестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15513-127">In the request body, supply a JSON representation for the securityBaselineDeviceState object.</span></span>

<span data-ttu-id="15513-128">В следующей таблице приведены свойства, необходимые при создании Секуритибаселинедевицестате.</span><span class="sxs-lookup"><span data-stu-id="15513-128">The following table shows the properties that are required when you create the securityBaselineDeviceState.</span></span>

|<span data-ttu-id="15513-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="15513-129">Property</span></span>|<span data-ttu-id="15513-130">Тип</span><span class="sxs-lookup"><span data-stu-id="15513-130">Type</span></span>|<span data-ttu-id="15513-131">Описание</span><span class="sxs-lookup"><span data-stu-id="15513-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15513-132">id</span><span class="sxs-lookup"><span data-stu-id="15513-132">id</span></span>|<span data-ttu-id="15513-133">Строка</span><span class="sxs-lookup"><span data-stu-id="15513-133">String</span></span>|<span data-ttu-id="15513-134">Уникальный идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="15513-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="15513-135">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="15513-135">managedDeviceId</span></span>|<span data-ttu-id="15513-136">String</span><span class="sxs-lookup"><span data-stu-id="15513-136">String</span></span>|<span data-ttu-id="15513-137">Идентификатор устройства Intune</span><span class="sxs-lookup"><span data-stu-id="15513-137">Intune device id</span></span>|
|<span data-ttu-id="15513-138">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="15513-138">deviceDisplayName</span></span>|<span data-ttu-id="15513-139">String</span><span class="sxs-lookup"><span data-stu-id="15513-139">String</span></span>|<span data-ttu-id="15513-140">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="15513-140">Display name of the device</span></span>|
|<span data-ttu-id="15513-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="15513-141">userPrincipalName</span></span>|<span data-ttu-id="15513-142">String</span><span class="sxs-lookup"><span data-stu-id="15513-142">String</span></span>|<span data-ttu-id="15513-143">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="15513-143">User Principal Name</span></span>|
|<span data-ttu-id="15513-144">state</span><span class="sxs-lookup"><span data-stu-id="15513-144">state</span></span>|[<span data-ttu-id="15513-145">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="15513-145">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="15513-146">Состояние соответствия нормативным требованиям безопасности.</span><span class="sxs-lookup"><span data-stu-id="15513-146">Security baseline compliance state.</span></span> <span data-ttu-id="15513-147">Возможные значения: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="15513-147">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="15513-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="15513-148">lastReportedDateTime</span></span>|<span data-ttu-id="15513-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15513-149">DateTimeOffset</span></span>|<span data-ttu-id="15513-150">Дата и время последнего изменения отчета о политике</span><span class="sxs-lookup"><span data-stu-id="15513-150">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="15513-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="15513-151">Response</span></span>
<span data-ttu-id="15513-152">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15513-152">If successful, this method returns a `201 Created` response code and a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15513-153">Пример</span><span class="sxs-lookup"><span data-stu-id="15513-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="15513-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="15513-154">Request</span></span>
<span data-ttu-id="15513-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15513-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="15513-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="15513-156">Response</span></span>
<span data-ttu-id="15513-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15513-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




