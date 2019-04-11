---
title: Создание Девицеманажементстрингсеттингинстанце
description: Создание нового объекта Девицеманажементстрингсеттингинстанце.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f52379e6cf4a729f7d1a94c839e8b1956348ea9e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31770321"
---
# <a name="create-devicemanagementstringsettinginstance"></a><span data-ttu-id="4d2e4-103">Создание Девицеманажементстрингсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="4d2e4-103">Create deviceManagementStringSettingInstance</span></span>

> <span data-ttu-id="4d2e4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d2e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d2e4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d2e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d2e4-106">Создание нового объекта [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="4d2e4-106">Create a new [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d2e4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4d2e4-107">Prerequisites</span></span>
<span data-ttu-id="4d2e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d2e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d2e4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d2e4-110">Permission type</span></span>|<span data-ttu-id="4d2e4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d2e4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d2e4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d2e4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d2e4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d2e4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d2e4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d2e4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d2e4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d2e4-115">Not supported.</span></span>|
|<span data-ttu-id="4d2e4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d2e4-116">Application</span></span>|<span data-ttu-id="4d2e4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d2e4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d2e4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d2e4-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4d2e4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d2e4-119">Request headers</span></span>
|<span data-ttu-id="4d2e4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d2e4-120">Header</span></span>|<span data-ttu-id="4d2e4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4d2e4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d2e4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d2e4-122">Authorization</span></span>|<span data-ttu-id="4d2e4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d2e4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d2e4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4d2e4-124">Accept</span></span>|<span data-ttu-id="4d2e4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4d2e4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d2e4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d2e4-126">Request body</span></span>
<span data-ttu-id="4d2e4-127">В тексте запроса добавьте представление объекта Девицеманажементстрингсеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d2e4-127">In the request body, supply a JSON representation for the deviceManagementStringSettingInstance object.</span></span>

<span data-ttu-id="4d2e4-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементстрингсеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="4d2e4-128">The following table shows the properties that are required when you create the deviceManagementStringSettingInstance.</span></span>

|<span data-ttu-id="4d2e4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d2e4-129">Property</span></span>|<span data-ttu-id="4d2e4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4d2e4-130">Type</span></span>|<span data-ttu-id="4d2e4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4d2e4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d2e4-132">id</span><span class="sxs-lookup"><span data-stu-id="4d2e4-132">id</span></span>|<span data-ttu-id="4d2e4-133">String</span><span class="sxs-lookup"><span data-stu-id="4d2e4-133">String</span></span>|<span data-ttu-id="4d2e4-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4d2e4-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="4d2e4-135">Дефинитионид</span><span class="sxs-lookup"><span data-stu-id="4d2e4-135">definitionId</span></span>|<span data-ttu-id="4d2e4-136">String</span><span class="sxs-lookup"><span data-stu-id="4d2e4-136">String</span></span>|<span data-ttu-id="4d2e4-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4d2e4-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="4d2e4-138">Валуежсон</span><span class="sxs-lookup"><span data-stu-id="4d2e4-138">valueJson</span></span>|<span data-ttu-id="4d2e4-139">String</span><span class="sxs-lookup"><span data-stu-id="4d2e4-139">String</span></span>|<span data-ttu-id="4d2e4-140">Представление JSON значения, наСледуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4d2e4-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="4d2e4-141">value</span><span class="sxs-lookup"><span data-stu-id="4d2e4-141">value</span></span>|<span data-ttu-id="4d2e4-142">String</span><span class="sxs-lookup"><span data-stu-id="4d2e4-142">String</span></span>|<span data-ttu-id="4d2e4-143">Строковое значение</span><span class="sxs-lookup"><span data-stu-id="4d2e4-143">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="4d2e4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d2e4-144">Response</span></span>
<span data-ttu-id="4d2e4-145">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d2e4-145">If successful, this method returns a `201 Created` response code and a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d2e4-146">Пример</span><span class="sxs-lookup"><span data-stu-id="4d2e4-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d2e4-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d2e4-147">Request</span></span>
<span data-ttu-id="4d2e4-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d2e4-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="4d2e4-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d2e4-149">Response</span></span>
<span data-ttu-id="4d2e4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d2e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "id": "fef30638-0638-fef3-3806-f3fe3806f3fe",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```





