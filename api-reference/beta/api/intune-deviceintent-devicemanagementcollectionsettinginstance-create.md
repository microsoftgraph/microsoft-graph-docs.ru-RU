---
title: Создание Девицеманажементколлектионсеттингинстанце
description: Создание нового объекта Девицеманажементколлектионсеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f576701930790461fd8865a35e61aacccb3e1cc2
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946107"
---
# <a name="create-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="d78a4-103">Создание Девицеманажементколлектионсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="d78a4-103">Create deviceManagementCollectionSettingInstance</span></span>

> <span data-ttu-id="d78a4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d78a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d78a4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d78a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d78a4-106">Создание нового объекта [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="d78a4-106">Create a new [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d78a4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d78a4-107">Prerequisites</span></span>
<span data-ttu-id="d78a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d78a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d78a4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d78a4-110">Permission type</span></span>|<span data-ttu-id="d78a4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d78a4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d78a4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d78a4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d78a4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d78a4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d78a4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d78a4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d78a4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d78a4-115">Not supported.</span></span>|
|<span data-ttu-id="d78a4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d78a4-116">Application</span></span>|<span data-ttu-id="d78a4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d78a4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d78a4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d78a4-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d78a4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d78a4-119">Request headers</span></span>
|<span data-ttu-id="d78a4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d78a4-120">Header</span></span>|<span data-ttu-id="d78a4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d78a4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d78a4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d78a4-122">Authorization</span></span>|<span data-ttu-id="d78a4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d78a4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d78a4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d78a4-124">Accept</span></span>|<span data-ttu-id="d78a4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d78a4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d78a4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d78a4-126">Request body</span></span>
<span data-ttu-id="d78a4-127">В тексте запроса добавьте представление объекта Девицеманажементколлектионсеттингинстанце в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d78a4-127">In the request body, supply a JSON representation for the deviceManagementCollectionSettingInstance object.</span></span>

<span data-ttu-id="d78a4-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементколлектионсеттингинстанце.</span><span class="sxs-lookup"><span data-stu-id="d78a4-128">The following table shows the properties that are required when you create the deviceManagementCollectionSettingInstance.</span></span>

|<span data-ttu-id="d78a4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d78a4-129">Property</span></span>|<span data-ttu-id="d78a4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d78a4-130">Type</span></span>|<span data-ttu-id="d78a4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d78a4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d78a4-132">id</span><span class="sxs-lookup"><span data-stu-id="d78a4-132">id</span></span>|<span data-ttu-id="d78a4-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d78a4-133">String</span></span>|<span data-ttu-id="d78a4-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d78a4-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="d78a4-135">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="d78a4-135">definitionId</span></span>|<span data-ttu-id="d78a4-136">Строка</span><span class="sxs-lookup"><span data-stu-id="d78a4-136">String</span></span>|<span data-ttu-id="d78a4-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d78a4-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="d78a4-138">валуежсон</span><span class="sxs-lookup"><span data-stu-id="d78a4-138">valueJson</span></span>|<span data-ttu-id="d78a4-139">Строка</span><span class="sxs-lookup"><span data-stu-id="d78a4-139">String</span></span>|<span data-ttu-id="d78a4-140">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d78a4-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d78a4-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="d78a4-141">Response</span></span>
<span data-ttu-id="d78a4-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d78a4-142">If successful, this method returns a `201 Created` response code and a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d78a4-143">Пример</span><span class="sxs-lookup"><span data-stu-id="d78a4-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="d78a4-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="d78a4-144">Request</span></span>
<span data-ttu-id="d78a4-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d78a4-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="d78a4-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="d78a4-146">Response</span></span>
<span data-ttu-id="d78a4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d78a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "id": "6ce278f7-78f7-6ce2-f778-e26cf778e26c",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```





