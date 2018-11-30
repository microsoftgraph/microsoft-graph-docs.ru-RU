---
title: Обновление deviceManagementScript
description: Обновление свойства объекта deviceManagementScript.
ms.openlocfilehash: d88579f130607b08b0d34620b701be5c239bc03f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077948"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="6cc18-103">Обновление deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="6cc18-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="6cc18-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6cc18-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cc18-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cc18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6cc18-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6cc18-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6cc18-107">Обновление свойства объекта [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="6cc18-107">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6cc18-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6cc18-108">Prerequisites</span></span>
<span data-ttu-id="6cc18-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cc18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cc18-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cc18-111">Permission type</span></span>|<span data-ttu-id="6cc18-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cc18-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cc18-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cc18-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cc18-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cc18-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6cc18-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cc18-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cc18-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cc18-116">Not supported.</span></span>|
|<span data-ttu-id="6cc18-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6cc18-117">Application</span></span>|<span data-ttu-id="6cc18-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cc18-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cc18-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cc18-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="6cc18-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6cc18-120">Request headers</span></span>
|<span data-ttu-id="6cc18-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6cc18-121">Header</span></span>|<span data-ttu-id="6cc18-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6cc18-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cc18-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cc18-123">Authorization</span></span>|<span data-ttu-id="6cc18-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6cc18-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cc18-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6cc18-125">Accept</span></span>|<span data-ttu-id="6cc18-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6cc18-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cc18-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6cc18-127">Request body</span></span>
<span data-ttu-id="6cc18-128">В тексте запроса укажите представление JSON для объекта [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="6cc18-128">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="6cc18-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="6cc18-129">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>

|<span data-ttu-id="6cc18-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6cc18-130">Property</span></span>|<span data-ttu-id="6cc18-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6cc18-131">Type</span></span>|<span data-ttu-id="6cc18-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6cc18-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cc18-133">id</span><span class="sxs-lookup"><span data-stu-id="6cc18-133">id</span></span>|<span data-ttu-id="6cc18-134">String</span><span class="sxs-lookup"><span data-stu-id="6cc18-134">String</span></span>|<span data-ttu-id="6cc18-135">Уникальный идентификатор для сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="6cc18-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="6cc18-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6cc18-136">displayName</span></span>|<span data-ttu-id="6cc18-137">String</span><span class="sxs-lookup"><span data-stu-id="6cc18-137">String</span></span>|<span data-ttu-id="6cc18-138">Имя скрипта управления устройства.</span><span class="sxs-lookup"><span data-stu-id="6cc18-138">Name of the device management script.</span></span>|
|<span data-ttu-id="6cc18-139">описание</span><span class="sxs-lookup"><span data-stu-id="6cc18-139">description</span></span>|<span data-ttu-id="6cc18-140">String</span><span class="sxs-lookup"><span data-stu-id="6cc18-140">String</span></span>|<span data-ttu-id="6cc18-141">Необязательное описание сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="6cc18-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="6cc18-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="6cc18-142">runSchedule</span></span>|[<span data-ttu-id="6cc18-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="6cc18-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="6cc18-144">Интервал для запуска сценария.</span><span class="sxs-lookup"><span data-stu-id="6cc18-144">The interval for script to run.</span></span> <span data-ttu-id="6cc18-145">Если не определена сценарий будет выполняться один раз</span><span class="sxs-lookup"><span data-stu-id="6cc18-145">If not defined the script will run once</span></span>|
|<span data-ttu-id="6cc18-146">scriptContent</span><span class="sxs-lookup"><span data-stu-id="6cc18-146">scriptContent</span></span>|<span data-ttu-id="6cc18-147">Двоичный</span><span class="sxs-lookup"><span data-stu-id="6cc18-147">Binary</span></span>|<span data-ttu-id="6cc18-148">Содержимое сценария.</span><span class="sxs-lookup"><span data-stu-id="6cc18-148">The script content.</span></span>|
|<span data-ttu-id="6cc18-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6cc18-149">createdDateTime</span></span>|<span data-ttu-id="6cc18-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cc18-150">DateTimeOffset</span></span>|<span data-ttu-id="6cc18-151">Дата и время создания сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="6cc18-151">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="6cc18-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6cc18-152">lastModifiedDateTime</span></span>|<span data-ttu-id="6cc18-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cc18-153">DateTimeOffset</span></span>|<span data-ttu-id="6cc18-154">Дата и время последнего изменения сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="6cc18-154">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="6cc18-155">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="6cc18-155">runAsAccount</span></span>|[<span data-ttu-id="6cc18-156">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="6cc18-156">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="6cc18-157">Указывает тип контекста выполнения скрипта управления устройства выполняется в.</span><span class="sxs-lookup"><span data-stu-id="6cc18-157">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="6cc18-158">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="6cc18-158">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="6cc18-159">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="6cc18-159">enforceSignatureCheck</span></span>|<span data-ttu-id="6cc18-160">Логический</span><span class="sxs-lookup"><span data-stu-id="6cc18-160">Boolean</span></span>|<span data-ttu-id="6cc18-161">Указывает, должно быть извлеченных подписи скрипта.</span><span class="sxs-lookup"><span data-stu-id="6cc18-161">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="6cc18-162">fileName</span><span class="sxs-lookup"><span data-stu-id="6cc18-162">fileName</span></span>|<span data-ttu-id="6cc18-163">String</span><span class="sxs-lookup"><span data-stu-id="6cc18-163">String</span></span>|<span data-ttu-id="6cc18-164">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="6cc18-164">Script file name.</span></span>|



## <a name="response"></a><span data-ttu-id="6cc18-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="6cc18-165">Response</span></span>
<span data-ttu-id="6cc18-166">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6cc18-166">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cc18-167">Пример</span><span class="sxs-lookup"><span data-stu-id="6cc18-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="6cc18-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cc18-168">Request</span></span>
<span data-ttu-id="6cc18-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cc18-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 361

{
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value"
}
```

### <a name="response"></a><span data-ttu-id="6cc18-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="6cc18-170">Response</span></span>
<span data-ttu-id="6cc18-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6cc18-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 530

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
  "fileName": "File Name value"
}
```





