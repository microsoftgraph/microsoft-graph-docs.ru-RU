---
title: Создание remoteActionAudit
description: Создание нового объекта remoteActionAudit.
ms.openlocfilehash: f39f1b289a081d89135fd7be230e2aecba6823c8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079603"
---
# <a name="create-remoteactionaudit"></a><span data-ttu-id="106dc-103">Создание remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="106dc-103">Create remoteActionAudit</span></span>

> <span data-ttu-id="106dc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="106dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="106dc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="106dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="106dc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="106dc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="106dc-107">Создание нового объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="106dc-107">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="106dc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="106dc-108">Prerequisites</span></span>
<span data-ttu-id="106dc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="106dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="106dc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="106dc-111">Permission type</span></span>|<span data-ttu-id="106dc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="106dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="106dc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="106dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="106dc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="106dc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="106dc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="106dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="106dc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="106dc-116">Not supported.</span></span>|
|<span data-ttu-id="106dc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="106dc-117">Application</span></span>|<span data-ttu-id="106dc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="106dc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="106dc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="106dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="106dc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="106dc-120">Request headers</span></span>
|<span data-ttu-id="106dc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="106dc-121">Header</span></span>|<span data-ttu-id="106dc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="106dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="106dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="106dc-123">Authorization</span></span>|<span data-ttu-id="106dc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="106dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="106dc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="106dc-125">Accept</span></span>|<span data-ttu-id="106dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="106dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="106dc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="106dc-127">Request body</span></span>
<span data-ttu-id="106dc-128">В тексте запроса укажите представление JSON для объекта remoteActionAudit.</span><span class="sxs-lookup"><span data-stu-id="106dc-128">In the request body, supply a JSON representation for the remoteActionAudit object.</span></span>

<span data-ttu-id="106dc-129">В следующей таблице показаны свойства, которые необходимы для создания remoteActionAudit.</span><span class="sxs-lookup"><span data-stu-id="106dc-129">The following table shows the properties that are required when you create the remoteActionAudit.</span></span>

|<span data-ttu-id="106dc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="106dc-130">Property</span></span>|<span data-ttu-id="106dc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="106dc-131">Type</span></span>|<span data-ttu-id="106dc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="106dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="106dc-133">id</span><span class="sxs-lookup"><span data-stu-id="106dc-133">id</span></span>|<span data-ttu-id="106dc-134">String</span><span class="sxs-lookup"><span data-stu-id="106dc-134">String</span></span>|<span data-ttu-id="106dc-135">Идентификатор отчета.</span><span class="sxs-lookup"><span data-stu-id="106dc-135">Report Id.</span></span>|
|<span data-ttu-id="106dc-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="106dc-136">deviceDisplayName</span></span>|<span data-ttu-id="106dc-137">String</span><span class="sxs-lookup"><span data-stu-id="106dc-137">String</span></span>|<span data-ttu-id="106dc-138">Имя устройства Intune.</span><span class="sxs-lookup"><span data-stu-id="106dc-138">Intune device name.</span></span>|
|<span data-ttu-id="106dc-139">userName</span><span class="sxs-lookup"><span data-stu-id="106dc-139">userName</span></span>|<span data-ttu-id="106dc-140">String</span><span class="sxs-lookup"><span data-stu-id="106dc-140">String</span></span>|<span data-ttu-id="106dc-141">\[устаревшие\] вместо этого используйте InitiatedByUserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="106dc-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="106dc-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="106dc-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="106dc-143">String</span><span class="sxs-lookup"><span data-stu-id="106dc-143">String</span></span>|<span data-ttu-id="106dc-144">Пользователя, который инициировал действие устройства имеет формат имени участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="106dc-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="106dc-145">action</span><span class="sxs-lookup"><span data-stu-id="106dc-145">action</span></span>|[<span data-ttu-id="106dc-146">remoteAction</span><span class="sxs-lookup"><span data-stu-id="106dc-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="106dc-147">Имя действия.</span><span class="sxs-lookup"><span data-stu-id="106dc-147">The action name.</span></span> <span data-ttu-id="106dc-148">Возможные значения: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` .</span><span class="sxs-lookup"><span data-stu-id="106dc-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="106dc-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="106dc-149">requestDateTime</span></span>|<span data-ttu-id="106dc-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="106dc-150">DateTimeOffset</span></span>|<span data-ttu-id="106dc-151">Время, когда действие был отправлен, в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="106dc-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="106dc-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="106dc-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="106dc-153">String</span><span class="sxs-lookup"><span data-stu-id="106dc-153">String</span></span>|<span data-ttu-id="106dc-154">Имя участника-пользователя владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="106dc-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="106dc-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="106dc-155">deviceIMEI</span></span>|<span data-ttu-id="106dc-156">String</span><span class="sxs-lookup"><span data-stu-id="106dc-156">String</span></span>|<span data-ttu-id="106dc-157">IMEI устройства.</span><span class="sxs-lookup"><span data-stu-id="106dc-157">IMEI of the device.</span></span>|
|<span data-ttu-id="106dc-158">actionState</span><span class="sxs-lookup"><span data-stu-id="106dc-158">actionState</span></span>|[<span data-ttu-id="106dc-159">actionState</span><span class="sxs-lookup"><span data-stu-id="106dc-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="106dc-160">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="106dc-160">Action state.</span></span> <span data-ttu-id="106dc-161">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="106dc-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|



## <a name="response"></a><span data-ttu-id="106dc-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="106dc-162">Response</span></span>
<span data-ttu-id="106dc-163">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="106dc-163">If successful, this method returns a `201 Created` response code and a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="106dc-164">Пример</span><span class="sxs-lookup"><span data-stu-id="106dc-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="106dc-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="106dc-165">Request</span></span>
<span data-ttu-id="106dc-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="106dc-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending"
}
```

### <a name="response"></a><span data-ttu-id="106dc-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="106dc-167">Response</span></span>
<span data-ttu-id="106dc-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="106dc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending"
}
```





