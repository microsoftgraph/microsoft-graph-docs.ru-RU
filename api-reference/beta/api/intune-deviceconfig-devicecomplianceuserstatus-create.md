---
title: Создание объекта deviceComplianceUserStatus
description: Создание объекта deviceComplianceUserStatus.
ms.openlocfilehash: 03b2b221ba41c2b8812c6cb0d4e6ec9ab711b583
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081608"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="37ee7-103">Создание объекта deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="37ee7-103">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="37ee7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="37ee7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37ee7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37ee7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37ee7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="37ee7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37ee7-107">Создание объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="37ee7-107">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="37ee7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="37ee7-108">Prerequisites</span></span>
<span data-ttu-id="37ee7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37ee7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37ee7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37ee7-111">Permission type</span></span>|<span data-ttu-id="37ee7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="37ee7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37ee7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37ee7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37ee7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37ee7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37ee7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37ee7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37ee7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37ee7-116">Not supported.</span></span>|
|<span data-ttu-id="37ee7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37ee7-117">Application</span></span>|<span data-ttu-id="37ee7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37ee7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37ee7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37ee7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="37ee7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37ee7-120">Request headers</span></span>
|<span data-ttu-id="37ee7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37ee7-121">Header</span></span>|<span data-ttu-id="37ee7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="37ee7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37ee7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37ee7-123">Authorization</span></span>|<span data-ttu-id="37ee7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="37ee7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37ee7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="37ee7-125">Accept</span></span>|<span data-ttu-id="37ee7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37ee7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37ee7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37ee7-127">Request body</span></span>
<span data-ttu-id="37ee7-128">В тексте запроса добавьте представление объекта deviceComplianceUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37ee7-128">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="37ee7-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="37ee7-129">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="37ee7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="37ee7-130">Property</span></span>|<span data-ttu-id="37ee7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="37ee7-131">Type</span></span>|<span data-ttu-id="37ee7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="37ee7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37ee7-133">id</span><span class="sxs-lookup"><span data-stu-id="37ee7-133">id</span></span>|<span data-ttu-id="37ee7-134">String</span><span class="sxs-lookup"><span data-stu-id="37ee7-134">String</span></span>|<span data-ttu-id="37ee7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="37ee7-135">Key of the entity.</span></span>|
|<span data-ttu-id="37ee7-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="37ee7-136">userDisplayName</span></span>|<span data-ttu-id="37ee7-137">String</span><span class="sxs-lookup"><span data-stu-id="37ee7-137">String</span></span>|<span data-ttu-id="37ee7-138">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="37ee7-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="37ee7-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="37ee7-139">devicesCount</span></span>|<span data-ttu-id="37ee7-140">Int32</span><span class="sxs-lookup"><span data-stu-id="37ee7-140">Int32</span></span>|<span data-ttu-id="37ee7-141">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="37ee7-141">Devices count for that user.</span></span>|
|<span data-ttu-id="37ee7-142">status</span><span class="sxs-lookup"><span data-stu-id="37ee7-142">status</span></span>|[<span data-ttu-id="37ee7-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="37ee7-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="37ee7-144">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="37ee7-144">Compliance status of the policy report.</span></span> <span data-ttu-id="37ee7-145">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="37ee7-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="37ee7-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="37ee7-146">lastReportedDateTime</span></span>|<span data-ttu-id="37ee7-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37ee7-147">DateTimeOffset</span></span>|<span data-ttu-id="37ee7-148">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="37ee7-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="37ee7-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="37ee7-149">userPrincipalName</span></span>|<span data-ttu-id="37ee7-150">String</span><span class="sxs-lookup"><span data-stu-id="37ee7-150">String</span></span>|<span data-ttu-id="37ee7-151">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="37ee7-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="37ee7-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="37ee7-152">Response</span></span>
<span data-ttu-id="37ee7-153">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="37ee7-153">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37ee7-154">Пример</span><span class="sxs-lookup"><span data-stu-id="37ee7-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="37ee7-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="37ee7-155">Request</span></span>
<span data-ttu-id="37ee7-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37ee7-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37ee7-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="37ee7-157">Response</span></span>
<span data-ttu-id="37ee7-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="37ee7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





