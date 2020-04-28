---
title: Обновление Девицеманажементкомплекссеттингинстанце
description: Обновление свойств объекта Девицеманажементкомплекссеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac459fbc02a57ec0a759ce1bdf530e292e4ef090
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43329059"
---
# <a name="update-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="4e413-103">Обновление Девицеманажементкомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="4e413-103">Update deviceManagementComplexSettingInstance</span></span>

<span data-ttu-id="4e413-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e413-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e413-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e413-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e413-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e413-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e413-107">Обновление свойств объекта [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="4e413-107">Update the properties of a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e413-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4e413-108">Prerequisites</span></span>
<span data-ttu-id="4e413-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e413-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e413-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e413-111">Permission type</span></span>|<span data-ttu-id="4e413-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e413-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e413-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e413-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e413-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e413-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4e413-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e413-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e413-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e413-116">Not supported.</span></span>|
|<span data-ttu-id="4e413-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e413-117">Application</span></span>|<span data-ttu-id="4e413-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e413-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e413-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e413-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4e413-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4e413-120">Request headers</span></span>
|<span data-ttu-id="4e413-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e413-121">Header</span></span>|<span data-ttu-id="4e413-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4e413-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e413-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e413-123">Authorization</span></span>|<span data-ttu-id="4e413-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e413-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e413-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e413-125">Accept</span></span>|<span data-ttu-id="4e413-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e413-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e413-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e413-127">Request body</span></span>
<span data-ttu-id="4e413-128">В тексте запроса добавьте представление объекта [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e413-128">In the request body, supply a JSON representation for the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="4e413-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="4e413-129">The following table shows the properties that are required when you create the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="4e413-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e413-130">Property</span></span>|<span data-ttu-id="4e413-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4e413-131">Type</span></span>|<span data-ttu-id="4e413-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4e413-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e413-133">id</span><span class="sxs-lookup"><span data-stu-id="4e413-133">id</span></span>|<span data-ttu-id="4e413-134">String</span><span class="sxs-lookup"><span data-stu-id="4e413-134">String</span></span>|<span data-ttu-id="4e413-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4e413-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="4e413-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="4e413-136">definitionId</span></span>|<span data-ttu-id="4e413-137">String</span><span class="sxs-lookup"><span data-stu-id="4e413-137">String</span></span>|<span data-ttu-id="4e413-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4e413-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="4e413-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="4e413-139">valueJson</span></span>|<span data-ttu-id="4e413-140">String</span><span class="sxs-lookup"><span data-stu-id="4e413-140">String</span></span>|<span data-ttu-id="4e413-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4e413-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4e413-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e413-142">Response</span></span>
<span data-ttu-id="4e413-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e413-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e413-144">Пример</span><span class="sxs-lookup"><span data-stu-id="4e413-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e413-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e413-145">Request</span></span>
<span data-ttu-id="4e413-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e413-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4e413-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e413-147">Response</span></span>
<span data-ttu-id="4e413-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e413-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



