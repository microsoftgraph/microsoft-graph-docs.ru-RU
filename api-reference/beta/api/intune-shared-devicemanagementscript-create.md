---
title: Создание deviceManagementScript
description: Создание нового объекта deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a4b93130c66977d9ccf3f0ad2fcedfbfe9cae6c7
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538163"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="6c6fd-103">Создание deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="6c6fd-103">Create deviceManagementScript</span></span>

> <span data-ttu-id="6c6fd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c6fd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c6fd-106">Создание нового объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="6c6fd-106">Create a new [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c6fd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6c6fd-107">Prerequisites</span></span>
<span data-ttu-id="6c6fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c6fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c6fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c6fd-110">Permission type</span></span>|<span data-ttu-id="6c6fd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c6fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c6fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c6fd-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6c6fd-113">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="6c6fd-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6c6fd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c6fd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="6c6fd-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="6c6fd-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6c6fd-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c6fd-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6c6fd-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c6fd-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c6fd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-118">Not supported.</span></span>|
|<span data-ttu-id="6c6fd-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="6c6fd-119">Application</span></span>||
| <span data-ttu-id="6c6fd-120">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="6c6fd-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6c6fd-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c6fd-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="6c6fd-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="6c6fd-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6c6fd-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c6fd-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c6fd-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c6fd-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="6c6fd-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c6fd-125">Request headers</span></span>
|<span data-ttu-id="6c6fd-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c6fd-126">Header</span></span>|<span data-ttu-id="6c6fd-127">Значение</span><span class="sxs-lookup"><span data-stu-id="6c6fd-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c6fd-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c6fd-128">Authorization</span></span>|<span data-ttu-id="6c6fd-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c6fd-130">Accept</span><span class="sxs-lookup"><span data-stu-id="6c6fd-130">Accept</span></span>|<span data-ttu-id="6c6fd-131">application/json</span><span class="sxs-lookup"><span data-stu-id="6c6fd-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c6fd-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c6fd-132">Request body</span></span>
<span data-ttu-id="6c6fd-133">В тексте запроса добавьте представление объекта deviceManagementScript в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-133">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="6c6fd-134">В следующей таблице приведены свойства, необходимые при создании deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-134">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="6c6fd-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c6fd-135">Property</span></span>|<span data-ttu-id="6c6fd-136">Тип</span><span class="sxs-lookup"><span data-stu-id="6c6fd-136">Type</span></span>|<span data-ttu-id="6c6fd-137">Описание</span><span class="sxs-lookup"><span data-stu-id="6c6fd-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c6fd-138">id</span><span class="sxs-lookup"><span data-stu-id="6c6fd-138">id</span></span>|<span data-ttu-id="6c6fd-139">Строка</span><span class="sxs-lookup"><span data-stu-id="6c6fd-139">String</span></span>|<span data-ttu-id="6c6fd-140">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-140">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="6c6fd-141">displayName</span><span class="sxs-lookup"><span data-stu-id="6c6fd-141">displayName</span></span>|<span data-ttu-id="6c6fd-142">Строка</span><span class="sxs-lookup"><span data-stu-id="6c6fd-142">String</span></span>|<span data-ttu-id="6c6fd-143">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-143">Name of the device management script.</span></span>|
|<span data-ttu-id="6c6fd-144">description</span><span class="sxs-lookup"><span data-stu-id="6c6fd-144">description</span></span>|<span data-ttu-id="6c6fd-145">String</span><span class="sxs-lookup"><span data-stu-id="6c6fd-145">String</span></span>|<span data-ttu-id="6c6fd-146">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-146">Optional description for the device management script.</span></span>|
|<span data-ttu-id="6c6fd-147">runSchedule</span><span class="sxs-lookup"><span data-stu-id="6c6fd-147">runSchedule</span></span>|[<span data-ttu-id="6c6fd-148">runSchedule</span><span class="sxs-lookup"><span data-stu-id="6c6fd-148">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="6c6fd-149">Интервал для запуска скрипта.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-149">The interval for script to run.</span></span> <span data-ttu-id="6c6fd-150">Если не определен, сценарий будет выполняться один раз</span><span class="sxs-lookup"><span data-stu-id="6c6fd-150">If not defined the script will run once</span></span>|
|<span data-ttu-id="6c6fd-151">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="6c6fd-151">scriptContent</span></span>|<span data-ttu-id="6c6fd-152">Binary</span><span class="sxs-lookup"><span data-stu-id="6c6fd-152">Binary</span></span>|<span data-ttu-id="6c6fd-153">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-153">The script content.</span></span>|
|<span data-ttu-id="6c6fd-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c6fd-154">createdDateTime</span></span>|<span data-ttu-id="6c6fd-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c6fd-155">DateTimeOffset</span></span>|<span data-ttu-id="6c6fd-156">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-156">The date and time the device management script was created.</span></span> <span data-ttu-id="6c6fd-157">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-157">This property is read-only.</span></span>|
|<span data-ttu-id="6c6fd-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c6fd-158">lastModifiedDateTime</span></span>|<span data-ttu-id="6c6fd-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c6fd-159">DateTimeOffset</span></span>|<span data-ttu-id="6c6fd-160">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-160">The date and time the device management script was last modified.</span></span> <span data-ttu-id="6c6fd-161">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-161">This property is read-only.</span></span>|
|<span data-ttu-id="6c6fd-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="6c6fd-162">runAsAccount</span></span>|[<span data-ttu-id="6c6fd-163">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="6c6fd-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="6c6fd-164">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-164">Indicates the type of execution context.</span></span> <span data-ttu-id="6c6fd-165">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="6c6fd-166">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="6c6fd-166">enforceSignatureCheck</span></span>|<span data-ttu-id="6c6fd-167">Логический</span><span class="sxs-lookup"><span data-stu-id="6c6fd-167">Boolean</span></span>|<span data-ttu-id="6c6fd-168">Указывает, нужно ли проверять подпись скрипта.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-168">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="6c6fd-169">fileName</span><span class="sxs-lookup"><span data-stu-id="6c6fd-169">fileName</span></span>|<span data-ttu-id="6c6fd-170">String</span><span class="sxs-lookup"><span data-stu-id="6c6fd-170">String</span></span>|<span data-ttu-id="6c6fd-171">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-171">Script file name.</span></span>|
|<span data-ttu-id="6c6fd-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6c6fd-172">roleScopeTagIds</span></span>|<span data-ttu-id="6c6fd-173">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6c6fd-173">String collection</span></span>|<span data-ttu-id="6c6fd-174">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-174">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="6c6fd-175">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="6c6fd-175">runAs32Bit</span></span>|<span data-ttu-id="6c6fd-176">Логический</span><span class="sxs-lookup"><span data-stu-id="6c6fd-176">Boolean</span></span>|<span data-ttu-id="6c6fd-177">Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="6c6fd-177">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="6c6fd-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c6fd-178">Response</span></span>
<span data-ttu-id="6c6fd-179">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-179">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c6fd-180">Пример</span><span class="sxs-lookup"><span data-stu-id="6c6fd-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c6fd-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c6fd-181">Request</span></span>
<span data-ttu-id="6c6fd-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```

### <a name="response"></a><span data-ttu-id="6c6fd-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c6fd-183">Response</span></span>
<span data-ttu-id="6c6fd-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c6fd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 615

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```






