---
title: Обновление объекта deviceComplianceUserStatus
description: Обновление свойств объекта deviceComplianceUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 20ab0b844fdf5066301c36bc2b21b09ab783573d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929853"
---
# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="eda92-103">Обновление объекта deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="eda92-103">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="eda92-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eda92-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eda92-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eda92-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eda92-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="eda92-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eda92-107">Обновление свойств объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="eda92-107">Update the properties of a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eda92-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="eda92-108">Prerequisites</span></span>
<span data-ttu-id="eda92-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eda92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eda92-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eda92-111">Permission type</span></span>|<span data-ttu-id="eda92-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eda92-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eda92-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eda92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eda92-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eda92-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eda92-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eda92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eda92-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eda92-116">Not supported.</span></span>|
|<span data-ttu-id="eda92-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eda92-117">Application</span></span>|<span data-ttu-id="eda92-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eda92-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eda92-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eda92-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="eda92-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eda92-120">Request headers</span></span>
|<span data-ttu-id="eda92-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eda92-121">Header</span></span>|<span data-ttu-id="eda92-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eda92-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eda92-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eda92-123">Authorization</span></span>|<span data-ttu-id="eda92-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="eda92-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eda92-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eda92-125">Accept</span></span>|<span data-ttu-id="eda92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eda92-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eda92-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eda92-127">Request body</span></span>
<span data-ttu-id="eda92-128">В тексте запроса добавьте представление объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eda92-128">In the request body, supply a JSON representation for the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="eda92-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="eda92-129">The following table shows the properties that are required when you create the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

|<span data-ttu-id="eda92-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="eda92-130">Property</span></span>|<span data-ttu-id="eda92-131">Тип</span><span class="sxs-lookup"><span data-stu-id="eda92-131">Type</span></span>|<span data-ttu-id="eda92-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eda92-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eda92-133">id</span><span class="sxs-lookup"><span data-stu-id="eda92-133">id</span></span>|<span data-ttu-id="eda92-134">String</span><span class="sxs-lookup"><span data-stu-id="eda92-134">String</span></span>|<span data-ttu-id="eda92-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eda92-135">Key of the entity.</span></span>|
|<span data-ttu-id="eda92-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="eda92-136">userDisplayName</span></span>|<span data-ttu-id="eda92-137">String</span><span class="sxs-lookup"><span data-stu-id="eda92-137">String</span></span>|<span data-ttu-id="eda92-138">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="eda92-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="eda92-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="eda92-139">devicesCount</span></span>|<span data-ttu-id="eda92-140">Int32</span><span class="sxs-lookup"><span data-stu-id="eda92-140">Int32</span></span>|<span data-ttu-id="eda92-141">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="eda92-141">Devices count for that user.</span></span>|
|<span data-ttu-id="eda92-142">status</span><span class="sxs-lookup"><span data-stu-id="eda92-142">status</span></span>|[<span data-ttu-id="eda92-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="eda92-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="eda92-144">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="eda92-144">Compliance status of the policy report.</span></span> <span data-ttu-id="eda92-145">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="eda92-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="eda92-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="eda92-146">lastReportedDateTime</span></span>|<span data-ttu-id="eda92-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eda92-147">DateTimeOffset</span></span>|<span data-ttu-id="eda92-148">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="eda92-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="eda92-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eda92-149">userPrincipalName</span></span>|<span data-ttu-id="eda92-150">String</span><span class="sxs-lookup"><span data-stu-id="eda92-150">String</span></span>|<span data-ttu-id="eda92-151">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="eda92-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="eda92-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="eda92-152">Response</span></span>
<span data-ttu-id="eda92-153">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eda92-153">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eda92-154">Пример</span><span class="sxs-lookup"><span data-stu-id="eda92-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="eda92-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="eda92-155">Request</span></span>
<span data-ttu-id="eda92-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eda92-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
Content-type: application/json
Content-length: 222

{
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="eda92-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="eda92-157">Response</span></span>
<span data-ttu-id="eda92-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="eda92-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





