---
title: Обновление Девицеманажементинтежерсеттингинстанце
description: Обновление свойств объекта Девицеманажементинтежерсеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b6f0a92030beb113bc3ed656995609f20ad76bb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42471584"
---
# <a name="update-devicemanagementintegersettinginstance"></a><span data-ttu-id="9114f-103">Обновление Девицеманажементинтежерсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="9114f-103">Update deviceManagementIntegerSettingInstance</span></span>

<span data-ttu-id="9114f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9114f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9114f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9114f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9114f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9114f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9114f-107">Обновление свойств объекта [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="9114f-107">Update the properties of a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9114f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9114f-108">Prerequisites</span></span>
<span data-ttu-id="9114f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9114f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9114f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9114f-111">Permission type</span></span>|<span data-ttu-id="9114f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9114f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9114f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9114f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9114f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9114f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9114f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9114f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9114f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9114f-116">Not supported.</span></span>|
|<span data-ttu-id="9114f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9114f-117">Application</span></span>|<span data-ttu-id="9114f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9114f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9114f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9114f-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9114f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9114f-120">Request headers</span></span>
|<span data-ttu-id="9114f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9114f-121">Header</span></span>|<span data-ttu-id="9114f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9114f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9114f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9114f-123">Authorization</span></span>|<span data-ttu-id="9114f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9114f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9114f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9114f-125">Accept</span></span>|<span data-ttu-id="9114f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9114f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9114f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9114f-127">Request body</span></span>
<span data-ttu-id="9114f-128">В тексте запроса добавьте представление объекта [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9114f-128">In the request body, supply a JSON representation for the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

<span data-ttu-id="9114f-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="9114f-129">The following table shows the properties that are required when you create the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).</span></span>

|<span data-ttu-id="9114f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9114f-130">Property</span></span>|<span data-ttu-id="9114f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9114f-131">Type</span></span>|<span data-ttu-id="9114f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9114f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9114f-133">id</span><span class="sxs-lookup"><span data-stu-id="9114f-133">id</span></span>|<span data-ttu-id="9114f-134">String</span><span class="sxs-lookup"><span data-stu-id="9114f-134">String</span></span>|<span data-ttu-id="9114f-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="9114f-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="9114f-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="9114f-136">definitionId</span></span>|<span data-ttu-id="9114f-137">String</span><span class="sxs-lookup"><span data-stu-id="9114f-137">String</span></span>|<span data-ttu-id="9114f-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="9114f-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="9114f-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="9114f-139">valueJson</span></span>|<span data-ttu-id="9114f-140">String</span><span class="sxs-lookup"><span data-stu-id="9114f-140">String</span></span>|<span data-ttu-id="9114f-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="9114f-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="9114f-142">value</span><span class="sxs-lookup"><span data-stu-id="9114f-142">value</span></span>|<span data-ttu-id="9114f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="9114f-143">Int32</span></span>|<span data-ttu-id="9114f-144">Целое значение</span><span class="sxs-lookup"><span data-stu-id="9114f-144">The integer value</span></span>|



## <a name="response"></a><span data-ttu-id="9114f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9114f-145">Response</span></span>
<span data-ttu-id="9114f-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9114f-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9114f-147">Пример</span><span class="sxs-lookup"><span data-stu-id="9114f-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="9114f-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="9114f-148">Request</span></span>
<span data-ttu-id="9114f-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9114f-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9114f-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="9114f-150">Response</span></span>
<span data-ttu-id="9114f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9114f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





