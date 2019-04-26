---
title: Создание объекта deviceConfigurationUserStatus
description: Создание объекта deviceConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 280e961cc25aa4eba2a739544055975013b88c51
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565851"
---
# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="64219-103">Создание объекта deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="64219-103">Create deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="64219-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64219-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64219-105">Создание объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="64219-105">Create a new [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64219-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="64219-106">Prerequisites</span></span>
<span data-ttu-id="64219-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64219-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64219-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64219-109">Permission type</span></span>|<span data-ttu-id="64219-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64219-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64219-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64219-111">Delegated (work or school account)</span></span>|<span data-ttu-id="64219-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64219-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64219-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64219-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64219-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64219-114">Not supported.</span></span>|
|<span data-ttu-id="64219-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64219-115">Application</span></span>|<span data-ttu-id="64219-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64219-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64219-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64219-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="64219-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64219-118">Request headers</span></span>
|<span data-ttu-id="64219-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64219-119">Header</span></span>|<span data-ttu-id="64219-120">Значение</span><span class="sxs-lookup"><span data-stu-id="64219-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64219-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64219-121">Authorization</span></span>|<span data-ttu-id="64219-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64219-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64219-123">Accept</span><span class="sxs-lookup"><span data-stu-id="64219-123">Accept</span></span>|<span data-ttu-id="64219-124">application/json</span><span class="sxs-lookup"><span data-stu-id="64219-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64219-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64219-125">Request body</span></span>
<span data-ttu-id="64219-126">В тексте запроса добавьте представление объекта deviceConfigurationUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64219-126">In the request body, supply a JSON representation for the deviceConfigurationUserStatus object.</span></span>

<span data-ttu-id="64219-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="64219-127">The following table shows the properties that are required when you create the deviceConfigurationUserStatus.</span></span>

|<span data-ttu-id="64219-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="64219-128">Property</span></span>|<span data-ttu-id="64219-129">Тип</span><span class="sxs-lookup"><span data-stu-id="64219-129">Type</span></span>|<span data-ttu-id="64219-130">Описание</span><span class="sxs-lookup"><span data-stu-id="64219-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64219-131">id</span><span class="sxs-lookup"><span data-stu-id="64219-131">id</span></span>|<span data-ttu-id="64219-132">Строка</span><span class="sxs-lookup"><span data-stu-id="64219-132">String</span></span>|<span data-ttu-id="64219-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="64219-133">Key of the entity.</span></span>|
|<span data-ttu-id="64219-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="64219-134">userDisplayName</span></span>|<span data-ttu-id="64219-135">String</span><span class="sxs-lookup"><span data-stu-id="64219-135">String</span></span>|<span data-ttu-id="64219-136">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="64219-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="64219-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="64219-137">devicesCount</span></span>|<span data-ttu-id="64219-138">Int32</span><span class="sxs-lookup"><span data-stu-id="64219-138">Int32</span></span>|<span data-ttu-id="64219-139">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="64219-139">Devices count for that user.</span></span>|
|<span data-ttu-id="64219-140">status</span><span class="sxs-lookup"><span data-stu-id="64219-140">status</span></span>|[<span data-ttu-id="64219-141">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="64219-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="64219-142">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="64219-142">Compliance status of the policy report.</span></span> <span data-ttu-id="64219-143">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="64219-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="64219-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="64219-144">lastReportedDateTime</span></span>|<span data-ttu-id="64219-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64219-145">DateTimeOffset</span></span>|<span data-ttu-id="64219-146">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="64219-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="64219-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="64219-147">userPrincipalName</span></span>|<span data-ttu-id="64219-148">String</span><span class="sxs-lookup"><span data-stu-id="64219-148">String</span></span>|<span data-ttu-id="64219-149">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="64219-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="64219-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="64219-150">Response</span></span>
<span data-ttu-id="64219-151">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64219-151">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64219-152">Пример</span><span class="sxs-lookup"><span data-stu-id="64219-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="64219-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="64219-153">Request</span></span>
<span data-ttu-id="64219-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64219-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="64219-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="64219-155">Response</span></span>
<span data-ttu-id="64219-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64219-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



