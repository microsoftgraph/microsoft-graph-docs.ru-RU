---
title: Создание Девицеманажементбулеансеттингинстанце
description: Создание нового объекта Девицеманажементбулеансеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0a2a47f04b1850c2dcf54d48bdb06b0243c2c40e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43330370"
---
# <a name="create-devicemanagementbooleansettinginstance"></a><span data-ttu-id="b051a-103">Создание Девицеманажементбулеансеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="b051a-103">Create deviceManagementBooleanSettingInstance</span></span>

<span data-ttu-id="b051a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b051a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b051a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b051a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b051a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b051a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b051a-107">Создание нового объекта [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="b051a-107">Create a new [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b051a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b051a-108">Prerequisites</span></span>
<span data-ttu-id="b051a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b051a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b051a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b051a-111">Permission type</span></span>|<span data-ttu-id="b051a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b051a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b051a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b051a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b051a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b051a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b051a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b051a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b051a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b051a-116">Not supported.</span></span>|
|<span data-ttu-id="b051a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b051a-117">Application</span></span>|<span data-ttu-id="b051a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b051a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b051a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b051a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b051a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b051a-120">Request headers</span></span>
|<span data-ttu-id="b051a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b051a-121">Header</span></span>|<span data-ttu-id="b051a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b051a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b051a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b051a-123">Authorization</span></span>|<span data-ttu-id="b051a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b051a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b051a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b051a-125">Accept</span></span>|<span data-ttu-id="b051a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b051a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b051a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b051a-127">Request body</span></span>
<span data-ttu-id="b051a-128">В тексте запроса добавьте представление объекта Девицеманажементбулеансеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b051a-128">In the request body, supply a JSON representation for the deviceManagementBooleanSettingInstance object.</span></span>

<span data-ttu-id="b051a-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементбулеансеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="b051a-129">The following table shows the properties that are required when you create the deviceManagementBooleanSettingInstance.</span></span>

|<span data-ttu-id="b051a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b051a-130">Property</span></span>|<span data-ttu-id="b051a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b051a-131">Type</span></span>|<span data-ttu-id="b051a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b051a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b051a-133">id</span><span class="sxs-lookup"><span data-stu-id="b051a-133">id</span></span>|<span data-ttu-id="b051a-134">String</span><span class="sxs-lookup"><span data-stu-id="b051a-134">String</span></span>|<span data-ttu-id="b051a-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="b051a-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="b051a-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="b051a-136">definitionId</span></span>|<span data-ttu-id="b051a-137">String</span><span class="sxs-lookup"><span data-stu-id="b051a-137">String</span></span>|<span data-ttu-id="b051a-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="b051a-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="b051a-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="b051a-139">valueJson</span></span>|<span data-ttu-id="b051a-140">String</span><span class="sxs-lookup"><span data-stu-id="b051a-140">String</span></span>|<span data-ttu-id="b051a-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="b051a-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="b051a-142">value</span><span class="sxs-lookup"><span data-stu-id="b051a-142">value</span></span>|<span data-ttu-id="b051a-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="b051a-143">Boolean</span></span>|<span data-ttu-id="b051a-144">Логическое значение</span><span class="sxs-lookup"><span data-stu-id="b051a-144">The boolean value</span></span>|



## <a name="response"></a><span data-ttu-id="b051a-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b051a-145">Response</span></span>
<span data-ttu-id="b051a-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b051a-146">If successful, this method returns a `201 Created` response code and a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b051a-147">Пример</span><span class="sxs-lookup"><span data-stu-id="b051a-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="b051a-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="b051a-148">Request</span></span>
<span data-ttu-id="b051a-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b051a-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b051a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="b051a-150">Response</span></span>
<span data-ttu-id="b051a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b051a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



