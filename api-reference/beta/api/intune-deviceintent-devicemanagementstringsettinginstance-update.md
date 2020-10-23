---
title: Обновление Девицеманажементстрингсеттингинстанце
description: Обновление свойств объекта Девицеманажементстрингсеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f76f20a5a7b7ccd1f1be6eae2d049acc0f395048
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735941"
---
# <a name="update-devicemanagementstringsettinginstance"></a><span data-ttu-id="443ce-103">Обновление Девицеманажементстрингсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="443ce-103">Update deviceManagementStringSettingInstance</span></span>

<span data-ttu-id="443ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="443ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="443ce-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="443ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="443ce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="443ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="443ce-107">Обновление свойств объекта [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="443ce-107">Update the properties of a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="443ce-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="443ce-108">Prerequisites</span></span>
<span data-ttu-id="443ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="443ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="443ce-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="443ce-111">Permission type</span></span>|<span data-ttu-id="443ce-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="443ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="443ce-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="443ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="443ce-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="443ce-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="443ce-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="443ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="443ce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="443ce-116">Not supported.</span></span>|
|<span data-ttu-id="443ce-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="443ce-117">Application</span></span>|<span data-ttu-id="443ce-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="443ce-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="443ce-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="443ce-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="443ce-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="443ce-120">Request headers</span></span>
|<span data-ttu-id="443ce-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="443ce-121">Header</span></span>|<span data-ttu-id="443ce-122">Значение</span><span class="sxs-lookup"><span data-stu-id="443ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="443ce-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="443ce-123">Authorization</span></span>|<span data-ttu-id="443ce-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="443ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="443ce-125">Accept</span><span class="sxs-lookup"><span data-stu-id="443ce-125">Accept</span></span>|<span data-ttu-id="443ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="443ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="443ce-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="443ce-127">Request body</span></span>
<span data-ttu-id="443ce-128">В тексте запроса добавьте представление объекта [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="443ce-128">In the request body, supply a JSON representation for the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

<span data-ttu-id="443ce-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="443ce-129">The following table shows the properties that are required when you create the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).</span></span>

|<span data-ttu-id="443ce-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="443ce-130">Property</span></span>|<span data-ttu-id="443ce-131">Тип</span><span class="sxs-lookup"><span data-stu-id="443ce-131">Type</span></span>|<span data-ttu-id="443ce-132">Описание</span><span class="sxs-lookup"><span data-stu-id="443ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="443ce-133">id</span><span class="sxs-lookup"><span data-stu-id="443ce-133">id</span></span>|<span data-ttu-id="443ce-134">Строка</span><span class="sxs-lookup"><span data-stu-id="443ce-134">String</span></span>|<span data-ttu-id="443ce-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="443ce-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="443ce-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="443ce-136">definitionId</span></span>|<span data-ttu-id="443ce-137">Строка</span><span class="sxs-lookup"><span data-stu-id="443ce-137">String</span></span>|<span data-ttu-id="443ce-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="443ce-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="443ce-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="443ce-139">valueJson</span></span>|<span data-ttu-id="443ce-140">Строка</span><span class="sxs-lookup"><span data-stu-id="443ce-140">String</span></span>|<span data-ttu-id="443ce-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="443ce-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="443ce-142">value</span><span class="sxs-lookup"><span data-stu-id="443ce-142">value</span></span>|<span data-ttu-id="443ce-143">String</span><span class="sxs-lookup"><span data-stu-id="443ce-143">String</span></span>|<span data-ttu-id="443ce-144">Строковое значение</span><span class="sxs-lookup"><span data-stu-id="443ce-144">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="443ce-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="443ce-145">Response</span></span>
<span data-ttu-id="443ce-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="443ce-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="443ce-147">Пример</span><span class="sxs-lookup"><span data-stu-id="443ce-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="443ce-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="443ce-148">Request</span></span>
<span data-ttu-id="443ce-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="443ce-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="443ce-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="443ce-150">Response</span></span>
<span data-ttu-id="443ce-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="443ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





