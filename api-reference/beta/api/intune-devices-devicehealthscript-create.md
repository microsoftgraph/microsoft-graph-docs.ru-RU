---
title: Создание Девицехеалсскрипт
description: Создание нового объекта Девицехеалсскрипт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58296b1aae8d3582edda8e206900e65be659de6a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37532136"
---
# <a name="create-devicehealthscript"></a><span data-ttu-id="19e00-103">Создание Девицехеалсскрипт</span><span class="sxs-lookup"><span data-stu-id="19e00-103">Create deviceHealthScript</span></span>

> <span data-ttu-id="19e00-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19e00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19e00-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19e00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19e00-106">Создание нового объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="19e00-106">Create a new [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19e00-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="19e00-107">Prerequisites</span></span>
<span data-ttu-id="19e00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19e00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19e00-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19e00-110">Permission type</span></span>|<span data-ttu-id="19e00-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19e00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19e00-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19e00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19e00-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19e00-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="19e00-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19e00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19e00-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19e00-115">Not supported.</span></span>|
|<span data-ttu-id="19e00-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="19e00-116">Application</span></span>|<span data-ttu-id="19e00-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19e00-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="19e00-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19e00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts
```

## <a name="request-headers"></a><span data-ttu-id="19e00-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19e00-119">Request headers</span></span>
|<span data-ttu-id="19e00-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19e00-120">Header</span></span>|<span data-ttu-id="19e00-121">Значение</span><span class="sxs-lookup"><span data-stu-id="19e00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19e00-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19e00-122">Authorization</span></span>|<span data-ttu-id="19e00-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19e00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19e00-124">Accept</span><span class="sxs-lookup"><span data-stu-id="19e00-124">Accept</span></span>|<span data-ttu-id="19e00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19e00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19e00-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19e00-126">Request body</span></span>
<span data-ttu-id="19e00-127">В тексте запроса добавьте представление объекта Девицехеалсскрипт в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19e00-127">In the request body, supply a JSON representation for the deviceHealthScript object.</span></span>

<span data-ttu-id="19e00-128">В следующей таблице приведены свойства, необходимые при создании Девицехеалсскрипт.</span><span class="sxs-lookup"><span data-stu-id="19e00-128">The following table shows the properties that are required when you create the deviceHealthScript.</span></span>

|<span data-ttu-id="19e00-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="19e00-129">Property</span></span>|<span data-ttu-id="19e00-130">Тип</span><span class="sxs-lookup"><span data-stu-id="19e00-130">Type</span></span>|<span data-ttu-id="19e00-131">Описание</span><span class="sxs-lookup"><span data-stu-id="19e00-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19e00-132">id</span><span class="sxs-lookup"><span data-stu-id="19e00-132">id</span></span>|<span data-ttu-id="19e00-133">String</span><span class="sxs-lookup"><span data-stu-id="19e00-133">String</span></span>|<span data-ttu-id="19e00-134">Уникальный идентификатор сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="19e00-134">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="19e00-135">publisher</span><span class="sxs-lookup"><span data-stu-id="19e00-135">publisher</span></span>|<span data-ttu-id="19e00-136">String</span><span class="sxs-lookup"><span data-stu-id="19e00-136">String</span></span>|<span data-ttu-id="19e00-137">Имя издателя сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="19e00-137">Name of the device health script publisher</span></span>|
|<span data-ttu-id="19e00-138">version</span><span class="sxs-lookup"><span data-stu-id="19e00-138">version</span></span>|<span data-ttu-id="19e00-139">String</span><span class="sxs-lookup"><span data-stu-id="19e00-139">String</span></span>|<span data-ttu-id="19e00-140">Версия сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="19e00-140">Version of the device health script</span></span>|
|<span data-ttu-id="19e00-141">displayName</span><span class="sxs-lookup"><span data-stu-id="19e00-141">displayName</span></span>|<span data-ttu-id="19e00-142">Строка</span><span class="sxs-lookup"><span data-stu-id="19e00-142">String</span></span>|<span data-ttu-id="19e00-143">Имя сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="19e00-143">Name of the device health script</span></span>|
|<span data-ttu-id="19e00-144">description</span><span class="sxs-lookup"><span data-stu-id="19e00-144">description</span></span>|<span data-ttu-id="19e00-145">String</span><span class="sxs-lookup"><span data-stu-id="19e00-145">String</span></span>|<span data-ttu-id="19e00-146">Описание сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="19e00-146">Description of the device health script</span></span>|
|<span data-ttu-id="19e00-147">детектионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="19e00-147">detectionScriptContent</span></span>|<span data-ttu-id="19e00-148">Binary</span><span class="sxs-lookup"><span data-stu-id="19e00-148">Binary</span></span>|<span data-ttu-id="19e00-149">Весь контент скрипта обнаружения PowerShell</span><span class="sxs-lookup"><span data-stu-id="19e00-149">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="19e00-150">ремедиатионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="19e00-150">remediationScriptContent</span></span>|<span data-ttu-id="19e00-151">Binary</span><span class="sxs-lookup"><span data-stu-id="19e00-151">Binary</span></span>|<span data-ttu-id="19e00-152">Все содержимое скрипта PowerShell об исправлении</span><span class="sxs-lookup"><span data-stu-id="19e00-152">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="19e00-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19e00-153">createdDateTime</span></span>|<span data-ttu-id="19e00-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19e00-154">DateTimeOffset</span></span>|<span data-ttu-id="19e00-155">Метка времени создания сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="19e00-155">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="19e00-156">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19e00-156">This property is read-only.</span></span>|
|<span data-ttu-id="19e00-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19e00-157">lastModifiedDateTime</span></span>|<span data-ttu-id="19e00-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19e00-158">DateTimeOffset</span></span>|<span data-ttu-id="19e00-159">Метка времени изменения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="19e00-159">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="19e00-160">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19e00-160">This property is read-only.</span></span>|
|<span data-ttu-id="19e00-161">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="19e00-161">runAsAccount</span></span>|[<span data-ttu-id="19e00-162">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="19e00-162">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="19e00-163">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="19e00-163">Indicates the type of execution context.</span></span> <span data-ttu-id="19e00-164">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="19e00-164">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="19e00-165">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="19e00-165">enforceSignatureCheck</span></span>|<span data-ttu-id="19e00-166">Логический</span><span class="sxs-lookup"><span data-stu-id="19e00-166">Boolean</span></span>|<span data-ttu-id="19e00-167">Указывает, нужно ли проверять подпись скрипта</span><span class="sxs-lookup"><span data-stu-id="19e00-167">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="19e00-168">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="19e00-168">runAs32Bit</span></span>|<span data-ttu-id="19e00-169">Логический</span><span class="sxs-lookup"><span data-stu-id="19e00-169">Boolean</span></span>|<span data-ttu-id="19e00-170">Указывает, следует ли выполнять скрипты PowerShell как 32-разрядные</span><span class="sxs-lookup"><span data-stu-id="19e00-170">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="19e00-171">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="19e00-171">roleScopeTagIds</span></span>|<span data-ttu-id="19e00-172">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="19e00-172">String collection</span></span>|<span data-ttu-id="19e00-173">Список идентификаторов тегов области для сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="19e00-173">List of Scope Tag IDs for the device health script</span></span>|



## <a name="response"></a><span data-ttu-id="19e00-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="19e00-174">Response</span></span>
<span data-ttu-id="19e00-175">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="19e00-175">If successful, this method returns a `201 Created` response code and a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19e00-176">Пример</span><span class="sxs-lookup"><span data-stu-id="19e00-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="19e00-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="19e00-177">Request</span></span>
<span data-ttu-id="19e00-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19e00-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="19e00-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="19e00-179">Response</span></span>
<span data-ttu-id="19e00-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19e00-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






