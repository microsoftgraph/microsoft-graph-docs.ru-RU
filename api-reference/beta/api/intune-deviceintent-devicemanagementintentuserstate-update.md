---
title: Обновление Девицеманажементинтентусерстате
description: Обновление свойств объекта Девицеманажементинтентусерстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e138452101628eab3deefd40b34369560ad5e102
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960064"
---
# <a name="update-devicemanagementintentuserstate"></a><span data-ttu-id="8bb55-103">Обновление Девицеманажементинтентусерстате</span><span class="sxs-lookup"><span data-stu-id="8bb55-103">Update deviceManagementIntentUserState</span></span>

> <span data-ttu-id="8bb55-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bb55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bb55-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bb55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bb55-106">Обновление свойств объекта [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="8bb55-106">Update the properties of a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bb55-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8bb55-107">Prerequisites</span></span>
<span data-ttu-id="8bb55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bb55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bb55-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8bb55-110">Permission type</span></span>|<span data-ttu-id="8bb55-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8bb55-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bb55-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bb55-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8bb55-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb55-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8bb55-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bb55-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bb55-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bb55-115">Not supported.</span></span>|
|<span data-ttu-id="8bb55-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8bb55-116">Application</span></span>|<span data-ttu-id="8bb55-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bb55-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bb55-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bb55-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStates/{deviceManagementIntentUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="8bb55-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bb55-119">Request headers</span></span>
|<span data-ttu-id="8bb55-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8bb55-120">Header</span></span>|<span data-ttu-id="8bb55-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8bb55-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bb55-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8bb55-122">Authorization</span></span>|<span data-ttu-id="8bb55-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bb55-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bb55-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8bb55-124">Accept</span></span>|<span data-ttu-id="8bb55-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8bb55-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bb55-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8bb55-126">Request body</span></span>
<span data-ttu-id="8bb55-127">В тексте запроса добавьте представление объекта [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bb55-127">In the request body, supply a JSON representation for the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

<span data-ttu-id="8bb55-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md).</span><span class="sxs-lookup"><span data-stu-id="8bb55-128">The following table shows the properties that are required when you create the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).</span></span>

|<span data-ttu-id="8bb55-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bb55-129">Property</span></span>|<span data-ttu-id="8bb55-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8bb55-130">Type</span></span>|<span data-ttu-id="8bb55-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8bb55-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bb55-132">id</span><span class="sxs-lookup"><span data-stu-id="8bb55-132">id</span></span>|<span data-ttu-id="8bb55-133">Строка</span><span class="sxs-lookup"><span data-stu-id="8bb55-133">String</span></span>|<span data-ttu-id="8bb55-134">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="8bb55-134">The ID</span></span>|
|<span data-ttu-id="8bb55-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8bb55-135">userPrincipalName</span></span>|<span data-ttu-id="8bb55-136">String</span><span class="sxs-lookup"><span data-stu-id="8bb55-136">String</span></span>|<span data-ttu-id="8bb55-137">Имя участника-пользователя, сообщаемое на устройстве</span><span class="sxs-lookup"><span data-stu-id="8bb55-137">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="8bb55-138">userName</span><span class="sxs-lookup"><span data-stu-id="8bb55-138">userName</span></span>|<span data-ttu-id="8bb55-139">String</span><span class="sxs-lookup"><span data-stu-id="8bb55-139">String</span></span>|<span data-ttu-id="8bb55-140">Имя пользователя, сообщаемое на устройстве</span><span class="sxs-lookup"><span data-stu-id="8bb55-140">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="8bb55-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="8bb55-141">deviceCount</span></span>|<span data-ttu-id="8bb55-142">Int32</span><span class="sxs-lookup"><span data-stu-id="8bb55-142">Int32</span></span>|<span data-ttu-id="8bb55-143">Количество устройств, принадлежащие пользователю для намерения</span><span class="sxs-lookup"><span data-stu-id="8bb55-143">Count of Devices that belongs to a user for an intent</span></span>|
|<span data-ttu-id="8bb55-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="8bb55-144">lastReportedDateTime</span></span>|<span data-ttu-id="8bb55-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bb55-145">DateTimeOffset</span></span>|<span data-ttu-id="8bb55-146">Дата и время последнего изменения отчета о намерениях</span><span class="sxs-lookup"><span data-stu-id="8bb55-146">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="8bb55-147">состояние</span><span class="sxs-lookup"><span data-stu-id="8bb55-147">state</span></span>|[<span data-ttu-id="8bb55-148">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="8bb55-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8bb55-149">Состояние пользователя для намерения.</span><span class="sxs-lookup"><span data-stu-id="8bb55-149">User state for an intent.</span></span> <span data-ttu-id="8bb55-150">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="8bb55-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|



## <a name="response"></a><span data-ttu-id="8bb55-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="8bb55-151">Response</span></span>
<span data-ttu-id="8bb55-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8bb55-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bb55-153">Пример</span><span class="sxs-lookup"><span data-stu-id="8bb55-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bb55-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bb55-154">Request</span></span>
<span data-ttu-id="8bb55-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bb55-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8bb55-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bb55-156">Response</span></span>
<span data-ttu-id="8bb55-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8bb55-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





