---
title: Обновление Граупполиципресентатиондропдовнлист
description: Обновление свойств объекта Граупполиципресентатиондропдовнлист.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e5cef0d04dd6c14cadb282e22176250298e21f2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964726"
---
# <a name="update-grouppolicypresentationdropdownlist"></a><span data-ttu-id="ae19d-103">Обновление Граупполиципресентатиондропдовнлист</span><span class="sxs-lookup"><span data-stu-id="ae19d-103">Update groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="ae19d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae19d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae19d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae19d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae19d-106">Обновление свойств объекта [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .</span><span class="sxs-lookup"><span data-stu-id="ae19d-106">Update the properties of a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae19d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ae19d-107">Prerequisites</span></span>
<span data-ttu-id="ae19d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae19d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae19d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae19d-110">Permission type</span></span>|<span data-ttu-id="ae19d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae19d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae19d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae19d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae19d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae19d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ae19d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae19d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae19d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae19d-115">Not supported.</span></span>|
|<span data-ttu-id="ae19d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae19d-116">Application</span></span>|<span data-ttu-id="ae19d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae19d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae19d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae19d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="ae19d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae19d-119">Request headers</span></span>
|<span data-ttu-id="ae19d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae19d-120">Header</span></span>|<span data-ttu-id="ae19d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ae19d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae19d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae19d-122">Authorization</span></span>|<span data-ttu-id="ae19d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae19d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae19d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ae19d-124">Accept</span></span>|<span data-ttu-id="ae19d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae19d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae19d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ae19d-126">Request body</span></span>
<span data-ttu-id="ae19d-127">В тексте запроса добавьте представление объекта [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae19d-127">In the request body, supply a JSON representation for the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

<span data-ttu-id="ae19d-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span><span class="sxs-lookup"><span data-stu-id="ae19d-128">The following table shows the properties that are required when you create the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span></span>

|<span data-ttu-id="ae19d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae19d-129">Property</span></span>|<span data-ttu-id="ae19d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ae19d-130">Type</span></span>|<span data-ttu-id="ae19d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ae19d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae19d-132">label</span><span class="sxs-lookup"><span data-stu-id="ae19d-132">label</span></span>|<span data-ttu-id="ae19d-133">String</span><span class="sxs-lookup"><span data-stu-id="ae19d-133">String</span></span>|<span data-ttu-id="ae19d-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="ae19d-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="ae19d-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="ae19d-135">The default value is empty.</span></span> <span data-ttu-id="ae19d-136">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ae19d-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ae19d-137">id</span><span class="sxs-lookup"><span data-stu-id="ae19d-137">id</span></span>|<span data-ttu-id="ae19d-138">String</span><span class="sxs-lookup"><span data-stu-id="ae19d-138">String</span></span>|<span data-ttu-id="ae19d-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ae19d-139">Key of the entity.</span></span> <span data-ttu-id="ae19d-140">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ae19d-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ae19d-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae19d-141">lastModifiedDateTime</span></span>|<span data-ttu-id="ae19d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae19d-142">DateTimeOffset</span></span>|<span data-ttu-id="ae19d-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ae19d-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="ae19d-144">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ae19d-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ae19d-145">Дефаултитем</span><span class="sxs-lookup"><span data-stu-id="ae19d-145">defaultItem</span></span>|[<span data-ttu-id="ae19d-146">Граупполиципресентатиондропдовнлиститем</span><span class="sxs-lookup"><span data-stu-id="ae19d-146">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="ae19d-147">Локализованное строковое значение, определяющее вариант списка элементов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ae19d-147">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="ae19d-148">items</span><span class="sxs-lookup"><span data-stu-id="ae19d-148">items</span></span>|<span data-ttu-id="ae19d-149">Коллекция [граупполиципресентатиондропдовнлиститем](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ae19d-149">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="ae19d-150">Представляет набор локализованных отображаемых имен и связанных с ними значений.</span><span class="sxs-lookup"><span data-stu-id="ae19d-150">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="ae19d-151">Обязательный</span><span class="sxs-lookup"><span data-stu-id="ae19d-151">required</span></span>|<span data-ttu-id="ae19d-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae19d-152">Boolean</span></span>|<span data-ttu-id="ae19d-153">Требование ввести значение в поле параметр.</span><span class="sxs-lookup"><span data-stu-id="ae19d-153">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="ae19d-154">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="ae19d-154">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="ae19d-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae19d-155">Response</span></span>
<span data-ttu-id="ae19d-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ae19d-156">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae19d-157">Пример</span><span class="sxs-lookup"><span data-stu-id="ae19d-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae19d-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae19d-158">Request</span></span>
<span data-ttu-id="ae19d-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae19d-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ae19d-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae19d-160">Response</span></span>
<span data-ttu-id="ae19d-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae19d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





