---
title: Создание Девицеманажементбулеансеттингинстанце
description: Создание нового объекта Девицеманажементбулеансеттингинстанце.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 239fef02ae06cbacc193c06de03fdb6ba3dbedb9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31770468"
---
# <a name="create-devicemanagementbooleansettinginstance"></a><span data-ttu-id="e569d-103">Создание Девицеманажементбулеансеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="e569d-103">Create deviceManagementBooleanSettingInstance</span></span>

> <span data-ttu-id="e569d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e569d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e569d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e569d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e569d-106">Создание нового объекта [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="e569d-106">Create a new [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e569d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e569d-107">Prerequisites</span></span>
<span data-ttu-id="e569d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e569d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e569d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e569d-110">Permission type</span></span>|<span data-ttu-id="e569d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e569d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e569d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e569d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e569d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e569d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e569d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e569d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e569d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e569d-115">Not supported.</span></span>|
|<span data-ttu-id="e569d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e569d-116">Application</span></span>|<span data-ttu-id="e569d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e569d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e569d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e569d-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e569d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e569d-119">Request headers</span></span>
|<span data-ttu-id="e569d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e569d-120">Header</span></span>|<span data-ttu-id="e569d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e569d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e569d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e569d-122">Authorization</span></span>|<span data-ttu-id="e569d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e569d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e569d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e569d-124">Accept</span></span>|<span data-ttu-id="e569d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e569d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e569d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e569d-126">Request body</span></span>
<span data-ttu-id="e569d-127">В тексте запроса добавьте представление объекта Девицеманажементбулеансеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e569d-127">In the request body, supply a JSON representation for the deviceManagementBooleanSettingInstance object.</span></span>

<span data-ttu-id="e569d-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементбулеансеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="e569d-128">The following table shows the properties that are required when you create the deviceManagementBooleanSettingInstance.</span></span>

|<span data-ttu-id="e569d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e569d-129">Property</span></span>|<span data-ttu-id="e569d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e569d-130">Type</span></span>|<span data-ttu-id="e569d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e569d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e569d-132">id</span><span class="sxs-lookup"><span data-stu-id="e569d-132">id</span></span>|<span data-ttu-id="e569d-133">String</span><span class="sxs-lookup"><span data-stu-id="e569d-133">String</span></span>|<span data-ttu-id="e569d-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="e569d-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="e569d-135">Дефинитионид</span><span class="sxs-lookup"><span data-stu-id="e569d-135">definitionId</span></span>|<span data-ttu-id="e569d-136">String</span><span class="sxs-lookup"><span data-stu-id="e569d-136">String</span></span>|<span data-ttu-id="e569d-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="e569d-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="e569d-138">Валуежсон</span><span class="sxs-lookup"><span data-stu-id="e569d-138">valueJson</span></span>|<span data-ttu-id="e569d-139">String</span><span class="sxs-lookup"><span data-stu-id="e569d-139">String</span></span>|<span data-ttu-id="e569d-140">Представление JSON значения, наСледуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="e569d-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="e569d-141">value</span><span class="sxs-lookup"><span data-stu-id="e569d-141">value</span></span>|<span data-ttu-id="e569d-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="e569d-142">Boolean</span></span>|<span data-ttu-id="e569d-143">Логическое значение</span><span class="sxs-lookup"><span data-stu-id="e569d-143">The boolean value</span></span>|



## <a name="response"></a><span data-ttu-id="e569d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="e569d-144">Response</span></span>
<span data-ttu-id="e569d-145">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e569d-145">If successful, this method returns a `201 Created` response code and a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e569d-146">Пример</span><span class="sxs-lookup"><span data-stu-id="e569d-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="e569d-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="e569d-147">Request</span></span>
<span data-ttu-id="e569d-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e569d-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e569d-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="e569d-149">Response</span></span>
<span data-ttu-id="e569d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e569d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





