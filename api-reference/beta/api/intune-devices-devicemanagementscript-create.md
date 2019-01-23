---
title: Создание deviceManagementScript
description: Создание нового объекта deviceManagementScript.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be0ffb8b912b25684ba0ed3dc383a995fb872f3b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409274"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="0e3b9-103">Создание deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="0e3b9-103">Create deviceManagementScript</span></span>

> <span data-ttu-id="0e3b9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0e3b9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e3b9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e3b9-107">Создание нового объекта [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="0e3b9-107">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e3b9-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="0e3b9-108">Prerequisites</span></span>
<span data-ttu-id="0e3b9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0e3b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0e3b9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e3b9-111">Permission type</span></span>|<span data-ttu-id="0e3b9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e3b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e3b9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e3b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e3b9-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e3b9-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0e3b9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e3b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e3b9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-116">Not supported.</span></span>|
|<span data-ttu-id="0e3b9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e3b9-117">Application</span></span>|<span data-ttu-id="0e3b9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e3b9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e3b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="0e3b9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e3b9-120">Request headers</span></span>
|<span data-ttu-id="0e3b9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e3b9-121">Header</span></span>|<span data-ttu-id="0e3b9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0e3b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e3b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e3b9-123">Authorization</span></span>|<span data-ttu-id="0e3b9-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0e3b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e3b9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0e3b9-125">Accept</span></span>|<span data-ttu-id="0e3b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e3b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e3b9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e3b9-127">Request body</span></span>
<span data-ttu-id="0e3b9-128">В тексте запроса укажите представление JSON для объекта deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-128">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="0e3b9-129">В следующей таблице показаны свойства, которые необходимы для создания deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-129">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="0e3b9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e3b9-130">Property</span></span>|<span data-ttu-id="0e3b9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0e3b9-131">Type</span></span>|<span data-ttu-id="0e3b9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0e3b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e3b9-133">id</span><span class="sxs-lookup"><span data-stu-id="0e3b9-133">id</span></span>|<span data-ttu-id="0e3b9-134">String</span><span class="sxs-lookup"><span data-stu-id="0e3b9-134">String</span></span>|<span data-ttu-id="0e3b9-135">Уникальный идентификатор для сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="0e3b9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0e3b9-136">displayName</span></span>|<span data-ttu-id="0e3b9-137">String</span><span class="sxs-lookup"><span data-stu-id="0e3b9-137">String</span></span>|<span data-ttu-id="0e3b9-138">Имя скрипта управления устройства.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-138">Name of the device management script.</span></span>|
|<span data-ttu-id="0e3b9-139">description</span><span class="sxs-lookup"><span data-stu-id="0e3b9-139">description</span></span>|<span data-ttu-id="0e3b9-140">String</span><span class="sxs-lookup"><span data-stu-id="0e3b9-140">String</span></span>|<span data-ttu-id="0e3b9-141">Необязательное описание сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="0e3b9-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="0e3b9-142">runSchedule</span></span>|[<span data-ttu-id="0e3b9-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="0e3b9-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="0e3b9-144">Интервал для запуска сценария.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-144">The interval for script to run.</span></span> <span data-ttu-id="0e3b9-145">Если не определена сценарий будет выполняться один раз</span><span class="sxs-lookup"><span data-stu-id="0e3b9-145">If not defined the script will run once</span></span>|
|<span data-ttu-id="0e3b9-146">scriptContent</span><span class="sxs-lookup"><span data-stu-id="0e3b9-146">scriptContent</span></span>|<span data-ttu-id="0e3b9-147">Binary</span><span class="sxs-lookup"><span data-stu-id="0e3b9-147">Binary</span></span>|<span data-ttu-id="0e3b9-148">Содержимое сценария.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-148">The script content.</span></span>|
|<span data-ttu-id="0e3b9-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e3b9-149">createdDateTime</span></span>|<span data-ttu-id="0e3b9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e3b9-150">DateTimeOffset</span></span>|<span data-ttu-id="0e3b9-151">Дата и время создания сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-151">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="0e3b9-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e3b9-152">lastModifiedDateTime</span></span>|<span data-ttu-id="0e3b9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e3b9-153">DateTimeOffset</span></span>|<span data-ttu-id="0e3b9-154">Дата и время последнего изменения сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-154">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="0e3b9-155">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="0e3b9-155">runAsAccount</span></span>|[<span data-ttu-id="0e3b9-156">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="0e3b9-156">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="0e3b9-157">Указывает тип контекста выполнения скрипта управления устройства выполняется в.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-157">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="0e3b9-158">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-158">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="0e3b9-159">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="0e3b9-159">enforceSignatureCheck</span></span>|<span data-ttu-id="0e3b9-160">Логический</span><span class="sxs-lookup"><span data-stu-id="0e3b9-160">Boolean</span></span>|<span data-ttu-id="0e3b9-161">Указывает, должно быть извлеченных подписи скрипта.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-161">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="0e3b9-162">fileName</span><span class="sxs-lookup"><span data-stu-id="0e3b9-162">fileName</span></span>|<span data-ttu-id="0e3b9-163">String</span><span class="sxs-lookup"><span data-stu-id="0e3b9-163">String</span></span>|<span data-ttu-id="0e3b9-164">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-164">Script file name.</span></span>|
|<span data-ttu-id="0e3b9-165">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0e3b9-165">roleScopeTagIds</span></span>|<span data-ttu-id="0e3b9-166">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0e3b9-166">String collection</span></span>|<span data-ttu-id="0e3b9-167">Список идентификаторов тег области для этого экземпляра PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-167">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="0e3b9-168">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="0e3b9-168">runAs32Bit</span></span>|<span data-ttu-id="0e3b9-169">Логический</span><span class="sxs-lookup"><span data-stu-id="0e3b9-169">Boolean</span></span>|<span data-ttu-id="0e3b9-170">Значение, указывающее ли сценарий PowerShell должна запускаться в 32-разрядная версия</span><span class="sxs-lookup"><span data-stu-id="0e3b9-170">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="0e3b9-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e3b9-171">Response</span></span>
<span data-ttu-id="0e3b9-172">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-172">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e3b9-173">Пример</span><span class="sxs-lookup"><span data-stu-id="0e3b9-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e3b9-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e3b9-174">Request</span></span>
<span data-ttu-id="0e3b9-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0e3b9-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e3b9-176">Response</span></span>
<span data-ttu-id="0e3b9-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0e3b9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




