---
title: Обновление Девицеманажементбулеансеттингинстанце
description: Обновление свойств объекта Девицеманажементбулеансеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab568b8f882487156212805e76c9786948b95d0c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960890"
---
# <a name="update-devicemanagementbooleansettinginstance"></a><span data-ttu-id="9f4db-103">Обновление Девицеманажементбулеансеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="9f4db-103">Update deviceManagementBooleanSettingInstance</span></span>

> <span data-ttu-id="9f4db-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f4db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f4db-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f4db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f4db-106">Обновление свойств объекта [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="9f4db-106">Update the properties of a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f4db-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f4db-107">Prerequisites</span></span>
<span data-ttu-id="9f4db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f4db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f4db-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f4db-110">Permission type</span></span>|<span data-ttu-id="9f4db-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f4db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f4db-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f4db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f4db-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f4db-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f4db-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f4db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f4db-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f4db-115">Not supported.</span></span>|
|<span data-ttu-id="9f4db-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f4db-116">Application</span></span>|<span data-ttu-id="9f4db-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f4db-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f4db-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f4db-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9f4db-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f4db-119">Request headers</span></span>
|<span data-ttu-id="9f4db-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f4db-120">Header</span></span>|<span data-ttu-id="9f4db-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9f4db-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f4db-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f4db-122">Authorization</span></span>|<span data-ttu-id="9f4db-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f4db-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f4db-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9f4db-124">Accept</span></span>|<span data-ttu-id="9f4db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f4db-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f4db-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f4db-126">Request body</span></span>
<span data-ttu-id="9f4db-127">В тексте запроса добавьте представление объекта [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f4db-127">In the request body, supply a JSON representation for the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

<span data-ttu-id="9f4db-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="9f4db-128">The following table shows the properties that are required when you create the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).</span></span>

|<span data-ttu-id="9f4db-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f4db-129">Property</span></span>|<span data-ttu-id="9f4db-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9f4db-130">Type</span></span>|<span data-ttu-id="9f4db-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9f4db-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f4db-132">id</span><span class="sxs-lookup"><span data-stu-id="9f4db-132">id</span></span>|<span data-ttu-id="9f4db-133">String</span><span class="sxs-lookup"><span data-stu-id="9f4db-133">String</span></span>|<span data-ttu-id="9f4db-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="9f4db-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="9f4db-135">Дефинитионид</span><span class="sxs-lookup"><span data-stu-id="9f4db-135">definitionId</span></span>|<span data-ttu-id="9f4db-136">String</span><span class="sxs-lookup"><span data-stu-id="9f4db-136">String</span></span>|<span data-ttu-id="9f4db-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="9f4db-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="9f4db-138">Валуежсон</span><span class="sxs-lookup"><span data-stu-id="9f4db-138">valueJson</span></span>|<span data-ttu-id="9f4db-139">String</span><span class="sxs-lookup"><span data-stu-id="9f4db-139">String</span></span>|<span data-ttu-id="9f4db-140">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="9f4db-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="9f4db-141">value</span><span class="sxs-lookup"><span data-stu-id="9f4db-141">value</span></span>|<span data-ttu-id="9f4db-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f4db-142">Boolean</span></span>|<span data-ttu-id="9f4db-143">Логическое значение</span><span class="sxs-lookup"><span data-stu-id="9f4db-143">The boolean value</span></span>|



## <a name="response"></a><span data-ttu-id="9f4db-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f4db-144">Response</span></span>
<span data-ttu-id="9f4db-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементбулеансеттингинстанце](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f4db-145">If successful, this method returns a `200 OK` response code and an updated [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f4db-146">Пример</span><span class="sxs-lookup"><span data-stu-id="9f4db-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f4db-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f4db-147">Request</span></span>
<span data-ttu-id="9f4db-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f4db-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f4db-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f4db-149">Response</span></span>
<span data-ttu-id="9f4db-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f4db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





