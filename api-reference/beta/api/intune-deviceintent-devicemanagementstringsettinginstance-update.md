---
title: Обновление deviceManagementStringSettingInstance
description: Обновление свойств объекта deviceManagementStringSettingInstance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9094bb663e3080177da82589b165ba539b360a14
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150740"
---
# <a name="update-devicemanagementstringsettinginstance"></a><span data-ttu-id="1f0c4-103">Обновление deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="1f0c4-103">Update deviceManagementStringSettingInstance</span></span>

<span data-ttu-id="1f0c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f0c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f0c4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f0c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f0c4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f0c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f0c4-107">Обновление свойств объекта [deviceManagementStringSettingInstance.](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="1f0c4-107">Update the properties of a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f0c4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1f0c4-108">Prerequisites</span></span>
<span data-ttu-id="1f0c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f0c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f0c4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f0c4-111">Permission type</span></span>|<span data-ttu-id="1f0c4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f0c4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f0c4-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f0c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f0c4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f0c4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f0c4-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f0c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f0c4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f0c4-116">Not supported.</span></span>|
|<span data-ttu-id="1f0c4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1f0c4-117">Application</span></span>|<span data-ttu-id="1f0c4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f0c4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f0c4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f0c4-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="1f0c4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1f0c4-120">Request headers</span></span>
|<span data-ttu-id="1f0c4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f0c4-121">Header</span></span>|<span data-ttu-id="1f0c4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1f0c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f0c4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f0c4-123">Authorization</span></span>|<span data-ttu-id="1f0c4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f0c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f0c4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1f0c4-125">Accept</span></span>|<span data-ttu-id="1f0c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f0c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f0c4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f0c4-127">Request body</span></span>
<span data-ttu-id="1f0c4-128">В теле запроса поставляем представление JSON для [объекта deviceManagementStringSettingInstance.](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="1f0c4-128">In the request body, supply a JSON representation for the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

<span data-ttu-id="1f0c4-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementStringSettingInstance.](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="1f0c4-129">The following table shows the properties that are required when you create the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).</span></span>

|<span data-ttu-id="1f0c4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f0c4-130">Property</span></span>|<span data-ttu-id="1f0c4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1f0c4-131">Type</span></span>|<span data-ttu-id="1f0c4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1f0c4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f0c4-133">id</span><span class="sxs-lookup"><span data-stu-id="1f0c4-133">id</span></span>|<span data-ttu-id="1f0c4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1f0c4-134">String</span></span>|<span data-ttu-id="1f0c4-135">ID экземпляра параметра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="1f0c4-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="1f0c4-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="1f0c4-136">definitionId</span></span>|<span data-ttu-id="1f0c4-137">Строка</span><span class="sxs-lookup"><span data-stu-id="1f0c4-137">String</span></span>|<span data-ttu-id="1f0c4-138">ID определения параметра для этого экземпляра, унаследованный от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="1f0c4-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="1f0c4-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="1f0c4-139">valueJson</span></span>|<span data-ttu-id="1f0c4-140">Строка</span><span class="sxs-lookup"><span data-stu-id="1f0c4-140">String</span></span>|<span data-ttu-id="1f0c4-141">Представление JSON значения, унаследованной от [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="1f0c4-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="1f0c4-142">value</span><span class="sxs-lookup"><span data-stu-id="1f0c4-142">value</span></span>|<span data-ttu-id="1f0c4-143">String</span><span class="sxs-lookup"><span data-stu-id="1f0c4-143">String</span></span>|<span data-ttu-id="1f0c4-144">Значение строки</span><span class="sxs-lookup"><span data-stu-id="1f0c4-144">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="1f0c4-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f0c4-145">Response</span></span>
<span data-ttu-id="1f0c4-146">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1f0c4-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f0c4-147">Пример</span><span class="sxs-lookup"><span data-stu-id="1f0c4-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f0c4-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f0c4-148">Request</span></span>
<span data-ttu-id="1f0c4-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f0c4-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1f0c4-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f0c4-150">Response</span></span>
<span data-ttu-id="1f0c4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f0c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




