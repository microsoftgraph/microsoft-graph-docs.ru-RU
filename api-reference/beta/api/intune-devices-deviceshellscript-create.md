---
title: Создание Девицешеллскрипт
description: Создание нового объекта Девицешеллскрипт.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c686f45d266241ce7cb42bbaef2d8020149a81aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994626"
---
# <a name="create-deviceshellscript"></a><span data-ttu-id="93490-103">Создание Девицешеллскрипт</span><span class="sxs-lookup"><span data-stu-id="93490-103">Create deviceShellScript</span></span>

<span data-ttu-id="93490-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93490-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93490-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93490-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93490-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93490-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93490-107">Создание нового объекта [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="93490-107">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93490-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="93490-108">Prerequisites</span></span>
<span data-ttu-id="93490-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93490-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93490-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93490-111">Permission type</span></span>|<span data-ttu-id="93490-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="93490-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93490-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93490-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93490-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93490-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="93490-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93490-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93490-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93490-116">Not supported.</span></span>|
|<span data-ttu-id="93490-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93490-117">Application</span></span>|<span data-ttu-id="93490-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93490-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93490-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93490-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="93490-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="93490-120">Request headers</span></span>
|<span data-ttu-id="93490-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93490-121">Header</span></span>|<span data-ttu-id="93490-122">Значение</span><span class="sxs-lookup"><span data-stu-id="93490-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93490-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="93490-123">Authorization</span></span>|<span data-ttu-id="93490-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93490-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93490-125">Accept</span><span class="sxs-lookup"><span data-stu-id="93490-125">Accept</span></span>|<span data-ttu-id="93490-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93490-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93490-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="93490-127">Request body</span></span>
<span data-ttu-id="93490-128">В тексте запроса добавьте представление объекта Девицешеллскрипт в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93490-128">In the request body, supply a JSON representation for the deviceShellScript object.</span></span>

<span data-ttu-id="93490-129">В следующей таблице приведены свойства, необходимые при создании Девицешеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="93490-129">The following table shows the properties that are required when you create the deviceShellScript.</span></span>

|<span data-ttu-id="93490-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="93490-130">Property</span></span>|<span data-ttu-id="93490-131">Тип</span><span class="sxs-lookup"><span data-stu-id="93490-131">Type</span></span>|<span data-ttu-id="93490-132">Описание</span><span class="sxs-lookup"><span data-stu-id="93490-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93490-133">ексекутионфрекуенци</span><span class="sxs-lookup"><span data-stu-id="93490-133">executionFrequency</span></span>|<span data-ttu-id="93490-134">Длительность</span><span class="sxs-lookup"><span data-stu-id="93490-134">Duration</span></span>|<span data-ttu-id="93490-135">Интервал для запуска скрипта.</span><span class="sxs-lookup"><span data-stu-id="93490-135">The interval for script to run.</span></span> <span data-ttu-id="93490-136">Если не определен, сценарий будет выполняться один раз</span><span class="sxs-lookup"><span data-stu-id="93490-136">If not defined the script will run once</span></span>|
|<span data-ttu-id="93490-137">ретрикаунт</span><span class="sxs-lookup"><span data-stu-id="93490-137">retryCount</span></span>|<span data-ttu-id="93490-138">Int32</span><span class="sxs-lookup"><span data-stu-id="93490-138">Int32</span></span>|<span data-ttu-id="93490-139">Количество повторных попыток выполнения скрипта в случае сбоя</span><span class="sxs-lookup"><span data-stu-id="93490-139">Number of times for the script to be retried if it fails</span></span>|
|<span data-ttu-id="93490-140">блоккексекутионнотификатионс</span><span class="sxs-lookup"><span data-stu-id="93490-140">blockExecutionNotifications</span></span>|<span data-ttu-id="93490-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="93490-141">Boolean</span></span>|<span data-ttu-id="93490-142">Не уведомляет пользователя о выполнении сценария</span><span class="sxs-lookup"><span data-stu-id="93490-142">Does not notify the user a script is being executed</span></span>|
|<span data-ttu-id="93490-143">id</span><span class="sxs-lookup"><span data-stu-id="93490-143">id</span></span>|<span data-ttu-id="93490-144">String</span><span class="sxs-lookup"><span data-stu-id="93490-144">String</span></span>|<span data-ttu-id="93490-145">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="93490-145">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="93490-146">displayName</span><span class="sxs-lookup"><span data-stu-id="93490-146">displayName</span></span>|<span data-ttu-id="93490-147">String</span><span class="sxs-lookup"><span data-stu-id="93490-147">String</span></span>|<span data-ttu-id="93490-148">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="93490-148">Name of the device management script.</span></span>|
|<span data-ttu-id="93490-149">description</span><span class="sxs-lookup"><span data-stu-id="93490-149">description</span></span>|<span data-ttu-id="93490-150">String</span><span class="sxs-lookup"><span data-stu-id="93490-150">String</span></span>|<span data-ttu-id="93490-151">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="93490-151">Optional description for the device management script.</span></span>|
|<span data-ttu-id="93490-152">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="93490-152">scriptContent</span></span>|<span data-ttu-id="93490-153">Binary</span><span class="sxs-lookup"><span data-stu-id="93490-153">Binary</span></span>|<span data-ttu-id="93490-154">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="93490-154">The script content.</span></span>|
|<span data-ttu-id="93490-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93490-155">createdDateTime</span></span>|<span data-ttu-id="93490-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93490-156">DateTimeOffset</span></span>|<span data-ttu-id="93490-157">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="93490-157">The date and time the device management script was created.</span></span> <span data-ttu-id="93490-158">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="93490-158">This property is read-only.</span></span>|
|<span data-ttu-id="93490-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93490-159">lastModifiedDateTime</span></span>|<span data-ttu-id="93490-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93490-160">DateTimeOffset</span></span>|<span data-ttu-id="93490-161">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="93490-161">The date and time the device management script was last modified.</span></span> <span data-ttu-id="93490-162">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="93490-162">This property is read-only.</span></span>|
|<span data-ttu-id="93490-163">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="93490-163">runAsAccount</span></span>|[<span data-ttu-id="93490-164">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="93490-164">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="93490-165">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="93490-165">Indicates the type of execution context.</span></span> <span data-ttu-id="93490-166">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="93490-166">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="93490-167">fileName</span><span class="sxs-lookup"><span data-stu-id="93490-167">fileName</span></span>|<span data-ttu-id="93490-168">String</span><span class="sxs-lookup"><span data-stu-id="93490-168">String</span></span>|<span data-ttu-id="93490-169">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="93490-169">Script file name.</span></span>|
|<span data-ttu-id="93490-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="93490-170">roleScopeTagIds</span></span>|<span data-ttu-id="93490-171">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="93490-171">String collection</span></span>|<span data-ttu-id="93490-172">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="93490-172">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="93490-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="93490-173">Response</span></span>
<span data-ttu-id="93490-174">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93490-174">If successful, this method returns a `201 Created` response code and a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93490-175">Пример</span><span class="sxs-lookup"><span data-stu-id="93490-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="93490-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="93490-176">Request</span></span>
<span data-ttu-id="93490-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93490-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts
Content-type: application/json
Content-length: 409

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "executionFrequency": "PT2M43.444327S",
  "retryCount": 10,
  "blockExecutionNotifications": true,
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="93490-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="93490-178">Response</span></span>
<span data-ttu-id="93490-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93490-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "executionFrequency": "PT2M43.444327S",
  "retryCount": 10,
  "blockExecutionNotifications": true,
  "id": "ca9e0ad8-0ad8-ca9e-d80a-9ecad80a9eca",
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```






