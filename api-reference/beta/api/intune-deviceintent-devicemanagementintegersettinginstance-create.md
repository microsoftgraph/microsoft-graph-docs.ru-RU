---
title: Создание Девицеманажементинтежерсеттингинстанце
description: Создание нового объекта Девицеманажементинтежерсеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d114a4632c9c2844a5863b58075c185e9a9f6bdc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42471878"
---
# <a name="create-devicemanagementintegersettinginstance"></a><span data-ttu-id="c35df-103">Создание Девицеманажементинтежерсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="c35df-103">Create deviceManagementIntegerSettingInstance</span></span>

<span data-ttu-id="c35df-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c35df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c35df-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c35df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c35df-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c35df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c35df-107">Создание нового объекта [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="c35df-107">Create a new [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c35df-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c35df-108">Prerequisites</span></span>
<span data-ttu-id="c35df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c35df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c35df-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c35df-111">Permission type</span></span>|<span data-ttu-id="c35df-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c35df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c35df-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c35df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c35df-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c35df-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c35df-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c35df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c35df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c35df-116">Not supported.</span></span>|
|<span data-ttu-id="c35df-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c35df-117">Application</span></span>|<span data-ttu-id="c35df-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c35df-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c35df-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c35df-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c35df-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c35df-120">Request headers</span></span>
|<span data-ttu-id="c35df-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c35df-121">Header</span></span>|<span data-ttu-id="c35df-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c35df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c35df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c35df-123">Authorization</span></span>|<span data-ttu-id="c35df-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c35df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c35df-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c35df-125">Accept</span></span>|<span data-ttu-id="c35df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c35df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c35df-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c35df-127">Request body</span></span>
<span data-ttu-id="c35df-128">В тексте запроса добавьте представление объекта Девицеманажементинтежерсеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c35df-128">In the request body, supply a JSON representation for the deviceManagementIntegerSettingInstance object.</span></span>

<span data-ttu-id="c35df-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтежерсеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="c35df-129">The following table shows the properties that are required when you create the deviceManagementIntegerSettingInstance.</span></span>

|<span data-ttu-id="c35df-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c35df-130">Property</span></span>|<span data-ttu-id="c35df-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c35df-131">Type</span></span>|<span data-ttu-id="c35df-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c35df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c35df-133">id</span><span class="sxs-lookup"><span data-stu-id="c35df-133">id</span></span>|<span data-ttu-id="c35df-134">String</span><span class="sxs-lookup"><span data-stu-id="c35df-134">String</span></span>|<span data-ttu-id="c35df-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="c35df-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="c35df-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="c35df-136">definitionId</span></span>|<span data-ttu-id="c35df-137">String</span><span class="sxs-lookup"><span data-stu-id="c35df-137">String</span></span>|<span data-ttu-id="c35df-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="c35df-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="c35df-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="c35df-139">valueJson</span></span>|<span data-ttu-id="c35df-140">String</span><span class="sxs-lookup"><span data-stu-id="c35df-140">String</span></span>|<span data-ttu-id="c35df-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="c35df-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="c35df-142">value</span><span class="sxs-lookup"><span data-stu-id="c35df-142">value</span></span>|<span data-ttu-id="c35df-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c35df-143">Int32</span></span>|<span data-ttu-id="c35df-144">Целое значение</span><span class="sxs-lookup"><span data-stu-id="c35df-144">The integer value</span></span>|



## <a name="response"></a><span data-ttu-id="c35df-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c35df-145">Response</span></span>
<span data-ttu-id="c35df-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c35df-146">If successful, this method returns a `201 Created` response code and a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c35df-147">Пример</span><span class="sxs-lookup"><span data-stu-id="c35df-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="c35df-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="c35df-148">Request</span></span>
<span data-ttu-id="c35df-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c35df-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c35df-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="c35df-150">Response</span></span>
<span data-ttu-id="c35df-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c35df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





