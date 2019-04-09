---
title: Создание Девицеманажементинтентусерстате
description: Создание нового объекта Девицеманажементинтентусерстате.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76ab09e1d72bb9bc0a8482cd9d71e4e4b0c3f7e6
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522799"
---
# <a name="create-devicemanagementintentuserstate"></a><span data-ttu-id="db5db-103">Создание Девицеманажементинтентусерстате</span><span class="sxs-lookup"><span data-stu-id="db5db-103">Create deviceManagementIntentUserState</span></span>

> <span data-ttu-id="db5db-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db5db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db5db-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db5db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db5db-106">Создание нового объекта [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) .</span><span class="sxs-lookup"><span data-stu-id="db5db-106">Create a new [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db5db-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="db5db-107">Prerequisites</span></span>
<span data-ttu-id="db5db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db5db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db5db-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db5db-110">Permission type</span></span>|<span data-ttu-id="db5db-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="db5db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db5db-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db5db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db5db-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db5db-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db5db-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db5db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db5db-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db5db-115">Not supported.</span></span>|
|<span data-ttu-id="db5db-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db5db-116">Application</span></span>|<span data-ttu-id="db5db-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db5db-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db5db-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db5db-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/userStates
```

## <a name="request-headers"></a><span data-ttu-id="db5db-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db5db-119">Request headers</span></span>
|<span data-ttu-id="db5db-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="db5db-120">Header</span></span>|<span data-ttu-id="db5db-121">Значение</span><span class="sxs-lookup"><span data-stu-id="db5db-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db5db-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db5db-122">Authorization</span></span>|<span data-ttu-id="db5db-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db5db-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db5db-124">Accept</span><span class="sxs-lookup"><span data-stu-id="db5db-124">Accept</span></span>|<span data-ttu-id="db5db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db5db-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db5db-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db5db-126">Request body</span></span>
<span data-ttu-id="db5db-127">В тексте запроса добавьте представление объекта Девицеманажементинтентусерстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db5db-127">In the request body, supply a JSON representation for the deviceManagementIntentUserState object.</span></span>

<span data-ttu-id="db5db-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтентусерстате.</span><span class="sxs-lookup"><span data-stu-id="db5db-128">The following table shows the properties that are required when you create the deviceManagementIntentUserState.</span></span>

|<span data-ttu-id="db5db-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="db5db-129">Property</span></span>|<span data-ttu-id="db5db-130">Тип</span><span class="sxs-lookup"><span data-stu-id="db5db-130">Type</span></span>|<span data-ttu-id="db5db-131">Описание</span><span class="sxs-lookup"><span data-stu-id="db5db-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db5db-132">id</span><span class="sxs-lookup"><span data-stu-id="db5db-132">id</span></span>|<span data-ttu-id="db5db-133">Строка</span><span class="sxs-lookup"><span data-stu-id="db5db-133">String</span></span>|<span data-ttu-id="db5db-134">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="db5db-134">The ID</span></span>|
|<span data-ttu-id="db5db-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="db5db-135">userPrincipalName</span></span>|<span data-ttu-id="db5db-136">String</span><span class="sxs-lookup"><span data-stu-id="db5db-136">String</span></span>|<span data-ttu-id="db5db-137">Имя участника-пользователя, сообщаемое на устройстве</span><span class="sxs-lookup"><span data-stu-id="db5db-137">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="db5db-138">userName</span><span class="sxs-lookup"><span data-stu-id="db5db-138">userName</span></span>|<span data-ttu-id="db5db-139">String</span><span class="sxs-lookup"><span data-stu-id="db5db-139">String</span></span>|<span data-ttu-id="db5db-140">Имя пользователя, сообщаемое на устройстве</span><span class="sxs-lookup"><span data-stu-id="db5db-140">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="db5db-141">deviceCount</span><span class="sxs-lookup"><span data-stu-id="db5db-141">deviceCount</span></span>|<span data-ttu-id="db5db-142">Int32</span><span class="sxs-lookup"><span data-stu-id="db5db-142">Int32</span></span>|<span data-ttu-id="db5db-143">Количество устройств, принадлежащие пользователю для намерения</span><span class="sxs-lookup"><span data-stu-id="db5db-143">Count of Devices that belongs to a user for an intent</span></span>|
|<span data-ttu-id="db5db-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="db5db-144">lastReportedDateTime</span></span>|<span data-ttu-id="db5db-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db5db-145">DateTimeOffset</span></span>|<span data-ttu-id="db5db-146">Дата и время последнего изменения отчета о намерениях</span><span class="sxs-lookup"><span data-stu-id="db5db-146">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="db5db-147">state</span><span class="sxs-lookup"><span data-stu-id="db5db-147">state</span></span>|[<span data-ttu-id="db5db-148">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="db5db-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="db5db-149">Состояние пользователя для намерения.</span><span class="sxs-lookup"><span data-stu-id="db5db-149">User state for an intent.</span></span> <span data-ttu-id="db5db-150">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="db5db-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|



## <a name="response"></a><span data-ttu-id="db5db-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="db5db-151">Response</span></span>
<span data-ttu-id="db5db-152">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтентусерстате](../resources/intune-deviceintent-devicemanagementintentuserstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="db5db-152">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db5db-153">Пример</span><span class="sxs-lookup"><span data-stu-id="db5db-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="db5db-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="db5db-154">Request</span></span>
<span data-ttu-id="db5db-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db5db-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="db5db-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="db5db-156">Response</span></span>
<span data-ttu-id="db5db-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db5db-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







