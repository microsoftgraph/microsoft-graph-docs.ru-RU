---
title: Создание deviceManagementScript
description: Создание нового объекта deviceManagementScript.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13afc26b59d6e9d46b68e1754f9b4362b5bda916
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465883"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="dea49-103">Создание deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="dea49-103">Create deviceManagementScript</span></span>

> <span data-ttu-id="dea49-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dea49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dea49-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dea49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dea49-106">Создание нового объекта [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="dea49-106">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dea49-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dea49-107">Prerequisites</span></span>
<span data-ttu-id="dea49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dea49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dea49-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dea49-110">Permission type</span></span>|<span data-ttu-id="dea49-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dea49-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dea49-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dea49-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dea49-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dea49-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="dea49-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dea49-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dea49-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dea49-115">Not supported.</span></span>|
|<span data-ttu-id="dea49-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dea49-116">Application</span></span>|<span data-ttu-id="dea49-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dea49-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dea49-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dea49-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="dea49-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dea49-119">Request headers</span></span>
|<span data-ttu-id="dea49-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dea49-120">Header</span></span>|<span data-ttu-id="dea49-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dea49-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dea49-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dea49-122">Authorization</span></span>|<span data-ttu-id="dea49-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dea49-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dea49-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dea49-124">Accept</span></span>|<span data-ttu-id="dea49-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dea49-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dea49-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dea49-126">Request body</span></span>
<span data-ttu-id="dea49-127">В тексте запроса добавьте представление объекта deviceManagementScript в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dea49-127">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="dea49-128">В следующей таблице приведены свойства, необходимые при создании deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="dea49-128">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="dea49-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dea49-129">Property</span></span>|<span data-ttu-id="dea49-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dea49-130">Type</span></span>|<span data-ttu-id="dea49-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dea49-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dea49-132">id</span><span class="sxs-lookup"><span data-stu-id="dea49-132">id</span></span>|<span data-ttu-id="dea49-133">Строка</span><span class="sxs-lookup"><span data-stu-id="dea49-133">String</span></span>|<span data-ttu-id="dea49-134">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="dea49-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="dea49-135">displayName</span><span class="sxs-lookup"><span data-stu-id="dea49-135">displayName</span></span>|<span data-ttu-id="dea49-136">Строка</span><span class="sxs-lookup"><span data-stu-id="dea49-136">String</span></span>|<span data-ttu-id="dea49-137">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="dea49-137">Name of the device management script.</span></span>|
|<span data-ttu-id="dea49-138">description</span><span class="sxs-lookup"><span data-stu-id="dea49-138">description</span></span>|<span data-ttu-id="dea49-139">String</span><span class="sxs-lookup"><span data-stu-id="dea49-139">String</span></span>|<span data-ttu-id="dea49-140">НеОбязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="dea49-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="dea49-141">runSchedule</span><span class="sxs-lookup"><span data-stu-id="dea49-141">runSchedule</span></span>|[<span data-ttu-id="dea49-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="dea49-142">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="dea49-143">Интервал для запуска скрипта.</span><span class="sxs-lookup"><span data-stu-id="dea49-143">The interval for script to run.</span></span> <span data-ttu-id="dea49-144">Если не определен, сценарий будет выполняться один раз</span><span class="sxs-lookup"><span data-stu-id="dea49-144">If not defined the script will run once</span></span>|
|<span data-ttu-id="dea49-145">Скриптконтент</span><span class="sxs-lookup"><span data-stu-id="dea49-145">scriptContent</span></span>|<span data-ttu-id="dea49-146">Binary</span><span class="sxs-lookup"><span data-stu-id="dea49-146">Binary</span></span>|<span data-ttu-id="dea49-147">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="dea49-147">The script content.</span></span>|
|<span data-ttu-id="dea49-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dea49-148">createdDateTime</span></span>|<span data-ttu-id="dea49-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dea49-149">DateTimeOffset</span></span>|<span data-ttu-id="dea49-150">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="dea49-150">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="dea49-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dea49-151">lastModifiedDateTime</span></span>|<span data-ttu-id="dea49-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dea49-152">DateTimeOffset</span></span>|<span data-ttu-id="dea49-153">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="dea49-153">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="dea49-154">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="dea49-154">runAsAccount</span></span>|[<span data-ttu-id="dea49-155">Рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="dea49-155">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="dea49-156">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="dea49-156">Indicates the type of execution context.</span></span> <span data-ttu-id="dea49-157">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="dea49-157">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="dea49-158">Свойства enforcesignaturecheck</span><span class="sxs-lookup"><span data-stu-id="dea49-158">enforceSignatureCheck</span></span>|<span data-ttu-id="dea49-159">Логический</span><span class="sxs-lookup"><span data-stu-id="dea49-159">Boolean</span></span>|<span data-ttu-id="dea49-160">Указывает, нужно ли проверять подпись скрипта.</span><span class="sxs-lookup"><span data-stu-id="dea49-160">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="dea49-161">fileName</span><span class="sxs-lookup"><span data-stu-id="dea49-161">fileName</span></span>|<span data-ttu-id="dea49-162">String</span><span class="sxs-lookup"><span data-stu-id="dea49-162">String</span></span>|<span data-ttu-id="dea49-163">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="dea49-163">Script file name.</span></span>|
|<span data-ttu-id="dea49-164">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dea49-164">roleScopeTagIds</span></span>|<span data-ttu-id="dea49-165">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="dea49-165">String collection</span></span>|<span data-ttu-id="dea49-166">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="dea49-166">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="dea49-167">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="dea49-167">runAs32Bit</span></span>|<span data-ttu-id="dea49-168">Логический</span><span class="sxs-lookup"><span data-stu-id="dea49-168">Boolean</span></span>|<span data-ttu-id="dea49-169">Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 бит</span><span class="sxs-lookup"><span data-stu-id="dea49-169">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="dea49-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="dea49-170">Response</span></span>
<span data-ttu-id="dea49-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dea49-171">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dea49-172">Пример</span><span class="sxs-lookup"><span data-stu-id="dea49-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="dea49-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="dea49-173">Request</span></span>
<span data-ttu-id="dea49-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dea49-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dea49-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="dea49-175">Response</span></span>
<span data-ttu-id="dea49-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dea49-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





