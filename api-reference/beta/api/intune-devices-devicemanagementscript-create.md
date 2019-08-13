---
title: Создание deviceManagementScript
description: Создание нового объекта deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e83d34f519093dbc6e7b70a2cda385be7426d2c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310544"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="73af5-103">Создание deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="73af5-103">Create deviceManagementScript</span></span>

> <span data-ttu-id="73af5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73af5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73af5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73af5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73af5-106">Создание нового объекта [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="73af5-106">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73af5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="73af5-107">Prerequisites</span></span>
<span data-ttu-id="73af5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73af5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73af5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73af5-110">Permission type</span></span>|<span data-ttu-id="73af5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73af5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73af5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73af5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73af5-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73af5-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="73af5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73af5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73af5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73af5-115">Not supported.</span></span>|
|<span data-ttu-id="73af5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73af5-116">Application</span></span>|<span data-ttu-id="73af5-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73af5-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73af5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73af5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="73af5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73af5-119">Request headers</span></span>
|<span data-ttu-id="73af5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73af5-120">Header</span></span>|<span data-ttu-id="73af5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="73af5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73af5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73af5-122">Authorization</span></span>|<span data-ttu-id="73af5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73af5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73af5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="73af5-124">Accept</span></span>|<span data-ttu-id="73af5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73af5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73af5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="73af5-126">Request body</span></span>
<span data-ttu-id="73af5-127">В тексте запроса добавьте представление объекта deviceManagementScript в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73af5-127">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="73af5-128">В следующей таблице приведены свойства, необходимые при создании deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="73af5-128">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="73af5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="73af5-129">Property</span></span>|<span data-ttu-id="73af5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="73af5-130">Type</span></span>|<span data-ttu-id="73af5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="73af5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73af5-132">id</span><span class="sxs-lookup"><span data-stu-id="73af5-132">id</span></span>|<span data-ttu-id="73af5-133">Строка</span><span class="sxs-lookup"><span data-stu-id="73af5-133">String</span></span>|<span data-ttu-id="73af5-134">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="73af5-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="73af5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="73af5-135">displayName</span></span>|<span data-ttu-id="73af5-136">Строка</span><span class="sxs-lookup"><span data-stu-id="73af5-136">String</span></span>|<span data-ttu-id="73af5-137">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="73af5-137">Name of the device management script.</span></span>|
|<span data-ttu-id="73af5-138">description</span><span class="sxs-lookup"><span data-stu-id="73af5-138">description</span></span>|<span data-ttu-id="73af5-139">String</span><span class="sxs-lookup"><span data-stu-id="73af5-139">String</span></span>|<span data-ttu-id="73af5-140">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="73af5-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="73af5-141">runSchedule</span><span class="sxs-lookup"><span data-stu-id="73af5-141">runSchedule</span></span>|[<span data-ttu-id="73af5-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="73af5-142">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="73af5-143">Интервал для запуска скрипта.</span><span class="sxs-lookup"><span data-stu-id="73af5-143">The interval for script to run.</span></span> <span data-ttu-id="73af5-144">Если не определен, сценарий будет выполняться один раз</span><span class="sxs-lookup"><span data-stu-id="73af5-144">If not defined the script will run once</span></span>|
|<span data-ttu-id="73af5-145">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="73af5-145">scriptContent</span></span>|<span data-ttu-id="73af5-146">Binary</span><span class="sxs-lookup"><span data-stu-id="73af5-146">Binary</span></span>|<span data-ttu-id="73af5-147">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="73af5-147">The script content.</span></span>|
|<span data-ttu-id="73af5-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73af5-148">createdDateTime</span></span>|<span data-ttu-id="73af5-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73af5-149">DateTimeOffset</span></span>|<span data-ttu-id="73af5-150">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="73af5-150">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="73af5-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73af5-151">lastModifiedDateTime</span></span>|<span data-ttu-id="73af5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73af5-152">DateTimeOffset</span></span>|<span data-ttu-id="73af5-153">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="73af5-153">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="73af5-154">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="73af5-154">runAsAccount</span></span>|[<span data-ttu-id="73af5-155">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="73af5-155">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="73af5-156">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="73af5-156">Indicates the type of execution context.</span></span> <span data-ttu-id="73af5-157">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="73af5-157">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="73af5-158">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="73af5-158">enforceSignatureCheck</span></span>|<span data-ttu-id="73af5-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="73af5-159">Boolean</span></span>|<span data-ttu-id="73af5-160">Указывает, нужно ли проверять подпись скрипта.</span><span class="sxs-lookup"><span data-stu-id="73af5-160">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="73af5-161">fileName</span><span class="sxs-lookup"><span data-stu-id="73af5-161">fileName</span></span>|<span data-ttu-id="73af5-162">String</span><span class="sxs-lookup"><span data-stu-id="73af5-162">String</span></span>|<span data-ttu-id="73af5-163">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="73af5-163">Script file name.</span></span>|
|<span data-ttu-id="73af5-164">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="73af5-164">roleScopeTagIds</span></span>|<span data-ttu-id="73af5-165">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="73af5-165">String collection</span></span>|<span data-ttu-id="73af5-166">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="73af5-166">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="73af5-167">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="73af5-167">runAs32Bit</span></span>|<span data-ttu-id="73af5-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="73af5-168">Boolean</span></span>|<span data-ttu-id="73af5-169">Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="73af5-169">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="73af5-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="73af5-170">Response</span></span>
<span data-ttu-id="73af5-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73af5-171">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73af5-172">Пример</span><span class="sxs-lookup"><span data-stu-id="73af5-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="73af5-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="73af5-173">Request</span></span>
<span data-ttu-id="73af5-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73af5-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="73af5-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="73af5-175">Response</span></span>
<span data-ttu-id="73af5-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73af5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






