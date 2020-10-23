---
title: Обновление Девицеманажементинтентусерстате
description: Обновление свойств объекта Девицеманажементинтентусерстате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf8d95b499c6ccb0ab9c1f9d314a84ec2de67002
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734422"
---
# <a name="update-devicemanagementintentuserstate"></a><span data-ttu-id="23916-103">Обновление Девицеманажементинтентусерстате</span><span class="sxs-lookup"><span data-stu-id="23916-103">Update deviceManagementIntentUserState</span></span>

<span data-ttu-id="23916-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23916-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23916-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23916-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23916-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23916-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23916-107">Обновление свойств объекта [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="23916-107">Update the properties of a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23916-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="23916-108">Prerequisites</span></span>
<span data-ttu-id="23916-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23916-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23916-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23916-111">Permission type</span></span>|<span data-ttu-id="23916-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="23916-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23916-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23916-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23916-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23916-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23916-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23916-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23916-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23916-116">Not supported.</span></span>|
|<span data-ttu-id="23916-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23916-117">Application</span></span>|<span data-ttu-id="23916-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23916-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23916-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23916-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="23916-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="23916-120">Request headers</span></span>
|<span data-ttu-id="23916-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23916-121">Header</span></span>|<span data-ttu-id="23916-122">Значение</span><span class="sxs-lookup"><span data-stu-id="23916-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23916-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23916-123">Authorization</span></span>|<span data-ttu-id="23916-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23916-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23916-125">Accept</span><span class="sxs-lookup"><span data-stu-id="23916-125">Accept</span></span>|<span data-ttu-id="23916-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23916-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23916-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="23916-127">Request body</span></span>
<span data-ttu-id="23916-128">В тексте запроса добавьте представление объекта [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23916-128">In the request body, supply a JSON representation for the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

<span data-ttu-id="23916-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md).</span><span class="sxs-lookup"><span data-stu-id="23916-129">The following table shows the properties that are required when you create the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).</span></span>

|<span data-ttu-id="23916-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="23916-130">Property</span></span>|<span data-ttu-id="23916-131">Тип</span><span class="sxs-lookup"><span data-stu-id="23916-131">Type</span></span>|<span data-ttu-id="23916-132">Описание</span><span class="sxs-lookup"><span data-stu-id="23916-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23916-133">id</span><span class="sxs-lookup"><span data-stu-id="23916-133">id</span></span>|<span data-ttu-id="23916-134">Строка</span><span class="sxs-lookup"><span data-stu-id="23916-134">String</span></span>|<span data-ttu-id="23916-135">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="23916-135">The ID</span></span>|
|<span data-ttu-id="23916-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="23916-136">userPrincipalName</span></span>|<span data-ttu-id="23916-137">String</span><span class="sxs-lookup"><span data-stu-id="23916-137">String</span></span>|<span data-ttu-id="23916-138">Имя участника-пользователя, сообщаемое на устройстве</span><span class="sxs-lookup"><span data-stu-id="23916-138">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="23916-139">userName</span><span class="sxs-lookup"><span data-stu-id="23916-139">userName</span></span>|<span data-ttu-id="23916-140">String</span><span class="sxs-lookup"><span data-stu-id="23916-140">String</span></span>|<span data-ttu-id="23916-141">Имя пользователя, сообщаемое на устройстве</span><span class="sxs-lookup"><span data-stu-id="23916-141">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="23916-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="23916-142">deviceCount</span></span>|<span data-ttu-id="23916-143">Int32</span><span class="sxs-lookup"><span data-stu-id="23916-143">Int32</span></span>|<span data-ttu-id="23916-144">Количество устройств, принадлежащие пользователю для намерения</span><span class="sxs-lookup"><span data-stu-id="23916-144">Count of Devices that belongs to a user for an intent</span></span>|
|<span data-ttu-id="23916-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="23916-145">lastReportedDateTime</span></span>|<span data-ttu-id="23916-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23916-146">DateTimeOffset</span></span>|<span data-ttu-id="23916-147">Дата и время последнего изменения отчета о намерениях</span><span class="sxs-lookup"><span data-stu-id="23916-147">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="23916-148">state</span><span class="sxs-lookup"><span data-stu-id="23916-148">state</span></span>|[<span data-ttu-id="23916-149">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="23916-149">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="23916-150">Состояние пользователя для намерения.</span><span class="sxs-lookup"><span data-stu-id="23916-150">User state for an intent.</span></span> <span data-ttu-id="23916-151">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="23916-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|



## <a name="response"></a><span data-ttu-id="23916-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="23916-152">Response</span></span>
<span data-ttu-id="23916-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23916-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23916-154">Пример</span><span class="sxs-lookup"><span data-stu-id="23916-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="23916-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="23916-155">Request</span></span>
<span data-ttu-id="23916-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23916-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceCount": 11,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable"
}
```

### <a name="response"></a><span data-ttu-id="23916-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="23916-157">Response</span></span>
<span data-ttu-id="23916-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23916-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "id": "0201286a-286a-0201-6a28-01026a280102",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceCount": 11,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable"
}
```





