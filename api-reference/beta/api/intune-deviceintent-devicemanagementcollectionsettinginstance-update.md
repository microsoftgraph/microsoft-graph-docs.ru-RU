---
title: Обновление Девицеманажементколлектионсеттингинстанце
description: Обновление свойств объекта Девицеманажементколлектионсеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1e7b6b198ea1d17ffed1e9d662c9e17d97c7828a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946086"
---
# <a name="update-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="32aab-103">Обновление Девицеманажементколлектионсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="32aab-103">Update deviceManagementCollectionSettingInstance</span></span>

> <span data-ttu-id="32aab-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32aab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32aab-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32aab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32aab-106">Обновление свойств объекта [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="32aab-106">Update the properties of a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32aab-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="32aab-107">Prerequisites</span></span>
<span data-ttu-id="32aab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32aab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32aab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32aab-110">Permission type</span></span>|<span data-ttu-id="32aab-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32aab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32aab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32aab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32aab-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32aab-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32aab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32aab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32aab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32aab-115">Not supported.</span></span>|
|<span data-ttu-id="32aab-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32aab-116">Application</span></span>|<span data-ttu-id="32aab-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32aab-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32aab-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32aab-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="32aab-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="32aab-119">Request headers</span></span>
|<span data-ttu-id="32aab-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32aab-120">Header</span></span>|<span data-ttu-id="32aab-121">Значение</span><span class="sxs-lookup"><span data-stu-id="32aab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32aab-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32aab-122">Authorization</span></span>|<span data-ttu-id="32aab-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32aab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32aab-124">Accept</span><span class="sxs-lookup"><span data-stu-id="32aab-124">Accept</span></span>|<span data-ttu-id="32aab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32aab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32aab-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="32aab-126">Request body</span></span>
<span data-ttu-id="32aab-127">В тексте запроса добавьте представление объекта [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32aab-127">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

<span data-ttu-id="32aab-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="32aab-128">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).</span></span>

|<span data-ttu-id="32aab-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="32aab-129">Property</span></span>|<span data-ttu-id="32aab-130">Тип</span><span class="sxs-lookup"><span data-stu-id="32aab-130">Type</span></span>|<span data-ttu-id="32aab-131">Описание</span><span class="sxs-lookup"><span data-stu-id="32aab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32aab-132">id</span><span class="sxs-lookup"><span data-stu-id="32aab-132">id</span></span>|<span data-ttu-id="32aab-133">Строка</span><span class="sxs-lookup"><span data-stu-id="32aab-133">String</span></span>|<span data-ttu-id="32aab-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="32aab-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="32aab-135">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="32aab-135">definitionId</span></span>|<span data-ttu-id="32aab-136">Строка</span><span class="sxs-lookup"><span data-stu-id="32aab-136">String</span></span>|<span data-ttu-id="32aab-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="32aab-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="32aab-138">валуежсон</span><span class="sxs-lookup"><span data-stu-id="32aab-138">valueJson</span></span>|<span data-ttu-id="32aab-139">Строка</span><span class="sxs-lookup"><span data-stu-id="32aab-139">String</span></span>|<span data-ttu-id="32aab-140">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="32aab-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="32aab-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="32aab-141">Response</span></span>
<span data-ttu-id="32aab-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="32aab-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32aab-143">Пример</span><span class="sxs-lookup"><span data-stu-id="32aab-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="32aab-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="32aab-144">Request</span></span>
<span data-ttu-id="32aab-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32aab-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="32aab-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="32aab-146">Response</span></span>
<span data-ttu-id="32aab-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32aab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





