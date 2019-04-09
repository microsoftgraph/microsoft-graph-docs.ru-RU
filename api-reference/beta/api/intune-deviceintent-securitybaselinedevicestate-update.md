---
title: Обновление Секуритибаселинедевицестате
description: Обновление свойств объекта Секуритибаселинедевицестате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1797f166fea7eb3507ae6a477ae574f4146c558
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522694"
---
# <a name="update-securitybaselinedevicestate"></a><span data-ttu-id="d09e2-103">Обновление Секуритибаселинедевицестате</span><span class="sxs-lookup"><span data-stu-id="d09e2-103">Update securityBaselineDeviceState</span></span>

> <span data-ttu-id="d09e2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d09e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d09e2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d09e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d09e2-106">Обновление свойств объекта [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="d09e2-106">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d09e2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d09e2-107">Prerequisites</span></span>
<span data-ttu-id="d09e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d09e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d09e2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d09e2-110">Permission type</span></span>|<span data-ttu-id="d09e2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d09e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d09e2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d09e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d09e2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d09e2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d09e2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d09e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d09e2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d09e2-115">Not supported.</span></span>|
|<span data-ttu-id="d09e2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d09e2-116">Application</span></span>|<span data-ttu-id="d09e2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d09e2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d09e2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d09e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates/{securityBaselineDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="d09e2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d09e2-119">Request headers</span></span>
|<span data-ttu-id="d09e2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d09e2-120">Header</span></span>|<span data-ttu-id="d09e2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d09e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d09e2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d09e2-122">Authorization</span></span>|<span data-ttu-id="d09e2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d09e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d09e2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d09e2-124">Accept</span></span>|<span data-ttu-id="d09e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d09e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d09e2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d09e2-126">Request body</span></span>
<span data-ttu-id="d09e2-127">В тексте запроса добавьте представление объекта [Секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d09e2-127">In the request body, supply a JSON representation for the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

<span data-ttu-id="d09e2-128">В следующей таблице приведены свойства, необходимые при создании [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span><span class="sxs-lookup"><span data-stu-id="d09e2-128">The following table shows the properties that are required when you create the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>

|<span data-ttu-id="d09e2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d09e2-129">Property</span></span>|<span data-ttu-id="d09e2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d09e2-130">Type</span></span>|<span data-ttu-id="d09e2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d09e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d09e2-132">id</span><span class="sxs-lookup"><span data-stu-id="d09e2-132">id</span></span>|<span data-ttu-id="d09e2-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d09e2-133">String</span></span>|<span data-ttu-id="d09e2-134">Уникальный идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="d09e2-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="d09e2-135">Манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="d09e2-135">managedDeviceId</span></span>|<span data-ttu-id="d09e2-136">String</span><span class="sxs-lookup"><span data-stu-id="d09e2-136">String</span></span>|<span data-ttu-id="d09e2-137">Идентификатор устройства Intune</span><span class="sxs-lookup"><span data-stu-id="d09e2-137">Intune device id</span></span>|
|<span data-ttu-id="d09e2-138">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d09e2-138">deviceDisplayName</span></span>|<span data-ttu-id="d09e2-139">String</span><span class="sxs-lookup"><span data-stu-id="d09e2-139">String</span></span>|<span data-ttu-id="d09e2-140">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="d09e2-140">Display name of the device</span></span>|
|<span data-ttu-id="d09e2-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d09e2-141">userPrincipalName</span></span>|<span data-ttu-id="d09e2-142">String</span><span class="sxs-lookup"><span data-stu-id="d09e2-142">String</span></span>|<span data-ttu-id="d09e2-143">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="d09e2-143">User Principal Name</span></span>|
|<span data-ttu-id="d09e2-144">state</span><span class="sxs-lookup"><span data-stu-id="d09e2-144">state</span></span>|[<span data-ttu-id="d09e2-145">Секуритибаселинекомплианцестате</span><span class="sxs-lookup"><span data-stu-id="d09e2-145">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="d09e2-146">Состояние соответствия нормативным требованиям безопасности.</span><span class="sxs-lookup"><span data-stu-id="d09e2-146">Security baseline compliance state.</span></span> <span data-ttu-id="d09e2-147">Возможные значения: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="d09e2-147">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="d09e2-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="d09e2-148">lastReportedDateTime</span></span>|<span data-ttu-id="d09e2-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d09e2-149">DateTimeOffset</span></span>|<span data-ttu-id="d09e2-150">Дата и время последнего изменения отчета о политике</span><span class="sxs-lookup"><span data-stu-id="d09e2-150">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="d09e2-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="d09e2-151">Response</span></span>
<span data-ttu-id="d09e2-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d09e2-152">If successful, this method returns a `200 OK` response code and an updated [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d09e2-153">Пример</span><span class="sxs-lookup"><span data-stu-id="d09e2-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="d09e2-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="d09e2-154">Request</span></span>
<span data-ttu-id="d09e2-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d09e2-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d09e2-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="d09e2-156">Response</span></span>
<span data-ttu-id="d09e2-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d09e2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







