---
title: Создание Девицеманажементинтентусерстате
description: Создание нового объекта Девицеманажементинтентусерстате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6f0ff431c09acc221d120faa4da9a8d0cb9f48d3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275225"
---
# <a name="create-devicemanagementintentuserstate"></a><span data-ttu-id="76451-103">Создание Девицеманажементинтентусерстате</span><span class="sxs-lookup"><span data-stu-id="76451-103">Create deviceManagementIntentUserState</span></span>

<span data-ttu-id="76451-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76451-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76451-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76451-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76451-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76451-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76451-107">Создание нового объекта [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="76451-107">Create a new [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76451-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="76451-108">Prerequisites</span></span>
<span data-ttu-id="76451-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76451-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76451-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76451-111">Permission type</span></span>|<span data-ttu-id="76451-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="76451-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76451-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76451-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76451-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76451-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76451-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76451-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76451-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76451-116">Not supported.</span></span>|
|<span data-ttu-id="76451-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76451-117">Application</span></span>|<span data-ttu-id="76451-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76451-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76451-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76451-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/userStates
```

## <a name="request-headers"></a><span data-ttu-id="76451-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="76451-120">Request headers</span></span>
|<span data-ttu-id="76451-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="76451-121">Header</span></span>|<span data-ttu-id="76451-122">Значение</span><span class="sxs-lookup"><span data-stu-id="76451-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76451-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76451-123">Authorization</span></span>|<span data-ttu-id="76451-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76451-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76451-125">Accept</span><span class="sxs-lookup"><span data-stu-id="76451-125">Accept</span></span>|<span data-ttu-id="76451-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76451-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76451-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76451-127">Request body</span></span>
<span data-ttu-id="76451-128">В тексте запроса добавьте представление объекта Девицеманажементинтентусерстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76451-128">In the request body, supply a JSON representation for the deviceManagementIntentUserState object.</span></span>

<span data-ttu-id="76451-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтентусерстате.</span><span class="sxs-lookup"><span data-stu-id="76451-129">The following table shows the properties that are required when you create the deviceManagementIntentUserState.</span></span>

|<span data-ttu-id="76451-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="76451-130">Property</span></span>|<span data-ttu-id="76451-131">Тип</span><span class="sxs-lookup"><span data-stu-id="76451-131">Type</span></span>|<span data-ttu-id="76451-132">Описание</span><span class="sxs-lookup"><span data-stu-id="76451-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76451-133">id</span><span class="sxs-lookup"><span data-stu-id="76451-133">id</span></span>|<span data-ttu-id="76451-134">String</span><span class="sxs-lookup"><span data-stu-id="76451-134">String</span></span>|<span data-ttu-id="76451-135">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="76451-135">The ID</span></span>|
|<span data-ttu-id="76451-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="76451-136">userPrincipalName</span></span>|<span data-ttu-id="76451-137">String</span><span class="sxs-lookup"><span data-stu-id="76451-137">String</span></span>|<span data-ttu-id="76451-138">Имя участника-пользователя, сообщаемое на устройстве</span><span class="sxs-lookup"><span data-stu-id="76451-138">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="76451-139">userName</span><span class="sxs-lookup"><span data-stu-id="76451-139">userName</span></span>|<span data-ttu-id="76451-140">String</span><span class="sxs-lookup"><span data-stu-id="76451-140">String</span></span>|<span data-ttu-id="76451-141">Имя пользователя, сообщаемое на устройстве</span><span class="sxs-lookup"><span data-stu-id="76451-141">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="76451-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="76451-142">deviceCount</span></span>|<span data-ttu-id="76451-143">Int32</span><span class="sxs-lookup"><span data-stu-id="76451-143">Int32</span></span>|<span data-ttu-id="76451-144">Количество устройств, принадлежащие пользователю для намерения</span><span class="sxs-lookup"><span data-stu-id="76451-144">Count of Devices that belongs to a user for an intent</span></span>|
|<span data-ttu-id="76451-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="76451-145">lastReportedDateTime</span></span>|<span data-ttu-id="76451-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76451-146">DateTimeOffset</span></span>|<span data-ttu-id="76451-147">Дата и время последнего изменения отчета о намерениях</span><span class="sxs-lookup"><span data-stu-id="76451-147">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="76451-148">state</span><span class="sxs-lookup"><span data-stu-id="76451-148">state</span></span>|[<span data-ttu-id="76451-149">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="76451-149">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="76451-150">Состояние пользователя для намерения.</span><span class="sxs-lookup"><span data-stu-id="76451-150">User state for an intent.</span></span> <span data-ttu-id="76451-151">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="76451-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|



## <a name="response"></a><span data-ttu-id="76451-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="76451-152">Response</span></span>
<span data-ttu-id="76451-153">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="76451-153">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76451-154">Пример</span><span class="sxs-lookup"><span data-stu-id="76451-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="76451-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="76451-155">Request</span></span>
<span data-ttu-id="76451-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76451-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="76451-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="76451-157">Response</span></span>
<span data-ttu-id="76451-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76451-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




