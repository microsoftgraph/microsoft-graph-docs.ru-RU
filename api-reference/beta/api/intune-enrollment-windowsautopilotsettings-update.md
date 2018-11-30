---
title: Обновление windowsAutopilotSettings
description: Обновление свойства объекта windowsAutopilotSettings.
ms.openlocfilehash: 6c02d73a08e18906de6e2959f69c3377c20ce911
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077743"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="21a70-103">Обновление windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="21a70-103">Update windowsAutopilotSettings</span></span>

> <span data-ttu-id="21a70-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="21a70-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21a70-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21a70-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21a70-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="21a70-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21a70-107">Обновление свойства объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="21a70-107">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21a70-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="21a70-108">Prerequisites</span></span>
<span data-ttu-id="21a70-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21a70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21a70-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21a70-111">Permission type</span></span>|<span data-ttu-id="21a70-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21a70-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21a70-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21a70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21a70-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21a70-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="21a70-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21a70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21a70-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21a70-116">Not supported.</span></span>|
|<span data-ttu-id="21a70-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21a70-117">Application</span></span>|<span data-ttu-id="21a70-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21a70-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21a70-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21a70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="21a70-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21a70-120">Request headers</span></span>
|<span data-ttu-id="21a70-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21a70-121">Header</span></span>|<span data-ttu-id="21a70-122">Значение</span><span class="sxs-lookup"><span data-stu-id="21a70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21a70-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21a70-123">Authorization</span></span>|<span data-ttu-id="21a70-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="21a70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21a70-125">Accept</span><span class="sxs-lookup"><span data-stu-id="21a70-125">Accept</span></span>|<span data-ttu-id="21a70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21a70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21a70-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21a70-127">Request body</span></span>
<span data-ttu-id="21a70-128">В тексте запроса укажите представление JSON для объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="21a70-128">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="21a70-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span><span class="sxs-lookup"><span data-stu-id="21a70-129">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="21a70-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="21a70-130">Property</span></span>|<span data-ttu-id="21a70-131">Тип</span><span class="sxs-lookup"><span data-stu-id="21a70-131">Type</span></span>|<span data-ttu-id="21a70-132">Описание</span><span class="sxs-lookup"><span data-stu-id="21a70-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21a70-133">id</span><span class="sxs-lookup"><span data-stu-id="21a70-133">id</span></span>|<span data-ttu-id="21a70-134">Строка</span><span class="sxs-lookup"><span data-stu-id="21a70-134">String</span></span>|<span data-ttu-id="21a70-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="21a70-135">The GUID for the object</span></span>|
|<span data-ttu-id="21a70-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="21a70-136">lastSyncDateTime</span></span>|<span data-ttu-id="21a70-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21a70-137">DateTimeOffset</span></span>|<span data-ttu-id="21a70-138">Последней полной синхронизации даты-времени со службой набору доменов Обнаружения.</span><span class="sxs-lookup"><span data-stu-id="21a70-138">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="21a70-139">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="21a70-139">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="21a70-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21a70-140">DateTimeOffset</span></span>|<span data-ttu-id="21a70-141">Последней полной синхронизации даты-времени со службой набору доменов Обнаружения.</span><span class="sxs-lookup"><span data-stu-id="21a70-141">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="21a70-142">syncStatus</span><span class="sxs-lookup"><span data-stu-id="21a70-142">syncStatus</span></span>|[<span data-ttu-id="21a70-143">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="21a70-143">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="21a70-144">Указывает состояние синхронизации со службой синхронизации (набору доменов Обнаружения) данных устройства.</span><span class="sxs-lookup"><span data-stu-id="21a70-144">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="21a70-145">Возможные значения: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="21a70-145">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="21a70-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="21a70-146">Response</span></span>
<span data-ttu-id="21a70-147">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="21a70-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21a70-148">Пример</span><span class="sxs-lookup"><span data-stu-id="21a70-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="21a70-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="21a70-149">Request</span></span>
<span data-ttu-id="21a70-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21a70-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
Content-type: application/json
Content-length: 167

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```

### <a name="response"></a><span data-ttu-id="21a70-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="21a70-151">Response</span></span>
<span data-ttu-id="21a70-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="21a70-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "08c16770-6770-08c1-7067-c1087067c108",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```





