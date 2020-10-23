---
title: Создание Девицекомплианцескрипт
description: Создание нового объекта Девицекомплианцескрипт.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9d73441f0925e183185babac04869541c11316c2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732939"
---
# <a name="create-devicecompliancescript"></a><span data-ttu-id="c2cbc-103">Создание Девицекомплианцескрипт</span><span class="sxs-lookup"><span data-stu-id="c2cbc-103">Create deviceComplianceScript</span></span>

<span data-ttu-id="c2cbc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2cbc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2cbc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2cbc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2cbc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2cbc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2cbc-107">Создание нового объекта [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md) .</span><span class="sxs-lookup"><span data-stu-id="c2cbc-107">Create a new [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2cbc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c2cbc-108">Prerequisites</span></span>
<span data-ttu-id="c2cbc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2cbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2cbc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2cbc-111">Permission type</span></span>|<span data-ttu-id="c2cbc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2cbc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2cbc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2cbc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2cbc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2cbc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c2cbc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2cbc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2cbc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2cbc-116">Not supported.</span></span>|
|<span data-ttu-id="c2cbc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2cbc-117">Application</span></span>|<span data-ttu-id="c2cbc-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2cbc-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2cbc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2cbc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceComplianceScripts
```

## <a name="request-headers"></a><span data-ttu-id="c2cbc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c2cbc-120">Request headers</span></span>
|<span data-ttu-id="c2cbc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2cbc-121">Header</span></span>|<span data-ttu-id="c2cbc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c2cbc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2cbc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2cbc-123">Authorization</span></span>|<span data-ttu-id="c2cbc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2cbc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2cbc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2cbc-125">Accept</span></span>|<span data-ttu-id="c2cbc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2cbc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2cbc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c2cbc-127">Request body</span></span>
<span data-ttu-id="c2cbc-128">В тексте запроса добавьте представление объекта Девицекомплианцескрипт в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2cbc-128">In the request body, supply a JSON representation for the deviceComplianceScript object.</span></span>

<span data-ttu-id="c2cbc-129">В следующей таблице приведены свойства, необходимые при создании Девицекомплианцескрипт.</span><span class="sxs-lookup"><span data-stu-id="c2cbc-129">The following table shows the properties that are required when you create the deviceComplianceScript.</span></span>

|<span data-ttu-id="c2cbc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2cbc-130">Property</span></span>|<span data-ttu-id="c2cbc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c2cbc-131">Type</span></span>|<span data-ttu-id="c2cbc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c2cbc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2cbc-133">id</span><span class="sxs-lookup"><span data-stu-id="c2cbc-133">id</span></span>|<span data-ttu-id="c2cbc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c2cbc-134">String</span></span>|<span data-ttu-id="c2cbc-135">Уникальный идентификатор для сценария соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="c2cbc-135">Unique Identifier for the device compliance script</span></span>|
|<span data-ttu-id="c2cbc-136">publisher</span><span class="sxs-lookup"><span data-stu-id="c2cbc-136">publisher</span></span>|<span data-ttu-id="c2cbc-137">String</span><span class="sxs-lookup"><span data-stu-id="c2cbc-137">String</span></span>|<span data-ttu-id="c2cbc-138">Имя издателя сценариев соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="c2cbc-138">Name of the device compliance script publisher</span></span>|
|<span data-ttu-id="c2cbc-139">version</span><span class="sxs-lookup"><span data-stu-id="c2cbc-139">version</span></span>|<span data-ttu-id="c2cbc-140">String</span><span class="sxs-lookup"><span data-stu-id="c2cbc-140">String</span></span>|<span data-ttu-id="c2cbc-141">Версия сценария соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="c2cbc-141">Version of the device compliance script</span></span>|
|<span data-ttu-id="c2cbc-142">displayName</span><span class="sxs-lookup"><span data-stu-id="c2cbc-142">displayName</span></span>|<span data-ttu-id="c2cbc-143">Строка</span><span class="sxs-lookup"><span data-stu-id="c2cbc-143">String</span></span>|<span data-ttu-id="c2cbc-144">Имя сценария соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="c2cbc-144">Name of the device compliance script</span></span>|
|<span data-ttu-id="c2cbc-145">description</span><span class="sxs-lookup"><span data-stu-id="c2cbc-145">description</span></span>|<span data-ttu-id="c2cbc-146">Строка</span><span class="sxs-lookup"><span data-stu-id="c2cbc-146">String</span></span>|<span data-ttu-id="c2cbc-147">Описание сценария соответствия требованиям устройства</span><span class="sxs-lookup"><span data-stu-id="c2cbc-147">Description of the device compliance script</span></span>|
|<span data-ttu-id="c2cbc-148">детектионскриптконтент</span><span class="sxs-lookup"><span data-stu-id="c2cbc-148">detectionScriptContent</span></span>|<span data-ttu-id="c2cbc-149">Binary</span><span class="sxs-lookup"><span data-stu-id="c2cbc-149">Binary</span></span>|<span data-ttu-id="c2cbc-150">Весь контент скрипта обнаружения PowerShell</span><span class="sxs-lookup"><span data-stu-id="c2cbc-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="c2cbc-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c2cbc-151">createdDateTime</span></span>|<span data-ttu-id="c2cbc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2cbc-152">DateTimeOffset</span></span>|<span data-ttu-id="c2cbc-153">Метка времени создания сценария соответствия устройства требованиям.</span><span class="sxs-lookup"><span data-stu-id="c2cbc-153">The timestamp of when the device compliance script was created.</span></span> <span data-ttu-id="c2cbc-154">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2cbc-154">This property is read-only.</span></span>|
|<span data-ttu-id="c2cbc-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2cbc-155">lastModifiedDateTime</span></span>|<span data-ttu-id="c2cbc-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2cbc-156">DateTimeOffset</span></span>|<span data-ttu-id="c2cbc-157">Метка времени изменения сценария соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="c2cbc-157">The timestamp of when the device compliance script was modified.</span></span> <span data-ttu-id="c2cbc-158">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2cbc-158">This property is read-only.</span></span>|
|<span data-ttu-id="c2cbc-159">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="c2cbc-159">runAsAccount</span></span>|[<span data-ttu-id="c2cbc-160">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="c2cbc-160">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="c2cbc-161">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="c2cbc-161">Indicates the type of execution context.</span></span> <span data-ttu-id="c2cbc-162">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="c2cbc-162">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="c2cbc-163">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="c2cbc-163">enforceSignatureCheck</span></span>|<span data-ttu-id="c2cbc-164">Логический</span><span class="sxs-lookup"><span data-stu-id="c2cbc-164">Boolean</span></span>|<span data-ttu-id="c2cbc-165">Указывает, нужно ли проверять подпись скрипта</span><span class="sxs-lookup"><span data-stu-id="c2cbc-165">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="c2cbc-166">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="c2cbc-166">runAs32Bit</span></span>|<span data-ttu-id="c2cbc-167">Логический</span><span class="sxs-lookup"><span data-stu-id="c2cbc-167">Boolean</span></span>|<span data-ttu-id="c2cbc-168">Указывает, следует ли выполнять скрипты PowerShell как 32-разрядные</span><span class="sxs-lookup"><span data-stu-id="c2cbc-168">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="c2cbc-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c2cbc-169">roleScopeTagIds</span></span>|<span data-ttu-id="c2cbc-170">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c2cbc-170">String collection</span></span>|<span data-ttu-id="c2cbc-171">Список идентификаторов тегов области для сценария соответствия требованиям устройств</span><span class="sxs-lookup"><span data-stu-id="c2cbc-171">List of Scope Tag IDs for the device compliance script</span></span>|



## <a name="response"></a><span data-ttu-id="c2cbc-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2cbc-172">Response</span></span>
<span data-ttu-id="c2cbc-173">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицекомплианцескрипт](../resources/intune-devices-devicecompliancescript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2cbc-173">If successful, this method returns a `201 Created` response code and a [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2cbc-174">Пример</span><span class="sxs-lookup"><span data-stu-id="c2cbc-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2cbc-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2cbc-175">Request</span></span>
<span data-ttu-id="c2cbc-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2cbc-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c2cbc-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2cbc-177">Response</span></span>
<span data-ttu-id="c2cbc-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2cbc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





