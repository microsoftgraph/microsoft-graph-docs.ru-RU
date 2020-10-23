---
title: Обновление Граупполиципресентатиондропдовнлист
description: Обновление свойств объекта Граупполиципресентатиондропдовнлист.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2e243176dd625bd777b337c7e44375a146e6fe34
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724679"
---
# <a name="update-grouppolicypresentationdropdownlist"></a><span data-ttu-id="3204e-103">Обновление Граупполиципресентатиондропдовнлист</span><span class="sxs-lookup"><span data-stu-id="3204e-103">Update groupPolicyPresentationDropdownList</span></span>

<span data-ttu-id="3204e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3204e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3204e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3204e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3204e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3204e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3204e-107">Обновление свойств объекта [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .</span><span class="sxs-lookup"><span data-stu-id="3204e-107">Update the properties of a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3204e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3204e-108">Prerequisites</span></span>
<span data-ttu-id="3204e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3204e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3204e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3204e-111">Permission type</span></span>|<span data-ttu-id="3204e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3204e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3204e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3204e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3204e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3204e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3204e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3204e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3204e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3204e-116">Not supported.</span></span>|
|<span data-ttu-id="3204e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3204e-117">Application</span></span>|<span data-ttu-id="3204e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3204e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3204e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3204e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="3204e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3204e-120">Request headers</span></span>
|<span data-ttu-id="3204e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3204e-121">Header</span></span>|<span data-ttu-id="3204e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3204e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3204e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3204e-123">Authorization</span></span>|<span data-ttu-id="3204e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3204e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3204e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3204e-125">Accept</span></span>|<span data-ttu-id="3204e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3204e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3204e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3204e-127">Request body</span></span>
<span data-ttu-id="3204e-128">В тексте запроса добавьте представление объекта [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3204e-128">In the request body, supply a JSON representation for the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

<span data-ttu-id="3204e-129">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span><span class="sxs-lookup"><span data-stu-id="3204e-129">The following table shows the properties that are required when you create the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span></span>

|<span data-ttu-id="3204e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3204e-130">Property</span></span>|<span data-ttu-id="3204e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3204e-131">Type</span></span>|<span data-ttu-id="3204e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3204e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3204e-133">label</span><span class="sxs-lookup"><span data-stu-id="3204e-133">label</span></span>|<span data-ttu-id="3204e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3204e-134">String</span></span>|<span data-ttu-id="3204e-135">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="3204e-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="3204e-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="3204e-136">The default value is empty.</span></span> <span data-ttu-id="3204e-137">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3204e-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="3204e-138">id</span><span class="sxs-lookup"><span data-stu-id="3204e-138">id</span></span>|<span data-ttu-id="3204e-139">Строка</span><span class="sxs-lookup"><span data-stu-id="3204e-139">String</span></span>|<span data-ttu-id="3204e-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3204e-140">Key of the entity.</span></span> <span data-ttu-id="3204e-141">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3204e-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="3204e-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3204e-142">lastModifiedDateTime</span></span>|<span data-ttu-id="3204e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3204e-143">DateTimeOffset</span></span>|<span data-ttu-id="3204e-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3204e-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="3204e-145">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3204e-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="3204e-146">дефаултитем</span><span class="sxs-lookup"><span data-stu-id="3204e-146">defaultItem</span></span>|[<span data-ttu-id="3204e-147">граупполиципресентатиондропдовнлиститем</span><span class="sxs-lookup"><span data-stu-id="3204e-147">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="3204e-148">Локализованное строковое значение, определяющее вариант списка элементов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3204e-148">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="3204e-149">элементы</span><span class="sxs-lookup"><span data-stu-id="3204e-149">items</span></span>|<span data-ttu-id="3204e-150">Коллекция [граупполиципресентатиондропдовнлиститем](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)</span><span class="sxs-lookup"><span data-stu-id="3204e-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="3204e-151">Представляет набор локализованных отображаемых имен и связанных с ними значений.</span><span class="sxs-lookup"><span data-stu-id="3204e-151">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="3204e-152">Обязательный</span><span class="sxs-lookup"><span data-stu-id="3204e-152">required</span></span>|<span data-ttu-id="3204e-153">Логический</span><span class="sxs-lookup"><span data-stu-id="3204e-153">Boolean</span></span>|<span data-ttu-id="3204e-154">Требование ввести значение в поле параметр.</span><span class="sxs-lookup"><span data-stu-id="3204e-154">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="3204e-155">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="3204e-155">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="3204e-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="3204e-156">Response</span></span>
<span data-ttu-id="3204e-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3204e-157">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3204e-158">Пример</span><span class="sxs-lookup"><span data-stu-id="3204e-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="3204e-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="3204e-159">Request</span></span>
<span data-ttu-id="3204e-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3204e-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
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

### <a name="response"></a><span data-ttu-id="3204e-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="3204e-161">Response</span></span>
<span data-ttu-id="3204e-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3204e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





