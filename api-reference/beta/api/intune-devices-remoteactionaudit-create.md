---
title: Создание remoteActionAudit
description: Создание нового объекта remoteActionAudit.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1686005b04e0e9fbf8376f7e14455937feff65af
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167433"
---
# <a name="create-remoteactionaudit"></a><span data-ttu-id="0b26a-103">Создание remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="0b26a-103">Create remoteActionAudit</span></span>

> <span data-ttu-id="0b26a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b26a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b26a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b26a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b26a-106">Создание нового объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="0b26a-106">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b26a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0b26a-107">Prerequisites</span></span>
<span data-ttu-id="0b26a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0b26a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0b26a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b26a-110">Permission type</span></span>|<span data-ttu-id="0b26a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b26a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b26a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b26a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b26a-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b26a-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0b26a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b26a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b26a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b26a-115">Not supported.</span></span>|
|<span data-ttu-id="0b26a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b26a-116">Application</span></span>|<span data-ttu-id="0b26a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b26a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b26a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b26a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="0b26a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b26a-119">Request headers</span></span>
|<span data-ttu-id="0b26a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b26a-120">Header</span></span>|<span data-ttu-id="0b26a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0b26a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b26a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b26a-122">Authorization</span></span>|<span data-ttu-id="0b26a-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0b26a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b26a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0b26a-124">Accept</span></span>|<span data-ttu-id="0b26a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b26a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b26a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b26a-126">Request body</span></span>
<span data-ttu-id="0b26a-127">В тексте запроса добавьте представление объекта remoteActionAudit в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b26a-127">In the request body, supply a JSON representation for the remoteActionAudit object.</span></span>

<span data-ttu-id="0b26a-128">В следующей таблице приведены свойства, необходимые при создании remoteActionAudit.</span><span class="sxs-lookup"><span data-stu-id="0b26a-128">The following table shows the properties that are required when you create the remoteActionAudit.</span></span>

|<span data-ttu-id="0b26a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b26a-129">Property</span></span>|<span data-ttu-id="0b26a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0b26a-130">Type</span></span>|<span data-ttu-id="0b26a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0b26a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b26a-132">id</span><span class="sxs-lookup"><span data-stu-id="0b26a-132">id</span></span>|<span data-ttu-id="0b26a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="0b26a-133">String</span></span>|<span data-ttu-id="0b26a-134">Идентификатор отчета.</span><span class="sxs-lookup"><span data-stu-id="0b26a-134">Report Id.</span></span>|
|<span data-ttu-id="0b26a-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="0b26a-135">deviceDisplayName</span></span>|<span data-ttu-id="0b26a-136">String</span><span class="sxs-lookup"><span data-stu-id="0b26a-136">String</span></span>|<span data-ttu-id="0b26a-137">Имя устройства Intune.</span><span class="sxs-lookup"><span data-stu-id="0b26a-137">Intune device name.</span></span>|
|<span data-ttu-id="0b26a-138">userName</span><span class="sxs-lookup"><span data-stu-id="0b26a-138">userName</span></span>|<span data-ttu-id="0b26a-139">String</span><span class="sxs-lookup"><span data-stu-id="0b26a-139">String</span></span>|<span data-ttu-id="0b26a-140">\[\] рекомендуется вместо этого использовать свойства initiatedbyuserprincipalname.</span><span class="sxs-lookup"><span data-stu-id="0b26a-140">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="0b26a-141">Свойства initiatedbyuserprincipalname</span><span class="sxs-lookup"><span data-stu-id="0b26a-141">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="0b26a-142">String</span><span class="sxs-lookup"><span data-stu-id="0b26a-142">String</span></span>|<span data-ttu-id="0b26a-143">Пользователь, который инициировал действие с устройством, имеет формат UPN.</span><span class="sxs-lookup"><span data-stu-id="0b26a-143">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="0b26a-144">action</span><span class="sxs-lookup"><span data-stu-id="0b26a-144">action</span></span>|[<span data-ttu-id="0b26a-145">Ремотеактион</span><span class="sxs-lookup"><span data-stu-id="0b26a-145">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="0b26a-146">Имя действия.</span><span class="sxs-lookup"><span data-stu-id="0b26a-146">The action name.</span></span> <span data-ttu-id="0b26a-147">Возможные значения: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `logoutSharedAppleDeviceActiveUser` `quickScan`,,,,,,,,,,,,,,,,,,,,, `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` .</span><span class="sxs-lookup"><span data-stu-id="0b26a-147">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="0b26a-148">Рекуестдатетиме</span><span class="sxs-lookup"><span data-stu-id="0b26a-148">requestDateTime</span></span>|<span data-ttu-id="0b26a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b26a-149">DateTimeOffset</span></span>|<span data-ttu-id="0b26a-150">Время, когда действие было выдано, заданное в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0b26a-150">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="0b26a-151">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0b26a-151">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="0b26a-152">String</span><span class="sxs-lookup"><span data-stu-id="0b26a-152">String</span></span>|<span data-ttu-id="0b26a-153">Имя участника-пользователя для владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="0b26a-153">Upn of the device owner.</span></span>|
|<span data-ttu-id="0b26a-154">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="0b26a-154">deviceIMEI</span></span>|<span data-ttu-id="0b26a-155">String</span><span class="sxs-lookup"><span data-stu-id="0b26a-155">String</span></span>|<span data-ttu-id="0b26a-156">IMEI устройства.</span><span class="sxs-lookup"><span data-stu-id="0b26a-156">IMEI of the device.</span></span>|
|<span data-ttu-id="0b26a-157">actionState</span><span class="sxs-lookup"><span data-stu-id="0b26a-157">actionState</span></span>|[<span data-ttu-id="0b26a-158">actionState</span><span class="sxs-lookup"><span data-stu-id="0b26a-158">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="0b26a-159">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="0b26a-159">Action state.</span></span> <span data-ttu-id="0b26a-160">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="0b26a-160">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|



## <a name="response"></a><span data-ttu-id="0b26a-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b26a-161">Response</span></span>
<span data-ttu-id="0b26a-162">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0b26a-162">If successful, this method returns a `201 Created` response code and a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b26a-163">Пример</span><span class="sxs-lookup"><span data-stu-id="0b26a-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b26a-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b26a-164">Request</span></span>
<span data-ttu-id="0b26a-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b26a-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0b26a-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="0b26a-166">Response</span></span>
<span data-ttu-id="0b26a-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b26a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




