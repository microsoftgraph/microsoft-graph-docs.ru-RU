---
title: Обновление объекта deviceComplianceUserStatus
description: Обновление свойств объекта deviceComplianceUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9604061eabefefb94e693917b480abc15b8ffc89
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259901"
---
# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="91aba-103">Обновление объекта deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="91aba-103">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="91aba-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91aba-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91aba-105">Обновление свойств объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="91aba-105">Update the properties of a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91aba-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="91aba-106">Prerequisites</span></span>
<span data-ttu-id="91aba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="91aba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="91aba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91aba-109">Permission type</span></span>|<span data-ttu-id="91aba-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="91aba-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91aba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91aba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="91aba-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91aba-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="91aba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91aba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91aba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91aba-114">Not supported.</span></span>|
|<span data-ttu-id="91aba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91aba-115">Application</span></span>|<span data-ttu-id="91aba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91aba-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91aba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91aba-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="91aba-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91aba-118">Request headers</span></span>
|<span data-ttu-id="91aba-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91aba-119">Header</span></span>|<span data-ttu-id="91aba-120">Значение</span><span class="sxs-lookup"><span data-stu-id="91aba-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91aba-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="91aba-121">Authorization</span></span>|<span data-ttu-id="91aba-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="91aba-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91aba-123">Accept</span><span class="sxs-lookup"><span data-stu-id="91aba-123">Accept</span></span>|<span data-ttu-id="91aba-124">application/json</span><span class="sxs-lookup"><span data-stu-id="91aba-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91aba-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91aba-125">Request body</span></span>
<span data-ttu-id="91aba-126">В тексте запроса добавьте представление объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91aba-126">In the request body, supply a JSON representation for the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="91aba-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="91aba-127">The following table shows the properties that are required when you create the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

|<span data-ttu-id="91aba-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="91aba-128">Property</span></span>|<span data-ttu-id="91aba-129">Тип</span><span class="sxs-lookup"><span data-stu-id="91aba-129">Type</span></span>|<span data-ttu-id="91aba-130">Описание</span><span class="sxs-lookup"><span data-stu-id="91aba-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91aba-131">id</span><span class="sxs-lookup"><span data-stu-id="91aba-131">id</span></span>|<span data-ttu-id="91aba-132">Строка</span><span class="sxs-lookup"><span data-stu-id="91aba-132">String</span></span>|<span data-ttu-id="91aba-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="91aba-133">Key of the entity.</span></span>|
|<span data-ttu-id="91aba-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="91aba-134">userDisplayName</span></span>|<span data-ttu-id="91aba-135">String</span><span class="sxs-lookup"><span data-stu-id="91aba-135">String</span></span>|<span data-ttu-id="91aba-136">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="91aba-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="91aba-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="91aba-137">devicesCount</span></span>|<span data-ttu-id="91aba-138">Int32</span><span class="sxs-lookup"><span data-stu-id="91aba-138">Int32</span></span>|<span data-ttu-id="91aba-139">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="91aba-139">Devices count for that user.</span></span>|
|<span data-ttu-id="91aba-140">status</span><span class="sxs-lookup"><span data-stu-id="91aba-140">status</span></span>|[<span data-ttu-id="91aba-141">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="91aba-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="91aba-142">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="91aba-142">Compliance status of the policy report.</span></span> <span data-ttu-id="91aba-143">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="91aba-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="91aba-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="91aba-144">lastReportedDateTime</span></span>|<span data-ttu-id="91aba-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91aba-145">DateTimeOffset</span></span>|<span data-ttu-id="91aba-146">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="91aba-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="91aba-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="91aba-147">userPrincipalName</span></span>|<span data-ttu-id="91aba-148">String</span><span class="sxs-lookup"><span data-stu-id="91aba-148">String</span></span>|<span data-ttu-id="91aba-149">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="91aba-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="91aba-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="91aba-150">Response</span></span>
<span data-ttu-id="91aba-151">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="91aba-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91aba-152">Пример</span><span class="sxs-lookup"><span data-stu-id="91aba-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="91aba-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="91aba-153">Request</span></span>
<span data-ttu-id="91aba-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91aba-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
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

### <a name="response"></a><span data-ttu-id="91aba-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="91aba-155">Response</span></span>
<span data-ttu-id="91aba-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="91aba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



