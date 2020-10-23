---
title: Обновление Девицекустоматтрибутешеллскрипт
description: Обновление свойств объекта Девицекустоматтрибутешеллскрипт.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aa48958a27c44f924f627ea5d133cc34b74804a1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704986"
---
# <a name="update-devicecustomattributeshellscript"></a><span data-ttu-id="3ff82-103">Обновление Девицекустоматтрибутешеллскрипт</span><span class="sxs-lookup"><span data-stu-id="3ff82-103">Update deviceCustomAttributeShellScript</span></span>

<span data-ttu-id="3ff82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ff82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ff82-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ff82-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ff82-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ff82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ff82-107">Обновление свойств объекта [девицекустоматтрибутешеллскрипт](../resources/intune-devices-devicecustomattributeshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="3ff82-107">Update the properties of a [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ff82-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3ff82-108">Prerequisites</span></span>
<span data-ttu-id="3ff82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ff82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ff82-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ff82-111">Permission type</span></span>|<span data-ttu-id="3ff82-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ff82-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ff82-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ff82-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ff82-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ff82-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3ff82-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ff82-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ff82-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ff82-116">Not supported.</span></span>|
|<span data-ttu-id="3ff82-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ff82-117">Application</span></span>|<span data-ttu-id="3ff82-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ff82-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ff82-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ff82-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="3ff82-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3ff82-120">Request headers</span></span>
|<span data-ttu-id="3ff82-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ff82-121">Header</span></span>|<span data-ttu-id="3ff82-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3ff82-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ff82-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ff82-123">Authorization</span></span>|<span data-ttu-id="3ff82-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ff82-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ff82-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3ff82-125">Accept</span></span>|<span data-ttu-id="3ff82-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ff82-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ff82-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3ff82-127">Request body</span></span>
<span data-ttu-id="3ff82-128">В тексте запроса добавьте представление объекта [девицекустоматтрибутешеллскрипт](../resources/intune-devices-devicecustomattributeshellscript.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ff82-128">In the request body, supply a JSON representation for the [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object.</span></span>

<span data-ttu-id="3ff82-129">В следующей таблице приведены свойства, необходимые при создании [девицекустоматтрибутешеллскрипт](../resources/intune-devices-devicecustomattributeshellscript.md).</span><span class="sxs-lookup"><span data-stu-id="3ff82-129">The following table shows the properties that are required when you create the [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md).</span></span>

|<span data-ttu-id="3ff82-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ff82-130">Property</span></span>|<span data-ttu-id="3ff82-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3ff82-131">Type</span></span>|<span data-ttu-id="3ff82-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3ff82-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ff82-133">id</span><span class="sxs-lookup"><span data-stu-id="3ff82-133">id</span></span>|<span data-ttu-id="3ff82-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3ff82-134">String</span></span>|<span data-ttu-id="3ff82-135">Уникальный идентификатор для объекта настраиваемого атрибута.</span><span class="sxs-lookup"><span data-stu-id="3ff82-135">Unique Identifier for the custom attribute entity.</span></span>|
|<span data-ttu-id="3ff82-136">кустоматтрибутенаме</span><span class="sxs-lookup"><span data-stu-id="3ff82-136">customAttributeName</span></span>|<span data-ttu-id="3ff82-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3ff82-137">String</span></span>|<span data-ttu-id="3ff82-138">Имя настраиваемого атрибута.</span><span class="sxs-lookup"><span data-stu-id="3ff82-138">The name of the custom attribute.</span></span>|
|<span data-ttu-id="3ff82-139">кустоматтрибутетипе</span><span class="sxs-lookup"><span data-stu-id="3ff82-139">customAttributeType</span></span>|[<span data-ttu-id="3ff82-140">девицекустоматтрибутевалуетипе</span><span class="sxs-lookup"><span data-stu-id="3ff82-140">deviceCustomAttributeValueType</span></span>](../resources/intune-devices-devicecustomattributevaluetype.md)|<span data-ttu-id="3ff82-141">Ожидаемый тип значения настраиваемого атрибута.</span><span class="sxs-lookup"><span data-stu-id="3ff82-141">The expected type of the custom attribute's value.</span></span> <span data-ttu-id="3ff82-142">Возможные значения: `integer`, `string`, `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="3ff82-142">Possible values are: `integer`, `string`, `dateTime`.</span></span>|
|<span data-ttu-id="3ff82-143">displayName</span><span class="sxs-lookup"><span data-stu-id="3ff82-143">displayName</span></span>|<span data-ttu-id="3ff82-144">Строка</span><span class="sxs-lookup"><span data-stu-id="3ff82-144">String</span></span>|<span data-ttu-id="3ff82-145">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="3ff82-145">Name of the device management script.</span></span>|
|<span data-ttu-id="3ff82-146">description</span><span class="sxs-lookup"><span data-stu-id="3ff82-146">description</span></span>|<span data-ttu-id="3ff82-147">Строка</span><span class="sxs-lookup"><span data-stu-id="3ff82-147">String</span></span>|<span data-ttu-id="3ff82-148">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="3ff82-148">Optional description for the device management script.</span></span>|
|<span data-ttu-id="3ff82-149">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="3ff82-149">scriptContent</span></span>|<span data-ttu-id="3ff82-150">Binary</span><span class="sxs-lookup"><span data-stu-id="3ff82-150">Binary</span></span>|<span data-ttu-id="3ff82-151">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="3ff82-151">The script content.</span></span>|
|<span data-ttu-id="3ff82-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ff82-152">createdDateTime</span></span>|<span data-ttu-id="3ff82-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ff82-153">DateTimeOffset</span></span>|<span data-ttu-id="3ff82-154">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="3ff82-154">The date and time the device management script was created.</span></span> <span data-ttu-id="3ff82-155">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ff82-155">This property is read-only.</span></span>|
|<span data-ttu-id="3ff82-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ff82-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3ff82-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ff82-157">DateTimeOffset</span></span>|<span data-ttu-id="3ff82-158">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="3ff82-158">The date and time the device management script was last modified.</span></span> <span data-ttu-id="3ff82-159">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ff82-159">This property is read-only.</span></span>|
|<span data-ttu-id="3ff82-160">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="3ff82-160">runAsAccount</span></span>|[<span data-ttu-id="3ff82-161">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="3ff82-161">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="3ff82-162">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="3ff82-162">Indicates the type of execution context.</span></span> <span data-ttu-id="3ff82-163">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="3ff82-163">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="3ff82-164">fileName</span><span class="sxs-lookup"><span data-stu-id="3ff82-164">fileName</span></span>|<span data-ttu-id="3ff82-165">String</span><span class="sxs-lookup"><span data-stu-id="3ff82-165">String</span></span>|<span data-ttu-id="3ff82-166">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="3ff82-166">Script file name.</span></span>|
|<span data-ttu-id="3ff82-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3ff82-167">roleScopeTagIds</span></span>|<span data-ttu-id="3ff82-168">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3ff82-168">String collection</span></span>|<span data-ttu-id="3ff82-169">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="3ff82-169">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="3ff82-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ff82-170">Response</span></span>
<span data-ttu-id="3ff82-171">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицекустоматтрибутешеллскрипт](../resources/intune-devices-devicecustomattributeshellscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3ff82-171">If successful, this method returns a `200 OK` response code and an updated [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ff82-172">Пример</span><span class="sxs-lookup"><span data-stu-id="3ff82-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ff82-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ff82-173">Request</span></span>
<span data-ttu-id="3ff82-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ff82-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}
Content-type: application/json
Content-length: 413

{
  "@odata.type": "#microsoft.graph.deviceCustomAttributeShellScript",
  "customAttributeName": "Custom Attribute Name value",
  "customAttributeType": "string",
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

### <a name="response"></a><span data-ttu-id="3ff82-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ff82-175">Response</span></span>
<span data-ttu-id="3ff82-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ff82-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 585

{
  "@odata.type": "#microsoft.graph.deviceCustomAttributeShellScript",
  "id": "929d921b-921b-929d-1b92-9d921b929d92",
  "customAttributeName": "Custom Attribute Name value",
  "customAttributeType": "string",
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





