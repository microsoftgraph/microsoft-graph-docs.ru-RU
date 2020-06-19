---
title: Обновление Девицекомплианцескрипт
description: Обновление свойств объекта Девицекомплианцескрипт.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 88187ad5f3ea66202823c074b85a5336078246df
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792480"
---
# <a name="update-devicecompliancescript"></a><span data-ttu-id="b2aa4-103">Обновление Девицекомплианцескрипт</span><span class="sxs-lookup"><span data-stu-id="b2aa4-103">Update deviceComplianceScript</span></span>

<span data-ttu-id="b2aa4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2aa4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2aa4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2aa4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2aa4-107">Обновление свойств объекта [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md) .</span><span class="sxs-lookup"><span data-stu-id="b2aa4-107">Update the properties of a [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2aa4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b2aa4-108">Prerequisites</span></span>
<span data-ttu-id="b2aa4-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b2aa4-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2aa4-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2aa4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2aa4-111">Permission type</span></span>|<span data-ttu-id="b2aa4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2aa4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2aa4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2aa4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2aa4-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2aa4-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b2aa4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2aa4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2aa4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-116">Not supported.</span></span>|
|<span data-ttu-id="b2aa4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2aa4-117">Application</span></span>|<span data-ttu-id="b2aa4-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2aa4-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2aa4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2aa4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="b2aa4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b2aa4-120">Request headers</span></span>
|<span data-ttu-id="b2aa4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2aa4-121">Header</span></span>|<span data-ttu-id="b2aa4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b2aa4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2aa4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2aa4-123">Authorization</span></span>|<span data-ttu-id="b2aa4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2aa4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b2aa4-125">Accept</span></span>|<span data-ttu-id="b2aa4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2aa4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2aa4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b2aa4-127">Request body</span></span>
<span data-ttu-id="b2aa4-128">В тексте запроса добавьте представление объекта [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-128">In the request body, supply a JSON representation for the [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object.</span></span>

<span data-ttu-id="b2aa4-129">В следующей таблице приведены свойства, необходимые при создании [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md).</span><span class="sxs-lookup"><span data-stu-id="b2aa4-129">The following table shows the properties that are required when you create the [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md).</span></span>

|<span data-ttu-id="b2aa4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2aa4-130">Property</span></span>|<span data-ttu-id="b2aa4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b2aa4-131">Type</span></span>|<span data-ttu-id="b2aa4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b2aa4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2aa4-133">id</span><span class="sxs-lookup"><span data-stu-id="b2aa4-133">id</span></span>|<span data-ttu-id="b2aa4-134">String</span><span class="sxs-lookup"><span data-stu-id="b2aa4-134">String</span></span>|<span data-ttu-id="b2aa4-135">Уникальный идентификатор для сценария соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="b2aa4-135">Unique Identifier for the device compliance script</span></span>|
|<span data-ttu-id="b2aa4-136">publisher</span><span class="sxs-lookup"><span data-stu-id="b2aa4-136">publisher</span></span>|<span data-ttu-id="b2aa4-137">String</span><span class="sxs-lookup"><span data-stu-id="b2aa4-137">String</span></span>|<span data-ttu-id="b2aa4-138">Имя издателя сценариев соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="b2aa4-138">Name of the device compliance script publisher</span></span>|
|<span data-ttu-id="b2aa4-139">version</span><span class="sxs-lookup"><span data-stu-id="b2aa4-139">version</span></span>|<span data-ttu-id="b2aa4-140">String</span><span class="sxs-lookup"><span data-stu-id="b2aa4-140">String</span></span>|<span data-ttu-id="b2aa4-141">Версия сценария соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="b2aa4-141">Version of the device compliance script</span></span>|
|<span data-ttu-id="b2aa4-142">displayName</span><span class="sxs-lookup"><span data-stu-id="b2aa4-142">displayName</span></span>|<span data-ttu-id="b2aa4-143">Строка</span><span class="sxs-lookup"><span data-stu-id="b2aa4-143">String</span></span>|<span data-ttu-id="b2aa4-144">Имя сценария соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="b2aa4-144">Name of the device compliance script</span></span>|
|<span data-ttu-id="b2aa4-145">description</span><span class="sxs-lookup"><span data-stu-id="b2aa4-145">description</span></span>|<span data-ttu-id="b2aa4-146">String</span><span class="sxs-lookup"><span data-stu-id="b2aa4-146">String</span></span>|<span data-ttu-id="b2aa4-147">Описание сценария соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="b2aa4-147">Description of the device compliance script</span></span>|
|<span data-ttu-id="b2aa4-148">детектионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="b2aa4-148">detectionScriptContent</span></span>|<span data-ttu-id="b2aa4-149">Binary</span><span class="sxs-lookup"><span data-stu-id="b2aa4-149">Binary</span></span>|<span data-ttu-id="b2aa4-150">Весь контент скрипта обнаружения PowerShell</span><span class="sxs-lookup"><span data-stu-id="b2aa4-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="b2aa4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2aa4-151">createdDateTime</span></span>|<span data-ttu-id="b2aa4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2aa4-152">DateTimeOffset</span></span>|<span data-ttu-id="b2aa4-153">Метка времени создания сценария соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-153">The timestamp of when the device compliance script was created.</span></span> <span data-ttu-id="b2aa4-154">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-154">This property is read-only.</span></span>|
|<span data-ttu-id="b2aa4-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2aa4-155">lastModifiedDateTime</span></span>|<span data-ttu-id="b2aa4-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2aa4-156">DateTimeOffset</span></span>|<span data-ttu-id="b2aa4-157">Метка времени изменения сценария соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-157">The timestamp of when the device compliance script was modified.</span></span> <span data-ttu-id="b2aa4-158">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-158">This property is read-only.</span></span>|
|<span data-ttu-id="b2aa4-159">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="b2aa4-159">runAsAccount</span></span>|[<span data-ttu-id="b2aa4-160">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="b2aa4-160">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="b2aa4-161">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-161">Indicates the type of execution context.</span></span> <span data-ttu-id="b2aa4-162">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-162">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="b2aa4-163">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="b2aa4-163">enforceSignatureCheck</span></span>|<span data-ttu-id="b2aa4-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2aa4-164">Boolean</span></span>|<span data-ttu-id="b2aa4-165">Указывает, нужно ли проверять подпись скрипта</span><span class="sxs-lookup"><span data-stu-id="b2aa4-165">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="b2aa4-166">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="b2aa4-166">runAs32Bit</span></span>|<span data-ttu-id="b2aa4-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2aa4-167">Boolean</span></span>|<span data-ttu-id="b2aa4-168">Указывает, следует ли выполнять скрипты PowerShell как 32-разрядные</span><span class="sxs-lookup"><span data-stu-id="b2aa4-168">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="b2aa4-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b2aa4-169">roleScopeTagIds</span></span>|<span data-ttu-id="b2aa4-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b2aa4-170">String collection</span></span>|<span data-ttu-id="b2aa4-171">Список идентификаторов тегов области для сценария соответствия требованиям устройств</span><span class="sxs-lookup"><span data-stu-id="b2aa4-171">List of Scope Tag IDs for the device compliance script</span></span>|



## <a name="response"></a><span data-ttu-id="b2aa4-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2aa4-172">Response</span></span>
<span data-ttu-id="b2aa4-173">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-173">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2aa4-174">Пример</span><span class="sxs-lookup"><span data-stu-id="b2aa4-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2aa4-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2aa4-175">Request</span></span>
<span data-ttu-id="b2aa4-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}
Content-type: application/json
Content-length: 420

{
  "@odata.type": "#microsoft.graph.deviceComplianceScript",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b2aa4-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2aa4-177">Response</span></span>
<span data-ttu-id="b2aa4-178">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-178">Here is an example of the response.</span></span> <span data-ttu-id="b2aa4-179">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-179">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b2aa4-180">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b2aa4-180">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 592

{
  "@odata.type": "#microsoft.graph.deviceComplianceScript",
  "id": "14e72a7b-2a7b-14e7-7b2a-e7147b2ae714",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```



