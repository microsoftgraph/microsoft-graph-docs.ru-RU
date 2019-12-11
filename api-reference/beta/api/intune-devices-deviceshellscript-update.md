---
title: Обновление Девицешеллскрипт
description: Обновление свойств объекта Девицешеллскрипт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e6296caa1a6f9bf1db185bd16810f2733a30e943
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944843"
---
# <a name="update-deviceshellscript"></a><span data-ttu-id="6a299-103">Обновление Девицешеллскрипт</span><span class="sxs-lookup"><span data-stu-id="6a299-103">Update deviceShellScript</span></span>

> <span data-ttu-id="6a299-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a299-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a299-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a299-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a299-106">Обновление свойств объекта [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="6a299-106">Update the properties of a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a299-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6a299-107">Prerequisites</span></span>
<span data-ttu-id="6a299-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a299-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a299-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a299-110">Permission type</span></span>|<span data-ttu-id="6a299-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a299-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a299-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a299-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a299-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a299-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6a299-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a299-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a299-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a299-115">Not supported.</span></span>|
|<span data-ttu-id="6a299-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a299-116">Application</span></span>|<span data-ttu-id="6a299-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a299-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a299-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a299-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="6a299-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6a299-119">Request headers</span></span>
|<span data-ttu-id="6a299-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6a299-120">Header</span></span>|<span data-ttu-id="6a299-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6a299-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a299-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a299-122">Authorization</span></span>|<span data-ttu-id="6a299-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a299-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a299-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6a299-124">Accept</span></span>|<span data-ttu-id="6a299-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a299-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a299-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6a299-126">Request body</span></span>
<span data-ttu-id="6a299-127">В тексте запроса добавьте представление объекта [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a299-127">In the request body, supply a JSON representation for the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

<span data-ttu-id="6a299-128">В следующей таблице приведены свойства, необходимые при создании [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md).</span><span class="sxs-lookup"><span data-stu-id="6a299-128">The following table shows the properties that are required when you create the [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>

|<span data-ttu-id="6a299-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a299-129">Property</span></span>|<span data-ttu-id="6a299-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6a299-130">Type</span></span>|<span data-ttu-id="6a299-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6a299-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a299-132">id</span><span class="sxs-lookup"><span data-stu-id="6a299-132">id</span></span>|<span data-ttu-id="6a299-133">Строка</span><span class="sxs-lookup"><span data-stu-id="6a299-133">String</span></span>|<span data-ttu-id="6a299-134">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="6a299-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="6a299-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6a299-135">displayName</span></span>|<span data-ttu-id="6a299-136">Строка</span><span class="sxs-lookup"><span data-stu-id="6a299-136">String</span></span>|<span data-ttu-id="6a299-137">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="6a299-137">Name of the device management script.</span></span>|
|<span data-ttu-id="6a299-138">description</span><span class="sxs-lookup"><span data-stu-id="6a299-138">description</span></span>|<span data-ttu-id="6a299-139">String</span><span class="sxs-lookup"><span data-stu-id="6a299-139">String</span></span>|<span data-ttu-id="6a299-140">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="6a299-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="6a299-141">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="6a299-141">scriptContent</span></span>|<span data-ttu-id="6a299-142">Binary</span><span class="sxs-lookup"><span data-stu-id="6a299-142">Binary</span></span>|<span data-ttu-id="6a299-143">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="6a299-143">The script content.</span></span>|
|<span data-ttu-id="6a299-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a299-144">createdDateTime</span></span>|<span data-ttu-id="6a299-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a299-145">DateTimeOffset</span></span>|<span data-ttu-id="6a299-146">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="6a299-146">The date and time the device management script was created.</span></span> <span data-ttu-id="6a299-147">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6a299-147">This property is read-only.</span></span>|
|<span data-ttu-id="6a299-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a299-148">lastModifiedDateTime</span></span>|<span data-ttu-id="6a299-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a299-149">DateTimeOffset</span></span>|<span data-ttu-id="6a299-150">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="6a299-150">The date and time the device management script was last modified.</span></span> <span data-ttu-id="6a299-151">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6a299-151">This property is read-only.</span></span>|
|<span data-ttu-id="6a299-152">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="6a299-152">runAsAccount</span></span>|[<span data-ttu-id="6a299-153">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="6a299-153">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="6a299-154">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="6a299-154">Indicates the type of execution context.</span></span> <span data-ttu-id="6a299-155">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="6a299-155">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="6a299-156">fileName</span><span class="sxs-lookup"><span data-stu-id="6a299-156">fileName</span></span>|<span data-ttu-id="6a299-157">String</span><span class="sxs-lookup"><span data-stu-id="6a299-157">String</span></span>|<span data-ttu-id="6a299-158">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="6a299-158">Script file name.</span></span>|
|<span data-ttu-id="6a299-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6a299-159">roleScopeTagIds</span></span>|<span data-ttu-id="6a299-160">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6a299-160">String collection</span></span>|<span data-ttu-id="6a299-161">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="6a299-161">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="6a299-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a299-162">Response</span></span>
<span data-ttu-id="6a299-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a299-163">If successful, this method returns a `200 OK` response code and an updated [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a299-164">Пример</span><span class="sxs-lookup"><span data-stu-id="6a299-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a299-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a299-165">Request</span></span>
<span data-ttu-id="6a299-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a299-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}
Content-type: application/json
Content-length: 305

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
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

### <a name="response"></a><span data-ttu-id="6a299-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a299-167">Response</span></span>
<span data-ttu-id="6a299-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a299-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 477

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
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





