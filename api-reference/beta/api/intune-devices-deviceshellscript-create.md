---
title: Создание Девицешеллскрипт
description: Создание нового объекта Девицешеллскрипт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 662d0be06b4a714a271e12b1e813aa09f5c76187
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469162"
---
# <a name="create-deviceshellscript"></a><span data-ttu-id="c7da1-103">Создание Девицешеллскрипт</span><span class="sxs-lookup"><span data-stu-id="c7da1-103">Create deviceShellScript</span></span>

<span data-ttu-id="c7da1-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c7da1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7da1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7da1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7da1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7da1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7da1-107">Создание нового объекта [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="c7da1-107">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7da1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c7da1-108">Prerequisites</span></span>
<span data-ttu-id="c7da1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7da1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7da1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7da1-111">Permission type</span></span>|<span data-ttu-id="c7da1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7da1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7da1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7da1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7da1-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7da1-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c7da1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7da1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7da1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7da1-116">Not supported.</span></span>|
|<span data-ttu-id="c7da1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7da1-117">Application</span></span>|<span data-ttu-id="c7da1-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7da1-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7da1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7da1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="c7da1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c7da1-120">Request headers</span></span>
|<span data-ttu-id="c7da1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7da1-121">Header</span></span>|<span data-ttu-id="c7da1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c7da1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7da1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7da1-123">Authorization</span></span>|<span data-ttu-id="c7da1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7da1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7da1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c7da1-125">Accept</span></span>|<span data-ttu-id="c7da1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7da1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7da1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7da1-127">Request body</span></span>
<span data-ttu-id="c7da1-128">В тексте запроса добавьте представление объекта Девицешеллскрипт в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7da1-128">In the request body, supply a JSON representation for the deviceShellScript object.</span></span>

<span data-ttu-id="c7da1-129">В следующей таблице приведены свойства, необходимые при создании Девицешеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="c7da1-129">The following table shows the properties that are required when you create the deviceShellScript.</span></span>

|<span data-ttu-id="c7da1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7da1-130">Property</span></span>|<span data-ttu-id="c7da1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c7da1-131">Type</span></span>|<span data-ttu-id="c7da1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c7da1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7da1-133">id</span><span class="sxs-lookup"><span data-stu-id="c7da1-133">id</span></span>|<span data-ttu-id="c7da1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c7da1-134">String</span></span>|<span data-ttu-id="c7da1-135">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="c7da1-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="c7da1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c7da1-136">displayName</span></span>|<span data-ttu-id="c7da1-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c7da1-137">String</span></span>|<span data-ttu-id="c7da1-138">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="c7da1-138">Name of the device management script.</span></span>|
|<span data-ttu-id="c7da1-139">description</span><span class="sxs-lookup"><span data-stu-id="c7da1-139">description</span></span>|<span data-ttu-id="c7da1-140">String</span><span class="sxs-lookup"><span data-stu-id="c7da1-140">String</span></span>|<span data-ttu-id="c7da1-141">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="c7da1-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="c7da1-142">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="c7da1-142">scriptContent</span></span>|<span data-ttu-id="c7da1-143">Binary</span><span class="sxs-lookup"><span data-stu-id="c7da1-143">Binary</span></span>|<span data-ttu-id="c7da1-144">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="c7da1-144">The script content.</span></span>|
|<span data-ttu-id="c7da1-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7da1-145">createdDateTime</span></span>|<span data-ttu-id="c7da1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7da1-146">DateTimeOffset</span></span>|<span data-ttu-id="c7da1-147">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="c7da1-147">The date and time the device management script was created.</span></span> <span data-ttu-id="c7da1-148">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c7da1-148">This property is read-only.</span></span>|
|<span data-ttu-id="c7da1-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7da1-149">lastModifiedDateTime</span></span>|<span data-ttu-id="c7da1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7da1-150">DateTimeOffset</span></span>|<span data-ttu-id="c7da1-151">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="c7da1-151">The date and time the device management script was last modified.</span></span> <span data-ttu-id="c7da1-152">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c7da1-152">This property is read-only.</span></span>|
|<span data-ttu-id="c7da1-153">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="c7da1-153">runAsAccount</span></span>|[<span data-ttu-id="c7da1-154">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="c7da1-154">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="c7da1-155">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="c7da1-155">Indicates the type of execution context.</span></span> <span data-ttu-id="c7da1-156">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="c7da1-156">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="c7da1-157">fileName</span><span class="sxs-lookup"><span data-stu-id="c7da1-157">fileName</span></span>|<span data-ttu-id="c7da1-158">String</span><span class="sxs-lookup"><span data-stu-id="c7da1-158">String</span></span>|<span data-ttu-id="c7da1-159">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="c7da1-159">Script file name.</span></span>|
|<span data-ttu-id="c7da1-160">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c7da1-160">roleScopeTagIds</span></span>|<span data-ttu-id="c7da1-161">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c7da1-161">String collection</span></span>|<span data-ttu-id="c7da1-162">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="c7da1-162">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="c7da1-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7da1-163">Response</span></span>
<span data-ttu-id="c7da1-164">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7da1-164">If successful, this method returns a `201 Created` response code and a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7da1-165">Пример</span><span class="sxs-lookup"><span data-stu-id="c7da1-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7da1-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7da1-166">Request</span></span>
<span data-ttu-id="c7da1-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7da1-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c7da1-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7da1-168">Response</span></span>
<span data-ttu-id="c7da1-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7da1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





