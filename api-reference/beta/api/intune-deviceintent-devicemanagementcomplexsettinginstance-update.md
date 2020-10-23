---
title: Обновление Девицеманажементкомплекссеттингинстанце
description: Обновление свойств объекта Девицеманажементкомплекссеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8678509bd08b6e15aedf8059fc443bbee554a6be
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704121"
---
# <a name="update-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="99014-103">Обновление Девицеманажементкомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="99014-103">Update deviceManagementComplexSettingInstance</span></span>

<span data-ttu-id="99014-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99014-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99014-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99014-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99014-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99014-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99014-107">Обновление свойств объекта [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="99014-107">Update the properties of a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99014-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="99014-108">Prerequisites</span></span>
<span data-ttu-id="99014-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99014-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99014-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99014-111">Permission type</span></span>|<span data-ttu-id="99014-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="99014-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99014-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99014-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99014-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99014-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="99014-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99014-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99014-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99014-116">Not supported.</span></span>|
|<span data-ttu-id="99014-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99014-117">Application</span></span>|<span data-ttu-id="99014-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99014-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99014-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99014-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="99014-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="99014-120">Request headers</span></span>
|<span data-ttu-id="99014-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99014-121">Header</span></span>|<span data-ttu-id="99014-122">Значение</span><span class="sxs-lookup"><span data-stu-id="99014-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99014-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99014-123">Authorization</span></span>|<span data-ttu-id="99014-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99014-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99014-125">Accept</span><span class="sxs-lookup"><span data-stu-id="99014-125">Accept</span></span>|<span data-ttu-id="99014-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99014-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99014-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="99014-127">Request body</span></span>
<span data-ttu-id="99014-128">В тексте запроса добавьте представление объекта [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99014-128">In the request body, supply a JSON representation for the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="99014-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="99014-129">The following table shows the properties that are required when you create the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="99014-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="99014-130">Property</span></span>|<span data-ttu-id="99014-131">Тип</span><span class="sxs-lookup"><span data-stu-id="99014-131">Type</span></span>|<span data-ttu-id="99014-132">Описание</span><span class="sxs-lookup"><span data-stu-id="99014-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99014-133">id</span><span class="sxs-lookup"><span data-stu-id="99014-133">id</span></span>|<span data-ttu-id="99014-134">Строка</span><span class="sxs-lookup"><span data-stu-id="99014-134">String</span></span>|<span data-ttu-id="99014-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="99014-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="99014-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="99014-136">definitionId</span></span>|<span data-ttu-id="99014-137">Строка</span><span class="sxs-lookup"><span data-stu-id="99014-137">String</span></span>|<span data-ttu-id="99014-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="99014-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="99014-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="99014-139">valueJson</span></span>|<span data-ttu-id="99014-140">Строка</span><span class="sxs-lookup"><span data-stu-id="99014-140">String</span></span>|<span data-ttu-id="99014-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="99014-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="99014-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="99014-142">Response</span></span>
<span data-ttu-id="99014-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементкомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="99014-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99014-144">Пример</span><span class="sxs-lookup"><span data-stu-id="99014-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="99014-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="99014-145">Request</span></span>
<span data-ttu-id="99014-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99014-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="99014-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="99014-147">Response</span></span>
<span data-ttu-id="99014-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="99014-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





