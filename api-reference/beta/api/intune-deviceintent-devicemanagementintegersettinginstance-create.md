---
title: Создание Девицеманажементинтежерсеттингинстанце
description: Создание нового объекта Девицеманажементинтежерсеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b87bd1004931263161e06129b18fd39fd56d916c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960610"
---
# <a name="create-devicemanagementintegersettinginstance"></a><span data-ttu-id="4b3df-103">Создание Девицеманажементинтежерсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="4b3df-103">Create deviceManagementIntegerSettingInstance</span></span>

> <span data-ttu-id="4b3df-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b3df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b3df-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b3df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b3df-106">Создание нового объекта [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="4b3df-106">Create a new [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b3df-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4b3df-107">Prerequisites</span></span>
<span data-ttu-id="4b3df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b3df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b3df-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b3df-110">Permission type</span></span>|<span data-ttu-id="4b3df-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b3df-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b3df-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b3df-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b3df-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b3df-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b3df-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b3df-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b3df-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b3df-115">Not supported.</span></span>|
|<span data-ttu-id="4b3df-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b3df-116">Application</span></span>|<span data-ttu-id="4b3df-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b3df-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b3df-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b3df-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4b3df-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b3df-119">Request headers</span></span>
|<span data-ttu-id="4b3df-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b3df-120">Header</span></span>|<span data-ttu-id="4b3df-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4b3df-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b3df-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b3df-122">Authorization</span></span>|<span data-ttu-id="4b3df-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b3df-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b3df-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4b3df-124">Accept</span></span>|<span data-ttu-id="4b3df-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b3df-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b3df-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4b3df-126">Request body</span></span>
<span data-ttu-id="4b3df-127">В тексте запроса добавьте представление объекта Девицеманажементинтежерсеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b3df-127">In the request body, supply a JSON representation for the deviceManagementIntegerSettingInstance object.</span></span>

<span data-ttu-id="4b3df-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтежерсеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="4b3df-128">The following table shows the properties that are required when you create the deviceManagementIntegerSettingInstance.</span></span>

|<span data-ttu-id="4b3df-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b3df-129">Property</span></span>|<span data-ttu-id="4b3df-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4b3df-130">Type</span></span>|<span data-ttu-id="4b3df-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4b3df-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b3df-132">id</span><span class="sxs-lookup"><span data-stu-id="4b3df-132">id</span></span>|<span data-ttu-id="4b3df-133">String</span><span class="sxs-lookup"><span data-stu-id="4b3df-133">String</span></span>|<span data-ttu-id="4b3df-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4b3df-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="4b3df-135">Дефинитионид</span><span class="sxs-lookup"><span data-stu-id="4b3df-135">definitionId</span></span>|<span data-ttu-id="4b3df-136">String</span><span class="sxs-lookup"><span data-stu-id="4b3df-136">String</span></span>|<span data-ttu-id="4b3df-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4b3df-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="4b3df-138">Валуежсон</span><span class="sxs-lookup"><span data-stu-id="4b3df-138">valueJson</span></span>|<span data-ttu-id="4b3df-139">String</span><span class="sxs-lookup"><span data-stu-id="4b3df-139">String</span></span>|<span data-ttu-id="4b3df-140">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4b3df-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="4b3df-141">value</span><span class="sxs-lookup"><span data-stu-id="4b3df-141">value</span></span>|<span data-ttu-id="4b3df-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4b3df-142">Int32</span></span>|<span data-ttu-id="4b3df-143">Целое значение</span><span class="sxs-lookup"><span data-stu-id="4b3df-143">The integer value</span></span>|



## <a name="response"></a><span data-ttu-id="4b3df-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b3df-144">Response</span></span>
<span data-ttu-id="4b3df-145">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b3df-145">If successful, this method returns a `201 Created` response code and a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b3df-146">Пример</span><span class="sxs-lookup"><span data-stu-id="4b3df-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b3df-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b3df-147">Request</span></span>
<span data-ttu-id="4b3df-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b3df-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="4b3df-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b3df-149">Response</span></span>
<span data-ttu-id="4b3df-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b3df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





