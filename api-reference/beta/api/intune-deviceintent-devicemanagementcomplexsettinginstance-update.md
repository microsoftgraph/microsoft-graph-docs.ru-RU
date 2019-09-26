---
title: Обновление Девицеманажементкомплекссеттингинстанце
description: Обновление свойств объекта Девицеманажементкомплекссеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7bd5025f3b81b0ddc71cfebf29c83913f4c657c5
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37181051"
---
# <a name="update-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="17eaa-103">Обновление Девицеманажементкомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="17eaa-103">Update deviceManagementComplexSettingInstance</span></span>

> <span data-ttu-id="17eaa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17eaa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17eaa-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17eaa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17eaa-106">Обновление свойств объекта [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="17eaa-106">Update the properties of a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17eaa-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="17eaa-107">Prerequisites</span></span>
<span data-ttu-id="17eaa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17eaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17eaa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17eaa-110">Permission type</span></span>|<span data-ttu-id="17eaa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="17eaa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17eaa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17eaa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17eaa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17eaa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17eaa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17eaa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17eaa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17eaa-115">Not supported.</span></span>|
|<span data-ttu-id="17eaa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17eaa-116">Application</span></span>|<span data-ttu-id="17eaa-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17eaa-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17eaa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17eaa-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="17eaa-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17eaa-119">Request headers</span></span>
|<span data-ttu-id="17eaa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17eaa-120">Header</span></span>|<span data-ttu-id="17eaa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="17eaa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17eaa-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17eaa-122">Authorization</span></span>|<span data-ttu-id="17eaa-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17eaa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17eaa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="17eaa-124">Accept</span></span>|<span data-ttu-id="17eaa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="17eaa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17eaa-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="17eaa-126">Request body</span></span>
<span data-ttu-id="17eaa-127">В тексте запроса добавьте представление объекта [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17eaa-127">In the request body, supply a JSON representation for the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="17eaa-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="17eaa-128">The following table shows the properties that are required when you create the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="17eaa-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="17eaa-129">Property</span></span>|<span data-ttu-id="17eaa-130">Тип</span><span class="sxs-lookup"><span data-stu-id="17eaa-130">Type</span></span>|<span data-ttu-id="17eaa-131">Описание</span><span class="sxs-lookup"><span data-stu-id="17eaa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17eaa-132">id</span><span class="sxs-lookup"><span data-stu-id="17eaa-132">id</span></span>|<span data-ttu-id="17eaa-133">String</span><span class="sxs-lookup"><span data-stu-id="17eaa-133">String</span></span>|<span data-ttu-id="17eaa-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="17eaa-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="17eaa-135">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="17eaa-135">definitionId</span></span>|<span data-ttu-id="17eaa-136">String.</span><span class="sxs-lookup"><span data-stu-id="17eaa-136">String</span></span>|<span data-ttu-id="17eaa-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="17eaa-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="17eaa-138">валуежсон</span><span class="sxs-lookup"><span data-stu-id="17eaa-138">valueJson</span></span>|<span data-ttu-id="17eaa-139">String.</span><span class="sxs-lookup"><span data-stu-id="17eaa-139">String</span></span>|<span data-ttu-id="17eaa-140">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="17eaa-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="17eaa-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="17eaa-141">Response</span></span>
<span data-ttu-id="17eaa-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="17eaa-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17eaa-143">Пример</span><span class="sxs-lookup"><span data-stu-id="17eaa-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="17eaa-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="17eaa-144">Request</span></span>
<span data-ttu-id="17eaa-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17eaa-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="17eaa-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="17eaa-146">Response</span></span>
<span data-ttu-id="17eaa-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17eaa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 207

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "id": "4deb3935-3935-4deb-3539-eb4d3539eb4d",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```




