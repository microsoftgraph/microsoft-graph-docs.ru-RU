---
title: Обновление устройстваCustomAttributeShellScript
description: Обновление свойств объекта deviceCustomAttributeShellScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dfe529650029c27aa03441b2d2c1e90ee6068b56
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150607"
---
# <a name="update-devicecustomattributeshellscript"></a><span data-ttu-id="4a6f6-103">Обновление устройстваCustomAttributeShellScript</span><span class="sxs-lookup"><span data-stu-id="4a6f6-103">Update deviceCustomAttributeShellScript</span></span>

<span data-ttu-id="4a6f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a6f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a6f6-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a6f6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a6f6-107">Обновление свойств объекта [deviceCustomAttributeShellScript.](../resources/intune-devices-devicecustomattributeshellscript.md)</span><span class="sxs-lookup"><span data-stu-id="4a6f6-107">Update the properties of a [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a6f6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4a6f6-108">Prerequisites</span></span>
<span data-ttu-id="4a6f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a6f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a6f6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a6f6-111">Permission type</span></span>|<span data-ttu-id="4a6f6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a6f6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a6f6-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a6f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a6f6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a6f6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4a6f6-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a6f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a6f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-116">Not supported.</span></span>|
|<span data-ttu-id="4a6f6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4a6f6-117">Application</span></span>|<span data-ttu-id="4a6f6-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a6f6-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a6f6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a6f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="4a6f6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4a6f6-120">Request headers</span></span>
|<span data-ttu-id="4a6f6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a6f6-121">Header</span></span>|<span data-ttu-id="4a6f6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4a6f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a6f6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a6f6-123">Authorization</span></span>|<span data-ttu-id="4a6f6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a6f6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4a6f6-125">Accept</span></span>|<span data-ttu-id="4a6f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a6f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a6f6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a6f6-127">Request body</span></span>
<span data-ttu-id="4a6f6-128">В теле запроса поставляем представление JSON для [объекта deviceCustomAttributeShellScript.](../resources/intune-devices-devicecustomattributeshellscript.md)</span><span class="sxs-lookup"><span data-stu-id="4a6f6-128">In the request body, supply a JSON representation for the [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object.</span></span>

<span data-ttu-id="4a6f6-129">В следующей таблице показаны свойства, необходимые при создании [устройстваCustomAttributeShellScript.](../resources/intune-devices-devicecustomattributeshellscript.md)</span><span class="sxs-lookup"><span data-stu-id="4a6f6-129">The following table shows the properties that are required when you create the [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md).</span></span>

|<span data-ttu-id="4a6f6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a6f6-130">Property</span></span>|<span data-ttu-id="4a6f6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4a6f6-131">Type</span></span>|<span data-ttu-id="4a6f6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4a6f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a6f6-133">id</span><span class="sxs-lookup"><span data-stu-id="4a6f6-133">id</span></span>|<span data-ttu-id="4a6f6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4a6f6-134">String</span></span>|<span data-ttu-id="4a6f6-135">Уникальный идентификатор для настраиваемого объекта атрибута.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-135">Unique Identifier for the custom attribute entity.</span></span>|
|<span data-ttu-id="4a6f6-136">customAttributeName</span><span class="sxs-lookup"><span data-stu-id="4a6f6-136">customAttributeName</span></span>|<span data-ttu-id="4a6f6-137">Строка</span><span class="sxs-lookup"><span data-stu-id="4a6f6-137">String</span></span>|<span data-ttu-id="4a6f6-138">Имя настраиваемого атрибута.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-138">The name of the custom attribute.</span></span>|
|<span data-ttu-id="4a6f6-139">customAttributeType</span><span class="sxs-lookup"><span data-stu-id="4a6f6-139">customAttributeType</span></span>|[<span data-ttu-id="4a6f6-140">deviceCustomAttributeValueType</span><span class="sxs-lookup"><span data-stu-id="4a6f6-140">deviceCustomAttributeValueType</span></span>](../resources/intune-devices-devicecustomattributevaluetype.md)|<span data-ttu-id="4a6f6-141">Ожидаемый тип значения настраиваемого атрибута.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-141">The expected type of the custom attribute's value.</span></span> <span data-ttu-id="4a6f6-142">Возможные значения: `integer`, `string`, `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-142">Possible values are: `integer`, `string`, `dateTime`.</span></span>|
|<span data-ttu-id="4a6f6-143">displayName</span><span class="sxs-lookup"><span data-stu-id="4a6f6-143">displayName</span></span>|<span data-ttu-id="4a6f6-144">Строка</span><span class="sxs-lookup"><span data-stu-id="4a6f6-144">String</span></span>|<span data-ttu-id="4a6f6-145">Имя сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-145">Name of the device management script.</span></span>|
|<span data-ttu-id="4a6f6-146">description</span><span class="sxs-lookup"><span data-stu-id="4a6f6-146">description</span></span>|<span data-ttu-id="4a6f6-147">Строка</span><span class="sxs-lookup"><span data-stu-id="4a6f6-147">String</span></span>|<span data-ttu-id="4a6f6-148">Необязательное описание сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-148">Optional description for the device management script.</span></span>|
|<span data-ttu-id="4a6f6-149">scriptContent</span><span class="sxs-lookup"><span data-stu-id="4a6f6-149">scriptContent</span></span>|<span data-ttu-id="4a6f6-150">Binary</span><span class="sxs-lookup"><span data-stu-id="4a6f6-150">Binary</span></span>|<span data-ttu-id="4a6f6-151">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-151">The script content.</span></span>|
|<span data-ttu-id="4a6f6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a6f6-152">createdDateTime</span></span>|<span data-ttu-id="4a6f6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a6f6-153">DateTimeOffset</span></span>|<span data-ttu-id="4a6f6-154">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-154">The date and time the device management script was created.</span></span> <span data-ttu-id="4a6f6-155">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-155">This property is read-only.</span></span>|
|<span data-ttu-id="4a6f6-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a6f6-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4a6f6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a6f6-157">DateTimeOffset</span></span>|<span data-ttu-id="4a6f6-158">Дата и время последнего изменения сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-158">The date and time the device management script was last modified.</span></span> <span data-ttu-id="4a6f6-159">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-159">This property is read-only.</span></span>|
|<span data-ttu-id="4a6f6-160">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="4a6f6-160">runAsAccount</span></span>|[<span data-ttu-id="4a6f6-161">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="4a6f6-161">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="4a6f6-162">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-162">Indicates the type of execution context.</span></span> <span data-ttu-id="4a6f6-163">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-163">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="4a6f6-164">fileName</span><span class="sxs-lookup"><span data-stu-id="4a6f6-164">fileName</span></span>|<span data-ttu-id="4a6f6-165">String</span><span class="sxs-lookup"><span data-stu-id="4a6f6-165">String</span></span>|<span data-ttu-id="4a6f6-166">Имя файла скрипта.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-166">Script file name.</span></span>|
|<span data-ttu-id="4a6f6-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4a6f6-167">roleScopeTagIds</span></span>|<span data-ttu-id="4a6f6-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4a6f6-168">String collection</span></span>|<span data-ttu-id="4a6f6-169">Список ID-тегов области для этого экземпляра PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-169">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="4a6f6-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a6f6-170">Response</span></span>
<span data-ttu-id="4a6f6-171">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-171">If successful, this method returns a `200 OK` response code and an updated [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a6f6-172">Пример</span><span class="sxs-lookup"><span data-stu-id="4a6f6-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a6f6-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a6f6-173">Request</span></span>
<span data-ttu-id="4a6f6-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4a6f6-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a6f6-175">Response</span></span>
<span data-ttu-id="4a6f6-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a6f6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




