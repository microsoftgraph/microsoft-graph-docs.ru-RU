---
title: Создание Девицекомплианцескрипт
description: Создание нового объекта Девицекомплианцескрипт.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bbd57133d102a6c0e8d7e28e275388cb13ecbee8
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792508"
---
# <a name="create-devicecompliancescript"></a><span data-ttu-id="d719a-103">Создание Девицекомплианцескрипт</span><span class="sxs-lookup"><span data-stu-id="d719a-103">Create deviceComplianceScript</span></span>

<span data-ttu-id="d719a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d719a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d719a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d719a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d719a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d719a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d719a-107">Создание нового объекта [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md) .</span><span class="sxs-lookup"><span data-stu-id="d719a-107">Create a new [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d719a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d719a-108">Prerequisites</span></span>
<span data-ttu-id="d719a-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d719a-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d719a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d719a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d719a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d719a-111">Permission type</span></span>|<span data-ttu-id="d719a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d719a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d719a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d719a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d719a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d719a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d719a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d719a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d719a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d719a-116">Not supported.</span></span>|
|<span data-ttu-id="d719a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d719a-117">Application</span></span>|<span data-ttu-id="d719a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d719a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d719a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d719a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceComplianceScripts
```

## <a name="request-headers"></a><span data-ttu-id="d719a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d719a-120">Request headers</span></span>
|<span data-ttu-id="d719a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d719a-121">Header</span></span>|<span data-ttu-id="d719a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d719a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d719a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d719a-123">Authorization</span></span>|<span data-ttu-id="d719a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d719a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d719a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d719a-125">Accept</span></span>|<span data-ttu-id="d719a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d719a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d719a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d719a-127">Request body</span></span>
<span data-ttu-id="d719a-128">В тексте запроса добавьте представление объекта Девицекомплианцескрипт в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d719a-128">In the request body, supply a JSON representation for the deviceComplianceScript object.</span></span>

<span data-ttu-id="d719a-129">В следующей таблице приведены свойства, необходимые при создании Девицекомплианцескрипт.</span><span class="sxs-lookup"><span data-stu-id="d719a-129">The following table shows the properties that are required when you create the deviceComplianceScript.</span></span>

|<span data-ttu-id="d719a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d719a-130">Property</span></span>|<span data-ttu-id="d719a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d719a-131">Type</span></span>|<span data-ttu-id="d719a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d719a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d719a-133">id</span><span class="sxs-lookup"><span data-stu-id="d719a-133">id</span></span>|<span data-ttu-id="d719a-134">String</span><span class="sxs-lookup"><span data-stu-id="d719a-134">String</span></span>|<span data-ttu-id="d719a-135">Уникальный идентификатор для сценария соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="d719a-135">Unique Identifier for the device compliance script</span></span>|
|<span data-ttu-id="d719a-136">publisher</span><span class="sxs-lookup"><span data-stu-id="d719a-136">publisher</span></span>|<span data-ttu-id="d719a-137">String</span><span class="sxs-lookup"><span data-stu-id="d719a-137">String</span></span>|<span data-ttu-id="d719a-138">Имя издателя сценариев соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="d719a-138">Name of the device compliance script publisher</span></span>|
|<span data-ttu-id="d719a-139">version</span><span class="sxs-lookup"><span data-stu-id="d719a-139">version</span></span>|<span data-ttu-id="d719a-140">String</span><span class="sxs-lookup"><span data-stu-id="d719a-140">String</span></span>|<span data-ttu-id="d719a-141">Версия сценария соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="d719a-141">Version of the device compliance script</span></span>|
|<span data-ttu-id="d719a-142">displayName</span><span class="sxs-lookup"><span data-stu-id="d719a-142">displayName</span></span>|<span data-ttu-id="d719a-143">Строка</span><span class="sxs-lookup"><span data-stu-id="d719a-143">String</span></span>|<span data-ttu-id="d719a-144">Имя сценария соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="d719a-144">Name of the device compliance script</span></span>|
|<span data-ttu-id="d719a-145">description</span><span class="sxs-lookup"><span data-stu-id="d719a-145">description</span></span>|<span data-ttu-id="d719a-146">String</span><span class="sxs-lookup"><span data-stu-id="d719a-146">String</span></span>|<span data-ttu-id="d719a-147">Описание сценария соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="d719a-147">Description of the device compliance script</span></span>|
|<span data-ttu-id="d719a-148">детектионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="d719a-148">detectionScriptContent</span></span>|<span data-ttu-id="d719a-149">Binary</span><span class="sxs-lookup"><span data-stu-id="d719a-149">Binary</span></span>|<span data-ttu-id="d719a-150">Весь контент скрипта обнаружения PowerShell</span><span class="sxs-lookup"><span data-stu-id="d719a-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="d719a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d719a-151">createdDateTime</span></span>|<span data-ttu-id="d719a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d719a-152">DateTimeOffset</span></span>|<span data-ttu-id="d719a-153">Метка времени создания сценария соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="d719a-153">The timestamp of when the device compliance script was created.</span></span> <span data-ttu-id="d719a-154">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d719a-154">This property is read-only.</span></span>|
|<span data-ttu-id="d719a-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d719a-155">lastModifiedDateTime</span></span>|<span data-ttu-id="d719a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d719a-156">DateTimeOffset</span></span>|<span data-ttu-id="d719a-157">Метка времени изменения сценария соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="d719a-157">The timestamp of when the device compliance script was modified.</span></span> <span data-ttu-id="d719a-158">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d719a-158">This property is read-only.</span></span>|
|<span data-ttu-id="d719a-159">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="d719a-159">runAsAccount</span></span>|[<span data-ttu-id="d719a-160">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="d719a-160">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="d719a-161">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="d719a-161">Indicates the type of execution context.</span></span> <span data-ttu-id="d719a-162">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="d719a-162">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="d719a-163">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="d719a-163">enforceSignatureCheck</span></span>|<span data-ttu-id="d719a-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="d719a-164">Boolean</span></span>|<span data-ttu-id="d719a-165">Указывает, нужно ли проверять подпись скрипта</span><span class="sxs-lookup"><span data-stu-id="d719a-165">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="d719a-166">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="d719a-166">runAs32Bit</span></span>|<span data-ttu-id="d719a-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="d719a-167">Boolean</span></span>|<span data-ttu-id="d719a-168">Указывает, следует ли выполнять скрипты PowerShell как 32-разрядные</span><span class="sxs-lookup"><span data-stu-id="d719a-168">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="d719a-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d719a-169">roleScopeTagIds</span></span>|<span data-ttu-id="d719a-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d719a-170">String collection</span></span>|<span data-ttu-id="d719a-171">Список идентификаторов тегов области для сценария соответствия требованиям устройств</span><span class="sxs-lookup"><span data-stu-id="d719a-171">List of Scope Tag IDs for the device compliance script</span></span>|



## <a name="response"></a><span data-ttu-id="d719a-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="d719a-172">Response</span></span>
<span data-ttu-id="d719a-173">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d719a-173">If successful, this method returns a `201 Created` response code and a [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d719a-174">Пример</span><span class="sxs-lookup"><span data-stu-id="d719a-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="d719a-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="d719a-175">Request</span></span>
<span data-ttu-id="d719a-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d719a-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts
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

### <a name="response"></a><span data-ttu-id="d719a-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="d719a-177">Response</span></span>
<span data-ttu-id="d719a-178">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="d719a-178">Here is an example of the response.</span></span> <span data-ttu-id="d719a-179">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="d719a-179">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d719a-180">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="d719a-180">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



