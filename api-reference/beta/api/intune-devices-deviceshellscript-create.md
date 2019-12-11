---
title: Создание Девицешеллскрипт
description: Создание нового объекта Девицешеллскрипт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 37e2777d766335d0d8ddade5eba1ea889b535113
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944864"
---
# <a name="create-deviceshellscript"></a><span data-ttu-id="be616-103">Создание Девицешеллскрипт</span><span class="sxs-lookup"><span data-stu-id="be616-103">Create deviceShellScript</span></span>

> <span data-ttu-id="be616-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be616-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be616-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be616-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be616-106">Создание нового объекта [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="be616-106">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be616-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="be616-107">Prerequisites</span></span>
<span data-ttu-id="be616-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be616-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be616-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be616-110">Permission type</span></span>|<span data-ttu-id="be616-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be616-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be616-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be616-112">Delegated (work or school account)</span></span>|<span data-ttu-id="be616-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be616-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="be616-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be616-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be616-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be616-115">Not supported.</span></span>|
|<span data-ttu-id="be616-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be616-116">Application</span></span>|<span data-ttu-id="be616-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be616-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be616-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be616-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="be616-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="be616-119">Request headers</span></span>
|<span data-ttu-id="be616-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be616-120">Header</span></span>|<span data-ttu-id="be616-121">Значение</span><span class="sxs-lookup"><span data-stu-id="be616-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be616-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be616-122">Authorization</span></span>|<span data-ttu-id="be616-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be616-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be616-124">Accept</span><span class="sxs-lookup"><span data-stu-id="be616-124">Accept</span></span>|<span data-ttu-id="be616-125">application/json</span><span class="sxs-lookup"><span data-stu-id="be616-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be616-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be616-126">Request body</span></span>
<span data-ttu-id="be616-127">В тексте запроса добавьте представление объекта Девицешеллскрипт в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be616-127">In the request body, supply a JSON representation for the deviceShellScript object.</span></span>

<span data-ttu-id="be616-128">В следующей таблице приведены свойства, необходимые при создании Девицешеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="be616-128">The following table shows the properties that are required when you create the deviceShellScript.</span></span>

|<span data-ttu-id="be616-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="be616-129">Property</span></span>|<span data-ttu-id="be616-130">Тип</span><span class="sxs-lookup"><span data-stu-id="be616-130">Type</span></span>|<span data-ttu-id="be616-131">Описание</span><span class="sxs-lookup"><span data-stu-id="be616-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be616-132">id</span><span class="sxs-lookup"><span data-stu-id="be616-132">id</span></span>|<span data-ttu-id="be616-133">Строка</span><span class="sxs-lookup"><span data-stu-id="be616-133">String</span></span>|<span data-ttu-id="be616-134">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="be616-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="be616-135">displayName</span><span class="sxs-lookup"><span data-stu-id="be616-135">displayName</span></span>|<span data-ttu-id="be616-136">Строка</span><span class="sxs-lookup"><span data-stu-id="be616-136">String</span></span>|<span data-ttu-id="be616-137">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="be616-137">Name of the device management script.</span></span>|
|<span data-ttu-id="be616-138">description</span><span class="sxs-lookup"><span data-stu-id="be616-138">description</span></span>|<span data-ttu-id="be616-139">String</span><span class="sxs-lookup"><span data-stu-id="be616-139">String</span></span>|<span data-ttu-id="be616-140">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="be616-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="be616-141">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="be616-141">scriptContent</span></span>|<span data-ttu-id="be616-142">Binary</span><span class="sxs-lookup"><span data-stu-id="be616-142">Binary</span></span>|<span data-ttu-id="be616-143">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="be616-143">The script content.</span></span>|
|<span data-ttu-id="be616-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be616-144">createdDateTime</span></span>|<span data-ttu-id="be616-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be616-145">DateTimeOffset</span></span>|<span data-ttu-id="be616-146">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="be616-146">The date and time the device management script was created.</span></span> <span data-ttu-id="be616-147">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="be616-147">This property is read-only.</span></span>|
|<span data-ttu-id="be616-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be616-148">lastModifiedDateTime</span></span>|<span data-ttu-id="be616-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be616-149">DateTimeOffset</span></span>|<span data-ttu-id="be616-150">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="be616-150">The date and time the device management script was last modified.</span></span> <span data-ttu-id="be616-151">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="be616-151">This property is read-only.</span></span>|
|<span data-ttu-id="be616-152">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="be616-152">runAsAccount</span></span>|[<span data-ttu-id="be616-153">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="be616-153">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="be616-154">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="be616-154">Indicates the type of execution context.</span></span> <span data-ttu-id="be616-155">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="be616-155">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="be616-156">fileName</span><span class="sxs-lookup"><span data-stu-id="be616-156">fileName</span></span>|<span data-ttu-id="be616-157">String</span><span class="sxs-lookup"><span data-stu-id="be616-157">String</span></span>|<span data-ttu-id="be616-158">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="be616-158">Script file name.</span></span>|
|<span data-ttu-id="be616-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="be616-159">roleScopeTagIds</span></span>|<span data-ttu-id="be616-160">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="be616-160">String collection</span></span>|<span data-ttu-id="be616-161">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="be616-161">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="be616-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="be616-162">Response</span></span>
<span data-ttu-id="be616-163">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be616-163">If successful, this method returns a `201 Created` response code and a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be616-164">Пример</span><span class="sxs-lookup"><span data-stu-id="be616-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="be616-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="be616-165">Request</span></span>
<span data-ttu-id="be616-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be616-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts
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

### <a name="response"></a><span data-ttu-id="be616-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="be616-167">Response</span></span>
<span data-ttu-id="be616-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be616-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





