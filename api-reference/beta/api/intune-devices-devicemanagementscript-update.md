---
title: Обновление deviceManagementScript
description: Обновление свойства объекта deviceManagementScript.
author: tfitzmac
ms.openlocfilehash: e0eb397960a9ddae4041578761d5001b729f1464
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325314"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="78f3b-103">Обновление deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="78f3b-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="78f3b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="78f3b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78f3b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78f3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78f3b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="78f3b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78f3b-107">Обновление свойства объекта [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="78f3b-107">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="78f3b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="78f3b-108">Prerequisites</span></span>
<span data-ttu-id="78f3b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78f3b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78f3b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78f3b-111">Permission type</span></span>|<span data-ttu-id="78f3b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="78f3b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78f3b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78f3b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78f3b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f3b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="78f3b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78f3b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78f3b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78f3b-116">Not supported.</span></span>|
|<span data-ttu-id="78f3b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78f3b-117">Application</span></span>|<span data-ttu-id="78f3b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78f3b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78f3b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78f3b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="78f3b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78f3b-120">Request headers</span></span>
|<span data-ttu-id="78f3b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="78f3b-121">Header</span></span>|<span data-ttu-id="78f3b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="78f3b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78f3b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="78f3b-123">Authorization</span></span>|<span data-ttu-id="78f3b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="78f3b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78f3b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="78f3b-125">Accept</span></span>|<span data-ttu-id="78f3b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78f3b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78f3b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78f3b-127">Request body</span></span>
<span data-ttu-id="78f3b-128">В тексте запроса укажите представление JSON для объекта [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="78f3b-128">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="78f3b-129">В следующей таблице показаны свойства, которые необходимы для создания [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="78f3b-129">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>

|<span data-ttu-id="78f3b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="78f3b-130">Property</span></span>|<span data-ttu-id="78f3b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="78f3b-131">Type</span></span>|<span data-ttu-id="78f3b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="78f3b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78f3b-133">id</span><span class="sxs-lookup"><span data-stu-id="78f3b-133">id</span></span>|<span data-ttu-id="78f3b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="78f3b-134">String</span></span>|<span data-ttu-id="78f3b-135">Уникальный идентификатор для сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="78f3b-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="78f3b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="78f3b-136">displayName</span></span>|<span data-ttu-id="78f3b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="78f3b-137">String</span></span>|<span data-ttu-id="78f3b-138">Имя скрипта управления устройства.</span><span class="sxs-lookup"><span data-stu-id="78f3b-138">Name of the device management script.</span></span>|
|<span data-ttu-id="78f3b-139">описание</span><span class="sxs-lookup"><span data-stu-id="78f3b-139">description</span></span>|<span data-ttu-id="78f3b-140">Строка</span><span class="sxs-lookup"><span data-stu-id="78f3b-140">String</span></span>|<span data-ttu-id="78f3b-141">Необязательное описание сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="78f3b-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="78f3b-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="78f3b-142">runSchedule</span></span>|[<span data-ttu-id="78f3b-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="78f3b-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="78f3b-144">Интервал для запуска сценария.</span><span class="sxs-lookup"><span data-stu-id="78f3b-144">The interval for script to run.</span></span> <span data-ttu-id="78f3b-145">Если не определена сценарий будет выполняться один раз</span><span class="sxs-lookup"><span data-stu-id="78f3b-145">If not defined the script will run once</span></span>|
|<span data-ttu-id="78f3b-146">scriptContent</span><span class="sxs-lookup"><span data-stu-id="78f3b-146">scriptContent</span></span>|<span data-ttu-id="78f3b-147">Binary</span><span class="sxs-lookup"><span data-stu-id="78f3b-147">Binary</span></span>|<span data-ttu-id="78f3b-148">Содержимое сценария.</span><span class="sxs-lookup"><span data-stu-id="78f3b-148">The script content.</span></span>|
|<span data-ttu-id="78f3b-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78f3b-149">createdDateTime</span></span>|<span data-ttu-id="78f3b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78f3b-150">DateTimeOffset</span></span>|<span data-ttu-id="78f3b-151">Дата и время создания сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="78f3b-151">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="78f3b-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78f3b-152">lastModifiedDateTime</span></span>|<span data-ttu-id="78f3b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78f3b-153">DateTimeOffset</span></span>|<span data-ttu-id="78f3b-154">Дата и время последнего изменения сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="78f3b-154">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="78f3b-155">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="78f3b-155">runAsAccount</span></span>|[<span data-ttu-id="78f3b-156">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="78f3b-156">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="78f3b-157">Указывает тип контекста выполнения скрипта управления устройства выполняется в.</span><span class="sxs-lookup"><span data-stu-id="78f3b-157">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="78f3b-158">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="78f3b-158">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="78f3b-159">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="78f3b-159">enforceSignatureCheck</span></span>|<span data-ttu-id="78f3b-160">Boolean.</span><span class="sxs-lookup"><span data-stu-id="78f3b-160">Boolean</span></span>|<span data-ttu-id="78f3b-161">Указывает, должно быть извлеченных подписи скрипта.</span><span class="sxs-lookup"><span data-stu-id="78f3b-161">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="78f3b-162">fileName</span><span class="sxs-lookup"><span data-stu-id="78f3b-162">fileName</span></span>|<span data-ttu-id="78f3b-163">String</span><span class="sxs-lookup"><span data-stu-id="78f3b-163">String</span></span>|<span data-ttu-id="78f3b-164">Имя файла сценария.</span><span class="sxs-lookup"><span data-stu-id="78f3b-164">Script file name.</span></span>|



## <a name="response"></a><span data-ttu-id="78f3b-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="78f3b-165">Response</span></span>
<span data-ttu-id="78f3b-166">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="78f3b-166">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78f3b-167">Пример</span><span class="sxs-lookup"><span data-stu-id="78f3b-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="78f3b-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="78f3b-168">Request</span></span>
<span data-ttu-id="78f3b-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78f3b-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="78f3b-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="78f3b-170">Response</span></span>
<span data-ttu-id="78f3b-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="78f3b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





