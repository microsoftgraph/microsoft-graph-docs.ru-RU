---
title: Обновление Граупполиципресентатиондропдовнлист
description: Обновление свойств объекта Граупполиципресентатиондропдовнлист.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bee92900d50e5813e12568ce9fd717b01deed590
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783019"
---
# <a name="update-grouppolicypresentationdropdownlist"></a><span data-ttu-id="cd332-103">Обновление Граупполиципресентатиондропдовнлист</span><span class="sxs-lookup"><span data-stu-id="cd332-103">Update groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="cd332-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd332-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd332-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd332-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd332-106">Обновление свойств объекта [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .</span><span class="sxs-lookup"><span data-stu-id="cd332-106">Update the properties of a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd332-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cd332-107">Prerequisites</span></span>
<span data-ttu-id="cd332-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd332-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd332-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd332-110">Permission type</span></span>|<span data-ttu-id="cd332-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd332-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd332-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd332-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd332-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd332-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cd332-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd332-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd332-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd332-115">Not supported.</span></span>|
|<span data-ttu-id="cd332-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd332-116">Application</span></span>|<span data-ttu-id="cd332-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd332-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd332-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd332-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="cd332-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd332-119">Request headers</span></span>
|<span data-ttu-id="cd332-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd332-120">Header</span></span>|<span data-ttu-id="cd332-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cd332-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd332-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd332-122">Authorization</span></span>|<span data-ttu-id="cd332-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd332-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd332-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cd332-124">Accept</span></span>|<span data-ttu-id="cd332-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd332-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd332-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd332-126">Request body</span></span>
<span data-ttu-id="cd332-127">В тексте запроса добавьте представление объекта [Граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd332-127">In the request body, supply a JSON representation for the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

<span data-ttu-id="cd332-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span><span class="sxs-lookup"><span data-stu-id="cd332-128">The following table shows the properties that are required when you create the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span></span>

|<span data-ttu-id="cd332-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd332-129">Property</span></span>|<span data-ttu-id="cd332-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cd332-130">Type</span></span>|<span data-ttu-id="cd332-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cd332-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd332-132">label</span><span class="sxs-lookup"><span data-stu-id="cd332-132">label</span></span>|<span data-ttu-id="cd332-133">String</span><span class="sxs-lookup"><span data-stu-id="cd332-133">String</span></span>|<span data-ttu-id="cd332-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="cd332-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="cd332-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="cd332-135">The default value is empty.</span></span> <span data-ttu-id="cd332-136">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="cd332-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cd332-137">id</span><span class="sxs-lookup"><span data-stu-id="cd332-137">id</span></span>|<span data-ttu-id="cd332-138">String</span><span class="sxs-lookup"><span data-stu-id="cd332-138">String</span></span>|<span data-ttu-id="cd332-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cd332-139">Key of the entity.</span></span> <span data-ttu-id="cd332-140">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="cd332-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cd332-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd332-141">lastModifiedDateTime</span></span>|<span data-ttu-id="cd332-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd332-142">DateTimeOffset</span></span>|<span data-ttu-id="cd332-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cd332-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="cd332-144">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="cd332-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cd332-145">Дефаултитем</span><span class="sxs-lookup"><span data-stu-id="cd332-145">defaultItem</span></span>|[<span data-ttu-id="cd332-146">Граупполиципресентатиондропдовнлиститем</span><span class="sxs-lookup"><span data-stu-id="cd332-146">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="cd332-147">Локализованное строковое значение, определяющее вариант списка элементов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="cd332-147">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="cd332-148">items</span><span class="sxs-lookup"><span data-stu-id="cd332-148">items</span></span>|<span data-ttu-id="cd332-149">Коллекция [граупполиципресентатиондропдовнлиститем](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)</span><span class="sxs-lookup"><span data-stu-id="cd332-149">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="cd332-150">Представляет набор локализованных отображаемых имен и связанных с ними значений.</span><span class="sxs-lookup"><span data-stu-id="cd332-150">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="cd332-151">Обязательный</span><span class="sxs-lookup"><span data-stu-id="cd332-151">required</span></span>|<span data-ttu-id="cd332-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd332-152">Boolean</span></span>|<span data-ttu-id="cd332-153">Требование ввести значение в поле параметр.</span><span class="sxs-lookup"><span data-stu-id="cd332-153">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="cd332-154">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="cd332-154">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="cd332-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd332-155">Response</span></span>
<span data-ttu-id="cd332-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cd332-156">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd332-157">Пример</span><span class="sxs-lookup"><span data-stu-id="cd332-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd332-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd332-158">Request</span></span>
<span data-ttu-id="cd332-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd332-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cd332-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd332-160">Response</span></span>
<span data-ttu-id="cd332-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd332-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





