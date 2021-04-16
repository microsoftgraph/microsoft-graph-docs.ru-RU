---
title: Создание deviceManagementScript
description: Создание нового объекта deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d077f34cef3c75680c48229680c76f0a045694c9
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867814"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="d411c-103">Создание deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="d411c-103">Create deviceManagementScript</span></span>

<span data-ttu-id="d411c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d411c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d411c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d411c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d411c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d411c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d411c-107">Создание нового [объекта deviceManagementScript.](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="d411c-107">Create a new [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d411c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d411c-108">Prerequisites</span></span>
<span data-ttu-id="d411c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d411c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d411c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d411c-111">Permission type</span></span>|<span data-ttu-id="d411c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d411c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d411c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d411c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d411c-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d411c-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d411c-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d411c-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="d411c-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d411c-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d411c-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d411c-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d411c-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d411c-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d411c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d411c-119">Not supported.</span></span>|
|<span data-ttu-id="d411c-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d411c-120">Application</span></span>||
| <span data-ttu-id="d411c-121">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="d411c-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d411c-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d411c-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="d411c-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="d411c-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="d411c-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d411c-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d411c-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d411c-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="d411c-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d411c-126">Request headers</span></span>
|<span data-ttu-id="d411c-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d411c-127">Header</span></span>|<span data-ttu-id="d411c-128">Значение</span><span class="sxs-lookup"><span data-stu-id="d411c-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d411c-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d411c-129">Authorization</span></span>|<span data-ttu-id="d411c-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d411c-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d411c-131">Accept</span><span class="sxs-lookup"><span data-stu-id="d411c-131">Accept</span></span>|<span data-ttu-id="d411c-132">application/json</span><span class="sxs-lookup"><span data-stu-id="d411c-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d411c-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d411c-133">Request body</span></span>
<span data-ttu-id="d411c-134">В теле запроса поставляем представление JSON для объекта deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="d411c-134">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="d411c-135">В следующей таблице показаны свойства, необходимые при создании deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="d411c-135">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="d411c-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="d411c-136">Property</span></span>|<span data-ttu-id="d411c-137">Тип</span><span class="sxs-lookup"><span data-stu-id="d411c-137">Type</span></span>|<span data-ttu-id="d411c-138">Описание</span><span class="sxs-lookup"><span data-stu-id="d411c-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d411c-139">id</span><span class="sxs-lookup"><span data-stu-id="d411c-139">id</span></span>|<span data-ttu-id="d411c-140">String</span><span class="sxs-lookup"><span data-stu-id="d411c-140">String</span></span>|<span data-ttu-id="d411c-141">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="d411c-141">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="d411c-142">displayName</span><span class="sxs-lookup"><span data-stu-id="d411c-142">displayName</span></span>|<span data-ttu-id="d411c-143">String</span><span class="sxs-lookup"><span data-stu-id="d411c-143">String</span></span>|<span data-ttu-id="d411c-144">Имя сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="d411c-144">Name of the device management script.</span></span>|
|<span data-ttu-id="d411c-145">description</span><span class="sxs-lookup"><span data-stu-id="d411c-145">description</span></span>|<span data-ttu-id="d411c-146">String</span><span class="sxs-lookup"><span data-stu-id="d411c-146">String</span></span>|<span data-ttu-id="d411c-147">Необязательное описание сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="d411c-147">Optional description for the device management script.</span></span>|
|<span data-ttu-id="d411c-148">scriptContent</span><span class="sxs-lookup"><span data-stu-id="d411c-148">scriptContent</span></span>|<span data-ttu-id="d411c-149">В двоичном формате</span><span class="sxs-lookup"><span data-stu-id="d411c-149">Binary</span></span>|<span data-ttu-id="d411c-150">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="d411c-150">The script content.</span></span>|
|<span data-ttu-id="d411c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d411c-151">createdDateTime</span></span>|<span data-ttu-id="d411c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d411c-152">DateTimeOffset</span></span>|<span data-ttu-id="d411c-153">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="d411c-153">The date and time the device management script was created.</span></span> <span data-ttu-id="d411c-154">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d411c-154">This property is read-only.</span></span>|
|<span data-ttu-id="d411c-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d411c-155">lastModifiedDateTime</span></span>|<span data-ttu-id="d411c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d411c-156">DateTimeOffset</span></span>|<span data-ttu-id="d411c-157">Дата и время последнего изменения сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="d411c-157">The date and time the device management script was last modified.</span></span> <span data-ttu-id="d411c-158">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d411c-158">This property is read-only.</span></span>|
|<span data-ttu-id="d411c-159">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="d411c-159">runAsAccount</span></span>|[<span data-ttu-id="d411c-160">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="d411c-160">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="d411c-161">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="d411c-161">Indicates the type of execution context.</span></span> <span data-ttu-id="d411c-162">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="d411c-162">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="d411c-163">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="d411c-163">enforceSignatureCheck</span></span>|<span data-ttu-id="d411c-164">Логический</span><span class="sxs-lookup"><span data-stu-id="d411c-164">Boolean</span></span>|<span data-ttu-id="d411c-165">Указать, нужно ли проверять подпись скрипта.</span><span class="sxs-lookup"><span data-stu-id="d411c-165">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="d411c-166">fileName</span><span class="sxs-lookup"><span data-stu-id="d411c-166">fileName</span></span>|<span data-ttu-id="d411c-167">String</span><span class="sxs-lookup"><span data-stu-id="d411c-167">String</span></span>|<span data-ttu-id="d411c-168">Имя файла скрипта.</span><span class="sxs-lookup"><span data-stu-id="d411c-168">Script file name.</span></span>|
|<span data-ttu-id="d411c-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d411c-169">roleScopeTagIds</span></span>|<span data-ttu-id="d411c-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d411c-170">String collection</span></span>|<span data-ttu-id="d411c-171">Список ID-тегов области для этого экземпляра PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="d411c-171">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="d411c-172">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="d411c-172">runAs32Bit</span></span>|<span data-ttu-id="d411c-173">Логический</span><span class="sxs-lookup"><span data-stu-id="d411c-173">Boolean</span></span>|<span data-ttu-id="d411c-174">Значение, указывающее, должен ли скрипт PowerShell работать как 32-битный</span><span class="sxs-lookup"><span data-stu-id="d411c-174">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="d411c-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="d411c-175">Response</span></span>
<span data-ttu-id="d411c-176">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d411c-176">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d411c-177">Пример</span><span class="sxs-lookup"><span data-stu-id="d411c-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="d411c-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="d411c-178">Request</span></span>
<span data-ttu-id="d411c-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d411c-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d411c-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="d411c-180">Response</span></span>
<span data-ttu-id="d411c-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d411c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







