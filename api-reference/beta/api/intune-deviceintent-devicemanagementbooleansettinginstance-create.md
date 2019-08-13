---
title: Создание Девицеманажементбулеансеттингинстанце
description: Создание нового объекта Девицеманажементбулеансеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9253cb2a65edde8b85b9177410b436271dbae16a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343951"
---
# <a name="create-devicemanagementbooleansettinginstance"></a><span data-ttu-id="af9a5-103">Создание Девицеманажементбулеансеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="af9a5-103">Create deviceManagementBooleanSettingInstance</span></span>

> <span data-ttu-id="af9a5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af9a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af9a5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af9a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af9a5-106">Создание нового объекта [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="af9a5-106">Create a new [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af9a5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="af9a5-107">Prerequisites</span></span>
<span data-ttu-id="af9a5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af9a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af9a5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af9a5-110">Permission type</span></span>|<span data-ttu-id="af9a5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af9a5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af9a5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af9a5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af9a5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af9a5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af9a5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af9a5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af9a5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af9a5-115">Not supported.</span></span>|
|<span data-ttu-id="af9a5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af9a5-116">Application</span></span>|<span data-ttu-id="af9a5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af9a5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af9a5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af9a5-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="af9a5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af9a5-119">Request headers</span></span>
|<span data-ttu-id="af9a5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af9a5-120">Header</span></span>|<span data-ttu-id="af9a5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="af9a5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af9a5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af9a5-122">Authorization</span></span>|<span data-ttu-id="af9a5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af9a5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af9a5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="af9a5-124">Accept</span></span>|<span data-ttu-id="af9a5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af9a5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af9a5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="af9a5-126">Request body</span></span>
<span data-ttu-id="af9a5-127">В тексте запроса добавьте представление объекта Девицеманажементбулеансеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af9a5-127">In the request body, supply a JSON representation for the deviceManagementBooleanSettingInstance object.</span></span>

<span data-ttu-id="af9a5-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементбулеансеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="af9a5-128">The following table shows the properties that are required when you create the deviceManagementBooleanSettingInstance.</span></span>

|<span data-ttu-id="af9a5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="af9a5-129">Property</span></span>|<span data-ttu-id="af9a5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="af9a5-130">Type</span></span>|<span data-ttu-id="af9a5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="af9a5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af9a5-132">id</span><span class="sxs-lookup"><span data-stu-id="af9a5-132">id</span></span>|<span data-ttu-id="af9a5-133">String</span><span class="sxs-lookup"><span data-stu-id="af9a5-133">String</span></span>|<span data-ttu-id="af9a5-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="af9a5-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="af9a5-135">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="af9a5-135">definitionId</span></span>|<span data-ttu-id="af9a5-136">String</span><span class="sxs-lookup"><span data-stu-id="af9a5-136">String</span></span>|<span data-ttu-id="af9a5-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="af9a5-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="af9a5-138">валуежсон</span><span class="sxs-lookup"><span data-stu-id="af9a5-138">valueJson</span></span>|<span data-ttu-id="af9a5-139">String</span><span class="sxs-lookup"><span data-stu-id="af9a5-139">String</span></span>|<span data-ttu-id="af9a5-140">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="af9a5-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="af9a5-141">value</span><span class="sxs-lookup"><span data-stu-id="af9a5-141">value</span></span>|<span data-ttu-id="af9a5-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="af9a5-142">Boolean</span></span>|<span data-ttu-id="af9a5-143">Логическое значение</span><span class="sxs-lookup"><span data-stu-id="af9a5-143">The boolean value</span></span>|



## <a name="response"></a><span data-ttu-id="af9a5-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="af9a5-144">Response</span></span>
<span data-ttu-id="af9a5-145">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="af9a5-145">If successful, this method returns a `201 Created` response code and a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af9a5-146">Пример</span><span class="sxs-lookup"><span data-stu-id="af9a5-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="af9a5-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="af9a5-147">Request</span></span>
<span data-ttu-id="af9a5-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af9a5-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="af9a5-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="af9a5-149">Response</span></span>
<span data-ttu-id="af9a5-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af9a5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






