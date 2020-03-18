---
title: Создание Девицеманажементбулеансеттингинстанце
description: Создание нового объекта Девицеманажементбулеансеттингинстанце.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c0ea64c5c33562cdb2278e0a8b6f9ce00cadb924
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42731098"
---
# <a name="create-devicemanagementbooleansettinginstance"></a><span data-ttu-id="35d54-103">Создание Девицеманажементбулеансеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="35d54-103">Create deviceManagementBooleanSettingInstance</span></span>

> <span data-ttu-id="35d54-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35d54-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35d54-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35d54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35d54-106">Создание нового объекта [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="35d54-106">Create a new [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35d54-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="35d54-107">Prerequisites</span></span>
<span data-ttu-id="35d54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35d54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35d54-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35d54-110">Permission type</span></span>|<span data-ttu-id="35d54-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35d54-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35d54-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35d54-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35d54-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35d54-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="35d54-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35d54-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35d54-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35d54-115">Not supported.</span></span>|
|<span data-ttu-id="35d54-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="35d54-116">Application</span></span>|<span data-ttu-id="35d54-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35d54-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35d54-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35d54-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/settings
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a><span data-ttu-id="35d54-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="35d54-119">Request headers</span></span>
|<span data-ttu-id="35d54-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35d54-120">Header</span></span>|<span data-ttu-id="35d54-121">Значение</span><span class="sxs-lookup"><span data-stu-id="35d54-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35d54-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="35d54-122">Authorization</span></span>|<span data-ttu-id="35d54-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35d54-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35d54-124">Accept</span><span class="sxs-lookup"><span data-stu-id="35d54-124">Accept</span></span>|<span data-ttu-id="35d54-125">application/json</span><span class="sxs-lookup"><span data-stu-id="35d54-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35d54-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35d54-126">Request body</span></span>
<span data-ttu-id="35d54-127">В тексте запроса добавьте представление объекта Девицеманажементбулеансеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35d54-127">In the request body, supply a JSON representation for the deviceManagementBooleanSettingInstance object.</span></span>

<span data-ttu-id="35d54-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементбулеансеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="35d54-128">The following table shows the properties that are required when you create the deviceManagementBooleanSettingInstance.</span></span>

|<span data-ttu-id="35d54-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="35d54-129">Property</span></span>|<span data-ttu-id="35d54-130">Тип</span><span class="sxs-lookup"><span data-stu-id="35d54-130">Type</span></span>|<span data-ttu-id="35d54-131">Описание</span><span class="sxs-lookup"><span data-stu-id="35d54-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35d54-132">id</span><span class="sxs-lookup"><span data-stu-id="35d54-132">id</span></span>|<span data-ttu-id="35d54-133">String</span><span class="sxs-lookup"><span data-stu-id="35d54-133">String</span></span>|<span data-ttu-id="35d54-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="35d54-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="35d54-135">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="35d54-135">definitionId</span></span>|<span data-ttu-id="35d54-136">String</span><span class="sxs-lookup"><span data-stu-id="35d54-136">String</span></span>|<span data-ttu-id="35d54-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="35d54-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="35d54-138">валуежсон</span><span class="sxs-lookup"><span data-stu-id="35d54-138">valueJson</span></span>|<span data-ttu-id="35d54-139">String</span><span class="sxs-lookup"><span data-stu-id="35d54-139">String</span></span>|<span data-ttu-id="35d54-140">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="35d54-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="35d54-141">value</span><span class="sxs-lookup"><span data-stu-id="35d54-141">value</span></span>|<span data-ttu-id="35d54-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="35d54-142">Boolean</span></span>|<span data-ttu-id="35d54-143">Логическое значение</span><span class="sxs-lookup"><span data-stu-id="35d54-143">The boolean value</span></span>|



## <a name="response"></a><span data-ttu-id="35d54-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="35d54-144">Response</span></span>
<span data-ttu-id="35d54-145">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="35d54-145">If successful, this method returns a `201 Created` response code and a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35d54-146">Пример</span><span class="sxs-lookup"><span data-stu-id="35d54-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="35d54-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="35d54-147">Request</span></span>
<span data-ttu-id="35d54-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35d54-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 176

{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="35d54-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="35d54-149">Response</span></span>
<span data-ttu-id="35d54-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35d54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 225

{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "id": "bb9b0041-0041-bb9b-4100-9bbb41009bbb",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": true
}
```




