---
title: Создание Девицехеалсскрипт
description: Создание нового объекта Девицехеалсскрипт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 02fe74bf70c5961b510bfd74ba732c81839e575a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945160"
---
# <a name="create-devicehealthscript"></a><span data-ttu-id="59d7c-103">Создание Девицехеалсскрипт</span><span class="sxs-lookup"><span data-stu-id="59d7c-103">Create deviceHealthScript</span></span>

> <span data-ttu-id="59d7c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59d7c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59d7c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="59d7c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59d7c-106">Создание нового объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="59d7c-106">Create a new [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59d7c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="59d7c-107">Prerequisites</span></span>
<span data-ttu-id="59d7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59d7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59d7c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59d7c-110">Permission type</span></span>|<span data-ttu-id="59d7c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="59d7c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59d7c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59d7c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="59d7c-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59d7c-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="59d7c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59d7c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59d7c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59d7c-115">Not supported.</span></span>|
|<span data-ttu-id="59d7c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59d7c-116">Application</span></span>|<span data-ttu-id="59d7c-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59d7c-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59d7c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59d7c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts
```

## <a name="request-headers"></a><span data-ttu-id="59d7c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="59d7c-119">Request headers</span></span>
|<span data-ttu-id="59d7c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59d7c-120">Header</span></span>|<span data-ttu-id="59d7c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="59d7c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59d7c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59d7c-122">Authorization</span></span>|<span data-ttu-id="59d7c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59d7c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59d7c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="59d7c-124">Accept</span></span>|<span data-ttu-id="59d7c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="59d7c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59d7c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="59d7c-126">Request body</span></span>
<span data-ttu-id="59d7c-127">В тексте запроса добавьте представление объекта Девицехеалсскрипт в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59d7c-127">In the request body, supply a JSON representation for the deviceHealthScript object.</span></span>

<span data-ttu-id="59d7c-128">В следующей таблице приведены свойства, необходимые при создании Девицехеалсскрипт.</span><span class="sxs-lookup"><span data-stu-id="59d7c-128">The following table shows the properties that are required when you create the deviceHealthScript.</span></span>

|<span data-ttu-id="59d7c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="59d7c-129">Property</span></span>|<span data-ttu-id="59d7c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="59d7c-130">Type</span></span>|<span data-ttu-id="59d7c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="59d7c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59d7c-132">id</span><span class="sxs-lookup"><span data-stu-id="59d7c-132">id</span></span>|<span data-ttu-id="59d7c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="59d7c-133">String</span></span>|<span data-ttu-id="59d7c-134">Уникальный идентификатор сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="59d7c-134">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="59d7c-135">publisher</span><span class="sxs-lookup"><span data-stu-id="59d7c-135">publisher</span></span>|<span data-ttu-id="59d7c-136">Строка</span><span class="sxs-lookup"><span data-stu-id="59d7c-136">String</span></span>|<span data-ttu-id="59d7c-137">Имя издателя сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="59d7c-137">Name of the device health script publisher</span></span>|
|<span data-ttu-id="59d7c-138">version</span><span class="sxs-lookup"><span data-stu-id="59d7c-138">version</span></span>|<span data-ttu-id="59d7c-139">String</span><span class="sxs-lookup"><span data-stu-id="59d7c-139">String</span></span>|<span data-ttu-id="59d7c-140">Версия сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="59d7c-140">Version of the device health script</span></span>|
|<span data-ttu-id="59d7c-141">displayName</span><span class="sxs-lookup"><span data-stu-id="59d7c-141">displayName</span></span>|<span data-ttu-id="59d7c-142">Строка</span><span class="sxs-lookup"><span data-stu-id="59d7c-142">String</span></span>|<span data-ttu-id="59d7c-143">Имя сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="59d7c-143">Name of the device health script</span></span>|
|<span data-ttu-id="59d7c-144">description</span><span class="sxs-lookup"><span data-stu-id="59d7c-144">description</span></span>|<span data-ttu-id="59d7c-145">String</span><span class="sxs-lookup"><span data-stu-id="59d7c-145">String</span></span>|<span data-ttu-id="59d7c-146">Описание сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="59d7c-146">Description of the device health script</span></span>|
|<span data-ttu-id="59d7c-147">детектионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="59d7c-147">detectionScriptContent</span></span>|<span data-ttu-id="59d7c-148">Binary</span><span class="sxs-lookup"><span data-stu-id="59d7c-148">Binary</span></span>|<span data-ttu-id="59d7c-149">Весь контент скрипта обнаружения PowerShell</span><span class="sxs-lookup"><span data-stu-id="59d7c-149">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="59d7c-150">ремедиатионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="59d7c-150">remediationScriptContent</span></span>|<span data-ttu-id="59d7c-151">Binary</span><span class="sxs-lookup"><span data-stu-id="59d7c-151">Binary</span></span>|<span data-ttu-id="59d7c-152">Все содержимое скрипта PowerShell об исправлении</span><span class="sxs-lookup"><span data-stu-id="59d7c-152">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="59d7c-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59d7c-153">createdDateTime</span></span>|<span data-ttu-id="59d7c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59d7c-154">DateTimeOffset</span></span>|<span data-ttu-id="59d7c-155">Метка времени создания сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="59d7c-155">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="59d7c-156">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="59d7c-156">This property is read-only.</span></span>|
|<span data-ttu-id="59d7c-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59d7c-157">lastModifiedDateTime</span></span>|<span data-ttu-id="59d7c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59d7c-158">DateTimeOffset</span></span>|<span data-ttu-id="59d7c-159">Метка времени изменения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="59d7c-159">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="59d7c-160">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="59d7c-160">This property is read-only.</span></span>|
|<span data-ttu-id="59d7c-161">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="59d7c-161">runAsAccount</span></span>|[<span data-ttu-id="59d7c-162">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="59d7c-162">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="59d7c-163">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="59d7c-163">Indicates the type of execution context.</span></span> <span data-ttu-id="59d7c-164">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="59d7c-164">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="59d7c-165">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="59d7c-165">enforceSignatureCheck</span></span>|<span data-ttu-id="59d7c-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d7c-166">Boolean</span></span>|<span data-ttu-id="59d7c-167">Указывает, нужно ли проверять подпись скрипта</span><span class="sxs-lookup"><span data-stu-id="59d7c-167">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="59d7c-168">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="59d7c-168">runAs32Bit</span></span>|<span data-ttu-id="59d7c-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="59d7c-169">Boolean</span></span>|<span data-ttu-id="59d7c-170">Указывает, следует ли выполнять скрипты PowerShell как 32-разрядные</span><span class="sxs-lookup"><span data-stu-id="59d7c-170">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="59d7c-171">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="59d7c-171">roleScopeTagIds</span></span>|<span data-ttu-id="59d7c-172">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="59d7c-172">String collection</span></span>|<span data-ttu-id="59d7c-173">Список идентификаторов тегов области для сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="59d7c-173">List of Scope Tag IDs for the device health script</span></span>|



## <a name="response"></a><span data-ttu-id="59d7c-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="59d7c-174">Response</span></span>
<span data-ttu-id="59d7c-175">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="59d7c-175">If successful, this method returns a `201 Created` response code and a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59d7c-176">Пример</span><span class="sxs-lookup"><span data-stu-id="59d7c-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="59d7c-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="59d7c-177">Request</span></span>
<span data-ttu-id="59d7c-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59d7c-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts
Content-type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="59d7c-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="59d7c-179">Response</span></span>
<span data-ttu-id="59d7c-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59d7c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 655

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
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





