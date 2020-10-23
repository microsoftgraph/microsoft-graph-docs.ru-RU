---
title: Обновление Девицеманажементколлектионсеттингинстанце
description: Обновление свойств объекта Девицеманажементколлектионсеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f00648ec49d0bcc628611b6d3d8990e5b5327d8f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736536"
---
# <a name="update-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="3fe89-103">Обновление Девицеманажементколлектионсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="3fe89-103">Update deviceManagementCollectionSettingInstance</span></span>

<span data-ttu-id="3fe89-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fe89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3fe89-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fe89-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fe89-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3fe89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fe89-107">Обновление свойств объекта [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="3fe89-107">Update the properties of a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fe89-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3fe89-108">Prerequisites</span></span>
<span data-ttu-id="3fe89-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fe89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fe89-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fe89-111">Permission type</span></span>|<span data-ttu-id="3fe89-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fe89-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fe89-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fe89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3fe89-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fe89-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3fe89-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fe89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fe89-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fe89-116">Not supported.</span></span>|
|<span data-ttu-id="3fe89-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fe89-117">Application</span></span>|<span data-ttu-id="3fe89-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fe89-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fe89-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fe89-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="3fe89-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3fe89-120">Request headers</span></span>
|<span data-ttu-id="3fe89-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3fe89-121">Header</span></span>|<span data-ttu-id="3fe89-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3fe89-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fe89-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3fe89-123">Authorization</span></span>|<span data-ttu-id="3fe89-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fe89-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fe89-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3fe89-125">Accept</span></span>|<span data-ttu-id="3fe89-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3fe89-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fe89-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3fe89-127">Request body</span></span>
<span data-ttu-id="3fe89-128">В тексте запроса добавьте представление объекта [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fe89-128">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

<span data-ttu-id="3fe89-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="3fe89-129">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).</span></span>

|<span data-ttu-id="3fe89-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fe89-130">Property</span></span>|<span data-ttu-id="3fe89-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3fe89-131">Type</span></span>|<span data-ttu-id="3fe89-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3fe89-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fe89-133">id</span><span class="sxs-lookup"><span data-stu-id="3fe89-133">id</span></span>|<span data-ttu-id="3fe89-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3fe89-134">String</span></span>|<span data-ttu-id="3fe89-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="3fe89-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="3fe89-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="3fe89-136">definitionId</span></span>|<span data-ttu-id="3fe89-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3fe89-137">String</span></span>|<span data-ttu-id="3fe89-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="3fe89-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="3fe89-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="3fe89-139">valueJson</span></span>|<span data-ttu-id="3fe89-140">Строка</span><span class="sxs-lookup"><span data-stu-id="3fe89-140">String</span></span>|<span data-ttu-id="3fe89-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="3fe89-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="3fe89-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="3fe89-142">Response</span></span>
<span data-ttu-id="3fe89-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3fe89-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fe89-144">Пример</span><span class="sxs-lookup"><span data-stu-id="3fe89-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fe89-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fe89-145">Request</span></span>
<span data-ttu-id="3fe89-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fe89-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="3fe89-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fe89-147">Response</span></span>
<span data-ttu-id="3fe89-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3fe89-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "id": "6ce278f7-78f7-6ce2-f778-e26cf778e26c",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```





