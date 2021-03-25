---
title: Обновление deviceShellScript
description: Обновление свойств объекта deviceShellScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b340b51afda2b4d06f86456e34f36a5347fa36f3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150229"
---
# <a name="update-deviceshellscript"></a><span data-ttu-id="cb034-103">Обновление deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="cb034-103">Update deviceShellScript</span></span>

<span data-ttu-id="cb034-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb034-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb034-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb034-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb034-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb034-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb034-107">Обновление свойств объекта [deviceShellScript.](../resources/intune-devices-deviceshellscript.md)</span><span class="sxs-lookup"><span data-stu-id="cb034-107">Update the properties of a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb034-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cb034-108">Prerequisites</span></span>
<span data-ttu-id="cb034-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb034-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb034-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb034-111">Permission type</span></span>|<span data-ttu-id="cb034-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb034-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb034-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb034-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb034-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb034-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cb034-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb034-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb034-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb034-116">Not supported.</span></span>|
|<span data-ttu-id="cb034-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cb034-117">Application</span></span>|<span data-ttu-id="cb034-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb034-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb034-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb034-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="cb034-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cb034-120">Request headers</span></span>
|<span data-ttu-id="cb034-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb034-121">Header</span></span>|<span data-ttu-id="cb034-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cb034-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb034-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb034-123">Authorization</span></span>|<span data-ttu-id="cb034-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb034-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb034-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cb034-125">Accept</span></span>|<span data-ttu-id="cb034-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb034-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb034-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb034-127">Request body</span></span>
<span data-ttu-id="cb034-128">В теле запроса поставляем представление JSON для [объекта deviceShellScript.](../resources/intune-devices-deviceshellscript.md)</span><span class="sxs-lookup"><span data-stu-id="cb034-128">In the request body, supply a JSON representation for the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

