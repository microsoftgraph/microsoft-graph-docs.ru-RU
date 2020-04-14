---
title: Создание Граупполиципресентатиондропдовнлист
description: Создание нового объекта Граупполиципресентатиондропдовнлист.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f265451d7de34d3a77a39cf95a72a3f27da3f362
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43424372"
---
# <a name="create-grouppolicypresentationdropdownlist"></a><span data-ttu-id="5f1c9-103">Создание Граупполиципресентатиондропдовнлист</span><span class="sxs-lookup"><span data-stu-id="5f1c9-103">Create groupPolicyPresentationDropdownList</span></span>

<span data-ttu-id="5f1c9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f1c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f1c9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f1c9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f1c9-107">Создание нового объекта [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .</span><span class="sxs-lookup"><span data-stu-id="5f1c9-107">Create a new [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f1c9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5f1c9-108">Prerequisites</span></span>
<span data-ttu-id="5f1c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f1c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f1c9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f1c9-111">Permission type</span></span>|<span data-ttu-id="5f1c9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f1c9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f1c9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f1c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5f1c9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f1c9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5f1c9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f1c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f1c9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-116">Not supported.</span></span>|
|<span data-ttu-id="5f1c9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5f1c9-117">Application</span></span>|<span data-ttu-id="5f1c9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f1c9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f1c9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f1c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="5f1c9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5f1c9-120">Request headers</span></span>
|<span data-ttu-id="5f1c9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5f1c9-121">Header</span></span>|<span data-ttu-id="5f1c9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5f1c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f1c9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f1c9-123">Authorization</span></span>|<span data-ttu-id="5f1c9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f1c9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5f1c9-125">Accept</span></span>|<span data-ttu-id="5f1c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f1c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f1c9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f1c9-127">Request body</span></span>
<span data-ttu-id="5f1c9-128">В тексте запроса добавьте представление объекта Граупполиципресентатиондропдовнлист в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-128">In the request body, supply a JSON representation for the groupPolicyPresentationDropdownList object.</span></span>

<span data-ttu-id="5f1c9-129">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатиондропдовнлист.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-129">The following table shows the properties that are required when you create the groupPolicyPresentationDropdownList.</span></span>

|<span data-ttu-id="5f1c9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f1c9-130">Property</span></span>|<span data-ttu-id="5f1c9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5f1c9-131">Type</span></span>|<span data-ttu-id="5f1c9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5f1c9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f1c9-133">label</span><span class="sxs-lookup"><span data-stu-id="5f1c9-133">label</span></span>|<span data-ttu-id="5f1c9-134">String</span><span class="sxs-lookup"><span data-stu-id="5f1c9-134">String</span></span>|<span data-ttu-id="5f1c9-135">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="5f1c9-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-136">The default value is empty.</span></span> <span data-ttu-id="5f1c9-137">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="5f1c9-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="5f1c9-138">id</span><span class="sxs-lookup"><span data-stu-id="5f1c9-138">id</span></span>|<span data-ttu-id="5f1c9-139">String</span><span class="sxs-lookup"><span data-stu-id="5f1c9-139">String</span></span>|<span data-ttu-id="5f1c9-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-140">Key of the entity.</span></span> <span data-ttu-id="5f1c9-141">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="5f1c9-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="5f1c9-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f1c9-142">lastModifiedDateTime</span></span>|<span data-ttu-id="5f1c9-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f1c9-143">DateTimeOffset</span></span>|<span data-ttu-id="5f1c9-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="5f1c9-145">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="5f1c9-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="5f1c9-146">дефаултитем</span><span class="sxs-lookup"><span data-stu-id="5f1c9-146">defaultItem</span></span>|[<span data-ttu-id="5f1c9-147">граупполиципресентатиондропдовнлиститем</span><span class="sxs-lookup"><span data-stu-id="5f1c9-147">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="5f1c9-148">Локализованное строковое значение, определяющее вариант списка элементов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-148">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="5f1c9-149">items</span><span class="sxs-lookup"><span data-stu-id="5f1c9-149">items</span></span>|<span data-ttu-id="5f1c9-150">Коллекция [граупполиципресентатиондропдовнлиститем](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)</span><span class="sxs-lookup"><span data-stu-id="5f1c9-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="5f1c9-151">Представляет набор локализованных отображаемых имен и связанных с ними значений.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-151">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="5f1c9-152">Обязательный</span><span class="sxs-lookup"><span data-stu-id="5f1c9-152">required</span></span>|<span data-ttu-id="5f1c9-153">Логическое</span><span class="sxs-lookup"><span data-stu-id="5f1c9-153">Boolean</span></span>|<span data-ttu-id="5f1c9-154">Требование ввести значение в поле параметр.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-154">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="5f1c9-155">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-155">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="5f1c9-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f1c9-156">Response</span></span>
<span data-ttu-id="5f1c9-157">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-157">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f1c9-158">Пример</span><span class="sxs-lookup"><span data-stu-id="5f1c9-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f1c9-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f1c9-159">Request</span></span>
<span data-ttu-id="5f1c9-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 489

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "Label value",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "Display Name value",
    "value": "Value value"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    }
  ],
  "required": true
}
```

### <a name="response"></a><span data-ttu-id="5f1c9-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f1c9-161">Response</span></span>
<span data-ttu-id="5f1c9-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5f1c9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 602

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "Label value",
  "id": "ba3ff7c9-f7c9-ba3f-c9f7-3fbac9f73fba",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "Display Name value",
    "value": "Value value"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    }
  ],
  "required": true
}
```



