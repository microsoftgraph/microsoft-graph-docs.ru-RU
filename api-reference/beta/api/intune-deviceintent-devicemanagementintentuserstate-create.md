---
title: Создание Девицеманажементинтентусерстате
description: Создание нового объекта Девицеманажементинтентусерстате.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eb5d434f2d4b867a245e6b8ac7809733a728af87
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815186"
---
# <a name="create-devicemanagementintentuserstate"></a><span data-ttu-id="e6ed1-103">Создание Девицеманажементинтентусерстате</span><span class="sxs-lookup"><span data-stu-id="e6ed1-103">Create deviceManagementIntentUserState</span></span>

> <span data-ttu-id="e6ed1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6ed1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6ed1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6ed1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6ed1-106">Создание нового объекта [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="e6ed1-106">Create a new [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6ed1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e6ed1-107">Prerequisites</span></span>
<span data-ttu-id="e6ed1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6ed1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6ed1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6ed1-110">Permission type</span></span>|<span data-ttu-id="e6ed1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6ed1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6ed1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6ed1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e6ed1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6ed1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6ed1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6ed1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6ed1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6ed1-115">Not supported.</span></span>|
|<span data-ttu-id="e6ed1-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e6ed1-116">Application</span></span>|<span data-ttu-id="e6ed1-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6ed1-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6ed1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6ed1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/userStates
```

## <a name="request-headers"></a><span data-ttu-id="e6ed1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e6ed1-119">Request headers</span></span>
|<span data-ttu-id="e6ed1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6ed1-120">Header</span></span>|<span data-ttu-id="e6ed1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e6ed1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6ed1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6ed1-122">Authorization</span></span>|<span data-ttu-id="e6ed1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6ed1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6ed1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e6ed1-124">Accept</span></span>|<span data-ttu-id="e6ed1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e6ed1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6ed1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6ed1-126">Request body</span></span>
<span data-ttu-id="e6ed1-127">В тексте запроса добавьте представление объекта Девицеманажементинтентусерстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6ed1-127">In the request body, supply a JSON representation for the deviceManagementIntentUserState object.</span></span>

<span data-ttu-id="e6ed1-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтентусерстате.</span><span class="sxs-lookup"><span data-stu-id="e6ed1-128">The following table shows the properties that are required when you create the deviceManagementIntentUserState.</span></span>

|<span data-ttu-id="e6ed1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6ed1-129">Property</span></span>|<span data-ttu-id="e6ed1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e6ed1-130">Type</span></span>|<span data-ttu-id="e6ed1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e6ed1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6ed1-132">id</span><span class="sxs-lookup"><span data-stu-id="e6ed1-132">id</span></span>|<span data-ttu-id="e6ed1-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e6ed1-133">String</span></span>|<span data-ttu-id="e6ed1-134">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="e6ed1-134">The ID</span></span>|
|<span data-ttu-id="e6ed1-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e6ed1-135">userPrincipalName</span></span>|<span data-ttu-id="e6ed1-136">String</span><span class="sxs-lookup"><span data-stu-id="e6ed1-136">String</span></span>|<span data-ttu-id="e6ed1-137">Имя участника-пользователя, сообщаемое на устройстве</span><span class="sxs-lookup"><span data-stu-id="e6ed1-137">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="e6ed1-138">userName</span><span class="sxs-lookup"><span data-stu-id="e6ed1-138">userName</span></span>|<span data-ttu-id="e6ed1-139">String</span><span class="sxs-lookup"><span data-stu-id="e6ed1-139">String</span></span>|<span data-ttu-id="e6ed1-140">Имя пользователя, сообщаемое на устройстве</span><span class="sxs-lookup"><span data-stu-id="e6ed1-140">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="e6ed1-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="e6ed1-141">deviceCount</span></span>|<span data-ttu-id="e6ed1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e6ed1-142">Int32</span></span>|<span data-ttu-id="e6ed1-143">Количество устройств, принадлежащие пользователю для намерения</span><span class="sxs-lookup"><span data-stu-id="e6ed1-143">Count of Devices that belongs to a user for an intent</span></span>|
|<span data-ttu-id="e6ed1-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6ed1-144">lastReportedDateTime</span></span>|<span data-ttu-id="e6ed1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6ed1-145">DateTimeOffset</span></span>|<span data-ttu-id="e6ed1-146">Дата и время последнего изменения отчета о намерениях</span><span class="sxs-lookup"><span data-stu-id="e6ed1-146">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="e6ed1-147">state</span><span class="sxs-lookup"><span data-stu-id="e6ed1-147">state</span></span>|[<span data-ttu-id="e6ed1-148">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="e6ed1-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e6ed1-149">Состояние пользователя для намерения.</span><span class="sxs-lookup"><span data-stu-id="e6ed1-149">User state for an intent.</span></span> <span data-ttu-id="e6ed1-150">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="e6ed1-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|



## <a name="response"></a><span data-ttu-id="e6ed1-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6ed1-151">Response</span></span>
<span data-ttu-id="e6ed1-152">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6ed1-152">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6ed1-153">Пример</span><span class="sxs-lookup"><span data-stu-id="e6ed1-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6ed1-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6ed1-154">Request</span></span>
<span data-ttu-id="e6ed1-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6ed1-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates
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

### <a name="response"></a><span data-ttu-id="e6ed1-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6ed1-156">Response</span></span>
<span data-ttu-id="e6ed1-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6ed1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