<span data-ttu-id="cb034-129">В следующей таблице показаны свойства, необходимые при создании [устройстваShellScript.](../resources/intune-devices-deviceshellscript.md)</span><span class="sxs-lookup"><span data-stu-id="cb034-129">The following table shows the properties that are required when you create the [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>

|<span data-ttu-id="cb034-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb034-130">Property</span></span>|<span data-ttu-id="cb034-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cb034-131">Type</span></span>|<span data-ttu-id="cb034-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cb034-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb034-133">executionFrequency</span><span class="sxs-lookup"><span data-stu-id="cb034-133">executionFrequency</span></span>|<span data-ttu-id="cb034-134">Duration</span><span class="sxs-lookup"><span data-stu-id="cb034-134">Duration</span></span>|<span data-ttu-id="cb034-135">Интервал для запуска скрипта.</span><span class="sxs-lookup"><span data-stu-id="cb034-135">The interval for script to run.</span></span> <span data-ttu-id="cb034-136">Если сценарий не определен, он будет работать один раз</span><span class="sxs-lookup"><span data-stu-id="cb034-136">If not defined the script will run once</span></span>|
|<span data-ttu-id="cb034-137">retryCount</span><span class="sxs-lookup"><span data-stu-id="cb034-137">retryCount</span></span>|<span data-ttu-id="cb034-138">Int32</span><span class="sxs-lookup"><span data-stu-id="cb034-138">Int32</span></span>|<span data-ttu-id="cb034-139">Количество случаев повторного и повторного и повторного повторного и повторного списания сценария</span><span class="sxs-lookup"><span data-stu-id="cb034-139">Number of times for the script to be retried if it fails</span></span>|
|<span data-ttu-id="cb034-140">blockExecutionNotifications</span><span class="sxs-lookup"><span data-stu-id="cb034-140">blockExecutionNotifications</span></span>|<span data-ttu-id="cb034-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb034-141">Boolean</span></span>|<span data-ttu-id="cb034-142">Не уведомляет пользователя о выполнении сценария</span><span class="sxs-lookup"><span data-stu-id="cb034-142">Does not notify the user a script is being executed</span></span>|
|<span data-ttu-id="cb034-143">id</span><span class="sxs-lookup"><span data-stu-id="cb034-143">id</span></span>|<span data-ttu-id="cb034-144">Строка</span><span class="sxs-lookup"><span data-stu-id="cb034-144">String</span></span>|<span data-ttu-id="cb034-145">Уникальный идентификатор для сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="cb034-145">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="cb034-146">displayName</span><span class="sxs-lookup"><span data-stu-id="cb034-146">displayName</span></span>|<span data-ttu-id="cb034-147">Строка</span><span class="sxs-lookup"><span data-stu-id="cb034-147">String</span></span>|<span data-ttu-id="cb034-148">Имя сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="cb034-148">Name of the device management script.</span></span>|
|<span data-ttu-id="cb034-149">description</span><span class="sxs-lookup"><span data-stu-id="cb034-149">description</span></span>|<span data-ttu-id="cb034-150">Строка</span><span class="sxs-lookup"><span data-stu-id="cb034-150">String</span></span>|<span data-ttu-id="cb034-151">Необязательное описание сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="cb034-151">Optional description for the device management script.</span></span>|
|<span data-ttu-id="cb034-152">scriptContent</span><span class="sxs-lookup"><span data-stu-id="cb034-152">scriptContent</span></span>|<span data-ttu-id="cb034-153">Binary</span><span class="sxs-lookup"><span data-stu-id="cb034-153">Binary</span></span>|<span data-ttu-id="cb034-154">Содержимое скрипта.</span><span class="sxs-lookup"><span data-stu-id="cb034-154">The script content.</span></span>|
|<span data-ttu-id="cb034-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb034-155">createdDateTime</span></span>|<span data-ttu-id="cb034-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb034-156">DateTimeOffset</span></span>|<span data-ttu-id="cb034-157">Дата и время создания сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="cb034-157">The date and time the device management script was created.</span></span> <span data-ttu-id="cb034-158">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb034-158">This property is read-only.</span></span>|
|<span data-ttu-id="cb034-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb034-159">lastModifiedDateTime</span></span>|<span data-ttu-id="cb034-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb034-160">DateTimeOffset</span></span>|<span data-ttu-id="cb034-161">Дата и время последнего изменения сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="cb034-161">The date and time the device management script was last modified.</span></span> <span data-ttu-id="cb034-162">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb034-162">This property is read-only.</span></span>|
|<span data-ttu-id="cb034-163">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="cb034-163">runAsAccount</span></span>|[<span data-ttu-id="cb034-164">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="cb034-164">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="cb034-165">Указывает тип контекста выполнения.</span><span class="sxs-lookup"><span data-stu-id="cb034-165">Indicates the type of execution context.</span></span> <span data-ttu-id="cb034-166">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="cb034-166">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="cb034-167">fileName</span><span class="sxs-lookup"><span data-stu-id="cb034-167">fileName</span></span>|<span data-ttu-id="cb034-168">String</span><span class="sxs-lookup"><span data-stu-id="cb034-168">String</span></span>|<span data-ttu-id="cb034-169">Имя файла скрипта.</span><span class="sxs-lookup"><span data-stu-id="cb034-169">Script file name.</span></span>|
|<span data-ttu-id="cb034-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cb034-170">roleScopeTagIds</span></span>|<span data-ttu-id="cb034-171">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cb034-171">String collection</span></span>|<span data-ttu-id="cb034-172">Список ID-тегов области для этого экземпляра PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="cb034-172">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="cb034-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb034-173">Response</span></span>
<span data-ttu-id="cb034-174">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект deviceShellScript](../resources/intune-devices-deviceshellscript.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cb034-174">If successful, this method returns a `200 OK` response code and an updated [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb034-175">Пример</span><span class="sxs-lookup"><span data-stu-id="cb034-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb034-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb034-176">Request</span></span>
<span data-ttu-id="cb034-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb034-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}
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

### <a name="response"></a><span data-ttu-id="cb034-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb034-178">Response</span></span>
<span data-ttu-id="cb034-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb034-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




