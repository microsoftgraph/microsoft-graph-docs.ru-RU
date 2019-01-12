---
title: Обновление windowsAutopilotSettings
description: Обновление свойства объекта windowsAutopilotSettings.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3d07ce1b4416b671e8d18ebaa416d2b6e7ffe96e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945106"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="144ff-103">Обновление windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="144ff-103">Update windowsAutopilotSettings</span></span>

> <span data-ttu-id="144ff-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="144ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="144ff-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="144ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="144ff-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="144ff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="144ff-107">Обновление свойства объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="144ff-107">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="144ff-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="144ff-108">Prerequisites</span></span>
<span data-ttu-id="144ff-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="144ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="144ff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="144ff-111">Permission type</span></span>|<span data-ttu-id="144ff-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="144ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="144ff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="144ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="144ff-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="144ff-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="144ff-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="144ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="144ff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="144ff-116">Not supported.</span></span>|
|<span data-ttu-id="144ff-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="144ff-117">Application</span></span>|<span data-ttu-id="144ff-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="144ff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="144ff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="144ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="144ff-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="144ff-120">Request headers</span></span>
|<span data-ttu-id="144ff-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="144ff-121">Header</span></span>|<span data-ttu-id="144ff-122">Значение</span><span class="sxs-lookup"><span data-stu-id="144ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="144ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="144ff-123">Authorization</span></span>|<span data-ttu-id="144ff-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="144ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="144ff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="144ff-125">Accept</span></span>|<span data-ttu-id="144ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="144ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="144ff-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="144ff-127">Request body</span></span>
<span data-ttu-id="144ff-128">В тексте запроса укажите представление JSON для объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="144ff-128">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="144ff-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span><span class="sxs-lookup"><span data-stu-id="144ff-129">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="144ff-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="144ff-130">Property</span></span>|<span data-ttu-id="144ff-131">Тип</span><span class="sxs-lookup"><span data-stu-id="144ff-131">Type</span></span>|<span data-ttu-id="144ff-132">Описание</span><span class="sxs-lookup"><span data-stu-id="144ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="144ff-133">id</span><span class="sxs-lookup"><span data-stu-id="144ff-133">id</span></span>|<span data-ttu-id="144ff-134">Строка</span><span class="sxs-lookup"><span data-stu-id="144ff-134">String</span></span>|<span data-ttu-id="144ff-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="144ff-135">The GUID for the object</span></span>|
|<span data-ttu-id="144ff-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="144ff-136">lastSyncDateTime</span></span>|<span data-ttu-id="144ff-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="144ff-137">DateTimeOffset</span></span>|<span data-ttu-id="144ff-138">Последней полной синхронизации даты-времени со службой набору доменов Обнаружения.</span><span class="sxs-lookup"><span data-stu-id="144ff-138">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="144ff-139">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="144ff-139">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="144ff-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="144ff-140">DateTimeOffset</span></span>|<span data-ttu-id="144ff-141">Последней полной синхронизации даты-времени со службой набору доменов Обнаружения.</span><span class="sxs-lookup"><span data-stu-id="144ff-141">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="144ff-142">syncStatus</span><span class="sxs-lookup"><span data-stu-id="144ff-142">syncStatus</span></span>|[<span data-ttu-id="144ff-143">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="144ff-143">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="144ff-144">Указывает состояние синхронизации со службой синхронизации (набору доменов Обнаружения) данных устройства.</span><span class="sxs-lookup"><span data-stu-id="144ff-144">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="144ff-145">Возможные значения: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="144ff-145">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="144ff-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="144ff-146">Response</span></span>
<span data-ttu-id="144ff-147">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="144ff-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="144ff-148">Пример</span><span class="sxs-lookup"><span data-stu-id="144ff-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="144ff-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="144ff-149">Request</span></span>
<span data-ttu-id="144ff-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="144ff-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="144ff-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="144ff-151">Response</span></span>
<span data-ttu-id="144ff-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="144ff-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





