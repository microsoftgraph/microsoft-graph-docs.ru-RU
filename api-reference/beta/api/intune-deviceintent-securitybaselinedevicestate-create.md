---
title: Создание securityBaselineDeviceState
description: Создайте новый объект securityBaselineDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 498c9799315ba844001c82058915e8b0ec68a548
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131990"
---
# <a name="create-securitybaselinedevicestate"></a><span data-ttu-id="88f7b-103">Создание securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="88f7b-103">Create securityBaselineDeviceState</span></span>

<span data-ttu-id="88f7b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88f7b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88f7b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88f7b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88f7b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88f7b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88f7b-107">Создайте новый [объект securityBaselineDeviceState.](../resources/intune-deviceintent-securitybaselinedevicestate.md)</span><span class="sxs-lookup"><span data-stu-id="88f7b-107">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88f7b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="88f7b-108">Prerequisites</span></span>
<span data-ttu-id="88f7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88f7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88f7b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88f7b-111">Permission type</span></span>|<span data-ttu-id="88f7b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88f7b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88f7b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88f7b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88f7b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88f7b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88f7b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88f7b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88f7b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88f7b-116">Not supported.</span></span>|
|<span data-ttu-id="88f7b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="88f7b-117">Application</span></span>|<span data-ttu-id="88f7b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88f7b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88f7b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88f7b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="88f7b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="88f7b-120">Request headers</span></span>
|<span data-ttu-id="88f7b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88f7b-121">Header</span></span>|<span data-ttu-id="88f7b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="88f7b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88f7b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="88f7b-123">Authorization</span></span>|<span data-ttu-id="88f7b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88f7b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88f7b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="88f7b-125">Accept</span></span>|<span data-ttu-id="88f7b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88f7b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88f7b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88f7b-127">Request body</span></span>
<span data-ttu-id="88f7b-128">В теле запроса поставляем представление JSON для объекта securityBaselineDeviceState.</span><span class="sxs-lookup"><span data-stu-id="88f7b-128">In the request body, supply a JSON representation for the securityBaselineDeviceState object.</span></span>

<span data-ttu-id="88f7b-129">В следующей таблице показаны свойства, необходимые при создании securityBaselineDeviceState.</span><span class="sxs-lookup"><span data-stu-id="88f7b-129">The following table shows the properties that are required when you create the securityBaselineDeviceState.</span></span>

|<span data-ttu-id="88f7b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="88f7b-130">Property</span></span>|<span data-ttu-id="88f7b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="88f7b-131">Type</span></span>|<span data-ttu-id="88f7b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="88f7b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88f7b-133">id</span><span class="sxs-lookup"><span data-stu-id="88f7b-133">id</span></span>|<span data-ttu-id="88f7b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="88f7b-134">String</span></span>|<span data-ttu-id="88f7b-135">Уникальный идентификатор сущности</span><span class="sxs-lookup"><span data-stu-id="88f7b-135">Unique identifier of the entity</span></span>|
|<span data-ttu-id="88f7b-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="88f7b-136">managedDeviceId</span></span>|<span data-ttu-id="88f7b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="88f7b-137">String</span></span>|<span data-ttu-id="88f7b-138">ID устройства Intune</span><span class="sxs-lookup"><span data-stu-id="88f7b-138">Intune device id</span></span>|
|<span data-ttu-id="88f7b-139">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="88f7b-139">deviceDisplayName</span></span>|<span data-ttu-id="88f7b-140">String</span><span class="sxs-lookup"><span data-stu-id="88f7b-140">String</span></span>|<span data-ttu-id="88f7b-141">Отображение имени устройства</span><span class="sxs-lookup"><span data-stu-id="88f7b-141">Display name of the device</span></span>|
|<span data-ttu-id="88f7b-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="88f7b-142">userPrincipalName</span></span>|<span data-ttu-id="88f7b-143">String</span><span class="sxs-lookup"><span data-stu-id="88f7b-143">String</span></span>|<span data-ttu-id="88f7b-144">"User Principal Name" (Имя участника-пользователя);</span><span class="sxs-lookup"><span data-stu-id="88f7b-144">User Principal Name</span></span>|
|<span data-ttu-id="88f7b-145">state</span><span class="sxs-lookup"><span data-stu-id="88f7b-145">state</span></span>|[<span data-ttu-id="88f7b-146">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="88f7b-146">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="88f7b-147">Состояние соответствия базовым требованиям безопасности.</span><span class="sxs-lookup"><span data-stu-id="88f7b-147">Security baseline compliance state.</span></span> <span data-ttu-id="88f7b-148">Возможные значения: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span><span class="sxs-lookup"><span data-stu-id="88f7b-148">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="88f7b-149">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="88f7b-149">lastReportedDateTime</span></span>|<span data-ttu-id="88f7b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88f7b-150">DateTimeOffset</span></span>|<span data-ttu-id="88f7b-151">Последнее измененное время даты отчета о политике</span><span class="sxs-lookup"><span data-stu-id="88f7b-151">Last modified date time of the policy report</span></span>|



## <a name="response"></a><span data-ttu-id="88f7b-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="88f7b-152">Response</span></span>
<span data-ttu-id="88f7b-153">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="88f7b-153">If successful, this method returns a `201 Created` response code and a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88f7b-154">Пример</span><span class="sxs-lookup"><span data-stu-id="88f7b-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="88f7b-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="88f7b-155">Request</span></span>
<span data-ttu-id="88f7b-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88f7b-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="88f7b-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="88f7b-157">Response</span></span>
<span data-ttu-id="88f7b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88f7b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




