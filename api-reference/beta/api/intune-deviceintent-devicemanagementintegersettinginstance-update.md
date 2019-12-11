---
title: Обновление Девицеманажементинтежерсеттингинстанце
description: Обновление свойств объекта Девицеманажементинтежерсеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aa2f138ba50f07489bf3a427e47996ce927d8d76
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945909"
---
# <a name="update-devicemanagementintegersettinginstance"></a><span data-ttu-id="402b3-103">Обновление Девицеманажементинтежерсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="402b3-103">Update deviceManagementIntegerSettingInstance</span></span>

> <span data-ttu-id="402b3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="402b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="402b3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="402b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="402b3-106">Обновление свойств объекта [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="402b3-106">Update the properties of a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="402b3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="402b3-107">Prerequisites</span></span>
<span data-ttu-id="402b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="402b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="402b3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="402b3-110">Permission type</span></span>|<span data-ttu-id="402b3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="402b3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="402b3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="402b3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="402b3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="402b3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="402b3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="402b3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="402b3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="402b3-115">Not supported.</span></span>|
|<span data-ttu-id="402b3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="402b3-116">Application</span></span>|<span data-ttu-id="402b3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="402b3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="402b3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="402b3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings/{deviceManagementSettingInstanceId}
```

## <a name="request-headers"></a><span data-ttu-id="402b3-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="402b3-119">Request headers</span></span>
|<span data-ttu-id="402b3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="402b3-120">Header</span></span>|<span data-ttu-id="402b3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="402b3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="402b3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="402b3-122">Authorization</span></span>|<span data-ttu-id="402b3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="402b3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="402b3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="402b3-124">Accept</span></span>|<span data-ttu-id="402b3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="402b3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="402b3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="402b3-126">Request body</span></span>
<span data-ttu-id="402b3-127">В тексте запроса добавьте представление объекта [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="402b3-127">In the request body, supply a JSON representation for the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

<span data-ttu-id="402b3-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="402b3-128">The following table shows the properties that are required when you create the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).</span></span>

|<span data-ttu-id="402b3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="402b3-129">Property</span></span>|<span data-ttu-id="402b3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="402b3-130">Type</span></span>|<span data-ttu-id="402b3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="402b3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="402b3-132">id</span><span class="sxs-lookup"><span data-stu-id="402b3-132">id</span></span>|<span data-ttu-id="402b3-133">Строка</span><span class="sxs-lookup"><span data-stu-id="402b3-133">String</span></span>|<span data-ttu-id="402b3-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="402b3-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="402b3-135">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="402b3-135">definitionId</span></span>|<span data-ttu-id="402b3-136">Строка</span><span class="sxs-lookup"><span data-stu-id="402b3-136">String</span></span>|<span data-ttu-id="402b3-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="402b3-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="402b3-138">валуежсон</span><span class="sxs-lookup"><span data-stu-id="402b3-138">valueJson</span></span>|<span data-ttu-id="402b3-139">Строка</span><span class="sxs-lookup"><span data-stu-id="402b3-139">String</span></span>|<span data-ttu-id="402b3-140">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="402b3-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="402b3-141">value</span><span class="sxs-lookup"><span data-stu-id="402b3-141">value</span></span>|<span data-ttu-id="402b3-142">Int32</span><span class="sxs-lookup"><span data-stu-id="402b3-142">Int32</span></span>|<span data-ttu-id="402b3-143">Целое значение</span><span class="sxs-lookup"><span data-stu-id="402b3-143">The integer value</span></span>|



## <a name="response"></a><span data-ttu-id="402b3-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="402b3-144">Response</span></span>
<span data-ttu-id="402b3-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="402b3-145">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="402b3-146">Пример</span><span class="sxs-lookup"><span data-stu-id="402b3-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="402b3-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="402b3-147">Request</span></span>
<span data-ttu-id="402b3-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="402b3-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="402b3-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="402b3-149">Response</span></span>
<span data-ttu-id="402b3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="402b3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "id": "60468ce7-8ce7-6046-e78c-4660e78c4660",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```





