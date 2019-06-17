---
title: Создание объекта deviceComplianceUserStatus
description: Создание объекта deviceComplianceUserStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f51a534f620252b8fd8536d828ea8a82e79b89db
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968086"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="53fd7-103">Создание объекта deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="53fd7-103">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="53fd7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53fd7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53fd7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53fd7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53fd7-106">Создание объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="53fd7-106">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53fd7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="53fd7-107">Prerequisites</span></span>
<span data-ttu-id="53fd7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53fd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53fd7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53fd7-110">Permission type</span></span>|<span data-ttu-id="53fd7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53fd7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53fd7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53fd7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53fd7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53fd7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="53fd7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53fd7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53fd7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53fd7-115">Not supported.</span></span>|
|<span data-ttu-id="53fd7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53fd7-116">Application</span></span>|<span data-ttu-id="53fd7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53fd7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53fd7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53fd7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="53fd7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53fd7-119">Request headers</span></span>
|<span data-ttu-id="53fd7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53fd7-120">Header</span></span>|<span data-ttu-id="53fd7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="53fd7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53fd7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53fd7-122">Authorization</span></span>|<span data-ttu-id="53fd7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53fd7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53fd7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="53fd7-124">Accept</span></span>|<span data-ttu-id="53fd7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53fd7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53fd7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="53fd7-126">Request body</span></span>
<span data-ttu-id="53fd7-127">В тексте запроса добавьте представление объекта deviceComplianceUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53fd7-127">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="53fd7-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="53fd7-128">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="53fd7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="53fd7-129">Property</span></span>|<span data-ttu-id="53fd7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="53fd7-130">Type</span></span>|<span data-ttu-id="53fd7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="53fd7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53fd7-132">id</span><span class="sxs-lookup"><span data-stu-id="53fd7-132">id</span></span>|<span data-ttu-id="53fd7-133">Строка</span><span class="sxs-lookup"><span data-stu-id="53fd7-133">String</span></span>|<span data-ttu-id="53fd7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="53fd7-134">Key of the entity.</span></span>|
|<span data-ttu-id="53fd7-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="53fd7-135">userDisplayName</span></span>|<span data-ttu-id="53fd7-136">String</span><span class="sxs-lookup"><span data-stu-id="53fd7-136">String</span></span>|<span data-ttu-id="53fd7-137">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="53fd7-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="53fd7-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="53fd7-138">devicesCount</span></span>|<span data-ttu-id="53fd7-139">Int32</span><span class="sxs-lookup"><span data-stu-id="53fd7-139">Int32</span></span>|<span data-ttu-id="53fd7-140">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="53fd7-140">Devices count for that user.</span></span>|
|<span data-ttu-id="53fd7-141">status</span><span class="sxs-lookup"><span data-stu-id="53fd7-141">status</span></span>|[<span data-ttu-id="53fd7-142">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="53fd7-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="53fd7-143">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="53fd7-143">Compliance status of the policy report.</span></span> <span data-ttu-id="53fd7-144">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="53fd7-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="53fd7-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="53fd7-145">lastReportedDateTime</span></span>|<span data-ttu-id="53fd7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53fd7-146">DateTimeOffset</span></span>|<span data-ttu-id="53fd7-147">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="53fd7-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="53fd7-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="53fd7-148">userPrincipalName</span></span>|<span data-ttu-id="53fd7-149">String</span><span class="sxs-lookup"><span data-stu-id="53fd7-149">String</span></span>|<span data-ttu-id="53fd7-150">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="53fd7-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="53fd7-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="53fd7-151">Response</span></span>
<span data-ttu-id="53fd7-152">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53fd7-152">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53fd7-153">Пример</span><span class="sxs-lookup"><span data-stu-id="53fd7-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="53fd7-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="53fd7-154">Request</span></span>
<span data-ttu-id="53fd7-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53fd7-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
Content-type: application/json
Content-length: 287

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="53fd7-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="53fd7-156">Response</span></span>
<span data-ttu-id="53fd7-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53fd7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 336

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```





