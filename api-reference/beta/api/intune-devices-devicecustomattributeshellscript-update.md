---
title: Обновление Девицекустоматтрибутешеллскрипт
description: Обновление свойств объекта Девицекустоматтрибутешеллскрипт.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e3a1680e8949ff85e156cb55bd0d68f3a79f8b62
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49235184"
---
# <a name="update-devicecustomattributeshellscript"></a><span data-ttu-id="8ce05-103">Обновление Девицекустоматтрибутешеллскрипт</span><span class="sxs-lookup"><span data-stu-id="8ce05-103">Update deviceCustomAttributeShellScript</span></span>

<span data-ttu-id="8ce05-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ce05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ce05-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ce05-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ce05-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ce05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ce05-107">Обновление свойств объекта [девицекустоматтрибутешеллскрипт](../resources/intune-devices-devicecustomattributeshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="8ce05-107">Update the properties of a [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ce05-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8ce05-108">Prerequisites</span></span>
<span data-ttu-id="8ce05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ce05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ce05-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ce05-111">Permission type</span></span>|<span data-ttu-id="8ce05-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ce05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ce05-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ce05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ce05-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ce05-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8ce05-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ce05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ce05-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ce05-116">Not supported.</span></span>|
|<span data-ttu-id="8ce05-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8ce05-117">Application</span></span>|<span data-ttu-id="8ce05-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ce05-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ce05-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ce05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="8ce05-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8ce05-120">Request headers</span></span>
|<span data-ttu-id="8ce05-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ce05-121">Header</span></span>|<span data-ttu-id="8ce05-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8ce05-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ce05-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ce05-123">Authorization</span></span>|<span data-ttu-id="8ce05-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ce05-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ce05-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8ce05-125">Accept</span></span>|<span data-ttu-id="8ce05-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ce05-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ce05-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ce05-127">Request body</span></span>
<span data-ttu-id="8ce05-128">В тексте запроса добавьте представление объекта [девицекустоматтрибутешеллскрипт](../resources/intune-devices-devicecustomattributeshellscript.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ce05-128">In the request body, supply a JSON representation for the [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object.</span></span>

<span data-ttu-id="8ce05-129">В следующей таблице приведены свойства, необходимые при создании [девицекустоматтрибутешеллскрипт](../resources/intune-devices-devicecustomattributeshellscript.md).</span><span class="sxs-lookup"><span data-stu-id="8ce05-129">The following table shows the properties that are required when you create the [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md).</span></span>

|<span data-ttu-id="8ce05-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ce05-130">Property</span></span>|<span data-ttu-id="8ce05-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8ce05-131">Type</span></span>|<span data-ttu-id="8ce05-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8ce05-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ce05-133">id</span><span class="sxs-lookup"><span data-stu-id="8ce05-133">id</span></span>|<span data-ttu-id="8ce05-134">String</span><span class="sxs-lookup"><span data-stu-id="8ce05-134">String</span></span>|<span data-ttu-id="8ce05-135">Уникальный идентификатор для объекта настраиваемого атрибута.</span><span class="sxs-lookup"><span data-stu-id="8ce05-135">Unique Identifier for the custom attribute entity.</span></span>|
|<span data-ttu-id="8ce05-136">кустоматтрибутенаме</span><span class="sxs-lookup"><span data-stu-id="8ce05-136">customAttributeName</span></span>|<span data-ttu-id="8ce05-137">String</span><span class="sxs-lookup"><span data-stu-id="8ce05-137">String</span></span>|<span data-ttu-id="8ce05-138">Имя настраиваемого атрибута.</span><span class="sxs-lookup"><span data-stu-id="8ce05-138">The name of the custom attribute.</span></span>|
|<span data-ttu-id="8ce05-139">кустоматтрибутетипе</span><span class="sxs-lookup"><span data-stu-id="8ce05-139">customAttributeType</span></span>|[<span data-ttu-id="8ce05-140">deviceCustomAttributeValueType</span><span class="sxs-lookup"><span data-stu-id="8ce05-140">deviceCustomAttributeValueType</span></span>](../resources/intune-devices-devicecustomattributevaluetype.md)|<span data-ttu-id="8ce05-141">Ожидаемый тип значения настраиваемого атрибута.</span><span class="sxs-lookup"><span data-stu-id="8ce05-141">The expected type of the custom attribute's value.</span></span> <span data-ttu-id="8ce05-142">Возможные значения: `integer`, `string`, `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="8ce05-142">Possible values are: `integer`, `string`, `dateTime`.</span></span>|
|<span data-ttu-id="8ce05-143">displayName</span><span class="sxs-lookup"><span data-stu-id="8ce05-143">displayName</span></span>|<span data-ttu-id="8ce05-144">String</span><span class="sxs-lookup"><span data-stu-id="8ce05-144">String</span></span>|<span data-ttu-id="8ce05-145">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="8ce05-145">Name of the device management script.</span></span>|
|<span data-ttu-id="8ce05-146">description</span><span class="sxs-lookup"><span data-stu-id="8ce05-146">description</span></span>|<span data-ttu-id="8ce05-147">String</span><span class="sxs-lookup"><span data-stu-id="8ce05-147">String</span></span>|<span data-ttu-id="8ce05-148">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="8ce05-148">Optional description for the device management script.</span></span>|
|<span data-ttu-id="8ce05-149">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="8ce05-149">scriptContent</span></span>|<span data-ttu-id="8ce05-150">Binary</span><span class="sxs-lookup"><span data-stu-id="8ce05-150">Binary</span></span>|<span data-ttu-id="8ce05-151">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="8ce05-151">The script content.</span></span>|
|<span data-ttu-id="8ce05-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ce05-152">createdDateTime</span></span>|<span data-ttu-id="8ce05-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ce05-153">DateTimeOffset</span></span>|<span data-ttu-id="8ce05-154">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="8ce05-154">The date and time the device management script was created.</span></span> <span data-ttu-id="8ce05-155">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ce05-155">This property is read-only.</span></span>|
|<span data-ttu-id="8ce05-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ce05-156">lastModifiedDateTime</span></span>|<span data-ttu-id="8ce05-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ce05-157">DateTimeOffset</span></span>|<span data-ttu-id="8ce05-158">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="8ce05-158">The date and time the device management script was last modified.</span></span> <span data-ttu-id="8ce05-159">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ce05-159">This property is read-only.</span></span>|
|<span data-ttu-id="8ce05-160">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="8ce05-160">runAsAccount</span></span>|[<span data-ttu-id="8ce05-161">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="8ce05-161">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="8ce05-162">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="8ce05-162">Indicates the type of execution context.</span></span> <span data-ttu-id="8ce05-163">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="8ce05-163">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="8ce05-164">fileName</span><span class="sxs-lookup"><span data-stu-id="8ce05-164">fileName</span></span>|<span data-ttu-id="8ce05-165">String</span><span class="sxs-lookup"><span data-stu-id="8ce05-165">String</span></span>|<span data-ttu-id="8ce05-166">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="8ce05-166">Script file name.</span></span>|
|<span data-ttu-id="8ce05-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8ce05-167">roleScopeTagIds</span></span>|<span data-ttu-id="8ce05-168">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8ce05-168">String collection</span></span>|<span data-ttu-id="8ce05-169">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="8ce05-169">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="8ce05-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ce05-170">Response</span></span>
<span data-ttu-id="8ce05-171">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицекустоматтрибутешеллскрипт](../resources/intune-devices-devicecustomattributeshellscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ce05-171">If successful, this method returns a `200 OK` response code and an updated [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ce05-172">Пример</span><span class="sxs-lookup"><span data-stu-id="8ce05-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ce05-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ce05-173">Request</span></span>
<span data-ttu-id="8ce05-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ce05-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8ce05-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ce05-175">Response</span></span>
<span data-ttu-id="8ce05-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ce05-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




