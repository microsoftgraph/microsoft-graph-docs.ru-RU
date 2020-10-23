---
title: Создание Девицекустоматтрибутешеллскрипт
description: Создание нового объекта Девицекустоматтрибутешеллскрипт.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba72710bfeec5d0b5549837eff0fec4d2bed5510
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705122"
---
# <a name="create-devicecustomattributeshellscript"></a><span data-ttu-id="68804-103">Создание Девицекустоматтрибутешеллскрипт</span><span class="sxs-lookup"><span data-stu-id="68804-103">Create deviceCustomAttributeShellScript</span></span>

<span data-ttu-id="68804-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68804-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68804-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68804-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68804-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68804-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68804-107">Создание нового объекта [девицекустоматтрибутешеллскрипт](../resources/intune-devices-devicecustomattributeshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="68804-107">Create a new [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68804-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="68804-108">Prerequisites</span></span>
<span data-ttu-id="68804-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68804-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68804-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68804-111">Permission type</span></span>|<span data-ttu-id="68804-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68804-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68804-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68804-113">Delegated (work or school account)</span></span>|<span data-ttu-id="68804-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68804-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="68804-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68804-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68804-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68804-116">Not supported.</span></span>|
|<span data-ttu-id="68804-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68804-117">Application</span></span>|<span data-ttu-id="68804-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68804-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68804-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68804-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCustomAttributeShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="68804-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="68804-120">Request headers</span></span>
|<span data-ttu-id="68804-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68804-121">Header</span></span>|<span data-ttu-id="68804-122">Значение</span><span class="sxs-lookup"><span data-stu-id="68804-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68804-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68804-123">Authorization</span></span>|<span data-ttu-id="68804-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68804-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68804-125">Accept</span><span class="sxs-lookup"><span data-stu-id="68804-125">Accept</span></span>|<span data-ttu-id="68804-126">application/json</span><span class="sxs-lookup"><span data-stu-id="68804-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68804-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="68804-127">Request body</span></span>
<span data-ttu-id="68804-128">В тексте запроса добавьте представление объекта Девицекустоматтрибутешеллскрипт в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68804-128">In the request body, supply a JSON representation for the deviceCustomAttributeShellScript object.</span></span>

<span data-ttu-id="68804-129">В следующей таблице приведены свойства, необходимые при создании Девицекустоматтрибутешеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="68804-129">The following table shows the properties that are required when you create the deviceCustomAttributeShellScript.</span></span>

|<span data-ttu-id="68804-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="68804-130">Property</span></span>|<span data-ttu-id="68804-131">Тип</span><span class="sxs-lookup"><span data-stu-id="68804-131">Type</span></span>|<span data-ttu-id="68804-132">Описание</span><span class="sxs-lookup"><span data-stu-id="68804-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68804-133">id</span><span class="sxs-lookup"><span data-stu-id="68804-133">id</span></span>|<span data-ttu-id="68804-134">Строка</span><span class="sxs-lookup"><span data-stu-id="68804-134">String</span></span>|<span data-ttu-id="68804-135">Уникальный идентификатор для объекта настраиваемого атрибута.</span><span class="sxs-lookup"><span data-stu-id="68804-135">Unique Identifier for the custom attribute entity.</span></span>|
|<span data-ttu-id="68804-136">кустоматтрибутенаме</span><span class="sxs-lookup"><span data-stu-id="68804-136">customAttributeName</span></span>|<span data-ttu-id="68804-137">Строка</span><span class="sxs-lookup"><span data-stu-id="68804-137">String</span></span>|<span data-ttu-id="68804-138">Имя настраиваемого атрибута.</span><span class="sxs-lookup"><span data-stu-id="68804-138">The name of the custom attribute.</span></span>|
|<span data-ttu-id="68804-139">кустоматтрибутетипе</span><span class="sxs-lookup"><span data-stu-id="68804-139">customAttributeType</span></span>|[<span data-ttu-id="68804-140">девицекустоматтрибутевалуетипе</span><span class="sxs-lookup"><span data-stu-id="68804-140">deviceCustomAttributeValueType</span></span>](../resources/intune-devices-devicecustomattributevaluetype.md)|<span data-ttu-id="68804-141">Ожидаемый тип значения настраиваемого атрибута.</span><span class="sxs-lookup"><span data-stu-id="68804-141">The expected type of the custom attribute's value.</span></span> <span data-ttu-id="68804-142">Возможные значения: `integer`, `string`, `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="68804-142">Possible values are: `integer`, `string`, `dateTime`.</span></span>|
|<span data-ttu-id="68804-143">displayName</span><span class="sxs-lookup"><span data-stu-id="68804-143">displayName</span></span>|<span data-ttu-id="68804-144">Строка</span><span class="sxs-lookup"><span data-stu-id="68804-144">String</span></span>|<span data-ttu-id="68804-145">Имя скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="68804-145">Name of the device management script.</span></span>|
|<span data-ttu-id="68804-146">description</span><span class="sxs-lookup"><span data-stu-id="68804-146">description</span></span>|<span data-ttu-id="68804-147">Строка</span><span class="sxs-lookup"><span data-stu-id="68804-147">String</span></span>|<span data-ttu-id="68804-148">Необязательное описание скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="68804-148">Optional description for the device management script.</span></span>|
|<span data-ttu-id="68804-149">скриптконтент</span><span class="sxs-lookup"><span data-stu-id="68804-149">scriptContent</span></span>|<span data-ttu-id="68804-150">Binary</span><span class="sxs-lookup"><span data-stu-id="68804-150">Binary</span></span>|<span data-ttu-id="68804-151">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="68804-151">The script content.</span></span>|
|<span data-ttu-id="68804-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="68804-152">createdDateTime</span></span>|<span data-ttu-id="68804-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68804-153">DateTimeOffset</span></span>|<span data-ttu-id="68804-154">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="68804-154">The date and time the device management script was created.</span></span> <span data-ttu-id="68804-155">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68804-155">This property is read-only.</span></span>|
|<span data-ttu-id="68804-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68804-156">lastModifiedDateTime</span></span>|<span data-ttu-id="68804-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68804-157">DateTimeOffset</span></span>|<span data-ttu-id="68804-158">Дата и время последнего изменения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="68804-158">The date and time the device management script was last modified.</span></span> <span data-ttu-id="68804-159">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68804-159">This property is read-only.</span></span>|
|<span data-ttu-id="68804-160">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="68804-160">runAsAccount</span></span>|[<span data-ttu-id="68804-161">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="68804-161">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="68804-162">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="68804-162">Indicates the type of execution context.</span></span> <span data-ttu-id="68804-163">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="68804-163">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="68804-164">fileName</span><span class="sxs-lookup"><span data-stu-id="68804-164">fileName</span></span>|<span data-ttu-id="68804-165">String</span><span class="sxs-lookup"><span data-stu-id="68804-165">String</span></span>|<span data-ttu-id="68804-166">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="68804-166">Script file name.</span></span>|
|<span data-ttu-id="68804-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="68804-167">roleScopeTagIds</span></span>|<span data-ttu-id="68804-168">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="68804-168">String collection</span></span>|<span data-ttu-id="68804-169">Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.</span><span class="sxs-lookup"><span data-stu-id="68804-169">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="68804-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="68804-170">Response</span></span>
<span data-ttu-id="68804-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицекустоматтрибутешеллскрипт](../resources/intune-devices-devicecustomattributeshellscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68804-171">If successful, this method returns a `201 Created` response code and a [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68804-172">Пример</span><span class="sxs-lookup"><span data-stu-id="68804-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="68804-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="68804-173">Request</span></span>
<span data-ttu-id="68804-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68804-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCustomAttributeShellScripts
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

### <a name="response"></a><span data-ttu-id="68804-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="68804-175">Response</span></span>
<span data-ttu-id="68804-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68804-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





