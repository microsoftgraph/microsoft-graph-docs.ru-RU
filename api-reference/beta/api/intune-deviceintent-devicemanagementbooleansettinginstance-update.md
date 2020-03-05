---
title: Обновление Девицеманажементбулеансеттингинстанце
description: Обновление свойств объекта Девицеманажементбулеансеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1e19f2d339c82a73d0bf2f0d762673907f72f373
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42472655"
---
# <a name="update-devicemanagementbooleansettinginstance"></a><span data-ttu-id="912e1-103">Обновление Девицеманажементбулеансеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="912e1-103">Update deviceManagementBooleanSettingInstance</span></span>

<span data-ttu-id="912e1-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="912e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="912e1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="912e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="912e1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="912e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="912e1-107">Обновление свойств объекта [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="912e1-107">Update the properties of a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="912e1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="912e1-108">Prerequisites</span></span>
<span data-ttu-id="912e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="912e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="912e1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="912e1-111">Permission type</span></span>|<span data-ttu-id="912e1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="912e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="912e1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="912e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="912e1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="912e1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="912e1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="912e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="912e1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="912e1-116">Not supported.</span></span>|
|<span data-ttu-id="912e1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="912e1-117">Application</span></span>|<span data-ttu-id="912e1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="912e1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="912e1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="912e1-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="912e1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="912e1-120">Request headers</span></span>
|<span data-ttu-id="912e1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="912e1-121">Header</span></span>|<span data-ttu-id="912e1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="912e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="912e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="912e1-123">Authorization</span></span>|<span data-ttu-id="912e1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="912e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="912e1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="912e1-125">Accept</span></span>|<span data-ttu-id="912e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="912e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="912e1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="912e1-127">Request body</span></span>
<span data-ttu-id="912e1-128">В тексте запроса добавьте представление объекта [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="912e1-128">In the request body, supply a JSON representation for the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

<span data-ttu-id="912e1-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="912e1-129">The following table shows the properties that are required when you create the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).</span></span>

|<span data-ttu-id="912e1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="912e1-130">Property</span></span>|<span data-ttu-id="912e1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="912e1-131">Type</span></span>|<span data-ttu-id="912e1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="912e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="912e1-133">id</span><span class="sxs-lookup"><span data-stu-id="912e1-133">id</span></span>|<span data-ttu-id="912e1-134">String</span><span class="sxs-lookup"><span data-stu-id="912e1-134">String</span></span>|<span data-ttu-id="912e1-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="912e1-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="912e1-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="912e1-136">definitionId</span></span>|<span data-ttu-id="912e1-137">String</span><span class="sxs-lookup"><span data-stu-id="912e1-137">String</span></span>|<span data-ttu-id="912e1-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="912e1-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="912e1-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="912e1-139">valueJson</span></span>|<span data-ttu-id="912e1-140">String</span><span class="sxs-lookup"><span data-stu-id="912e1-140">String</span></span>|<span data-ttu-id="912e1-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="912e1-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="912e1-142">value</span><span class="sxs-lookup"><span data-stu-id="912e1-142">value</span></span>|<span data-ttu-id="912e1-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="912e1-143">Boolean</span></span>|<span data-ttu-id="912e1-144">Логическое значение</span><span class="sxs-lookup"><span data-stu-id="912e1-144">The boolean value</span></span>|



## <a name="response"></a><span data-ttu-id="912e1-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="912e1-145">Response</span></span>
<span data-ttu-id="912e1-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="912e1-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="912e1-147">Пример</span><span class="sxs-lookup"><span data-stu-id="912e1-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="912e1-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="912e1-148">Request</span></span>
<span data-ttu-id="912e1-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="912e1-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 176

{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="912e1-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="912e1-150">Response</span></span>
<span data-ttu-id="912e1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="912e1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





