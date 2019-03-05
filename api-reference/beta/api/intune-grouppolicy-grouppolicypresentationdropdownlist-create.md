---
title: Создание Граупполиципресентатиондропдовнлист
description: Создание нового объекта Граупполиципресентатиондропдовнлист.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12ec4cba923fd493441731e205c2e0a7facf87b0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152012"
---
# <a name="create-grouppolicypresentationdropdownlist"></a><span data-ttu-id="6d4ad-103">Создание Граупполиципресентатиондропдовнлист</span><span class="sxs-lookup"><span data-stu-id="6d4ad-103">Create groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="6d4ad-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d4ad-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d4ad-106">Создание нового объекта [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .</span><span class="sxs-lookup"><span data-stu-id="6d4ad-106">Create a new [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d4ad-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6d4ad-107">Prerequisites</span></span>
<span data-ttu-id="6d4ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6d4ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6d4ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d4ad-110">Permission type</span></span>|<span data-ttu-id="6d4ad-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d4ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d4ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d4ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6d4ad-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d4ad-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6d4ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d4ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d4ad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-115">Not supported.</span></span>|
|<span data-ttu-id="6d4ad-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d4ad-116">Application</span></span>|<span data-ttu-id="6d4ad-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d4ad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d4ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="6d4ad-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d4ad-119">Request headers</span></span>
|<span data-ttu-id="6d4ad-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d4ad-120">Header</span></span>|<span data-ttu-id="6d4ad-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6d4ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d4ad-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d4ad-122">Authorization</span></span>|<span data-ttu-id="6d4ad-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6d4ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d4ad-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6d4ad-124">Accept</span></span>|<span data-ttu-id="6d4ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6d4ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d4ad-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d4ad-126">Request body</span></span>
<span data-ttu-id="6d4ad-127">В тексте запроса добавьте представление объекта Граупполиципресентатиондропдовнлист в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-127">In the request body, supply a JSON representation for the groupPolicyPresentationDropdownList object.</span></span>

<span data-ttu-id="6d4ad-128">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатиондропдовнлист.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-128">The following table shows the properties that are required when you create the groupPolicyPresentationDropdownList.</span></span>

|<span data-ttu-id="6d4ad-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d4ad-129">Property</span></span>|<span data-ttu-id="6d4ad-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6d4ad-130">Type</span></span>|<span data-ttu-id="6d4ad-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6d4ad-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d4ad-132">label</span><span class="sxs-lookup"><span data-stu-id="6d4ad-132">label</span></span>|<span data-ttu-id="6d4ad-133">String</span><span class="sxs-lookup"><span data-stu-id="6d4ad-133">String</span></span>|<span data-ttu-id="6d4ad-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="6d4ad-135">Значение по умолчанию — пустое значение.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-135">The default value is empty.</span></span> <span data-ttu-id="6d4ad-136">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6d4ad-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6d4ad-137">id</span><span class="sxs-lookup"><span data-stu-id="6d4ad-137">id</span></span>|<span data-ttu-id="6d4ad-138">String</span><span class="sxs-lookup"><span data-stu-id="6d4ad-138">String</span></span>|<span data-ttu-id="6d4ad-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-139">Key of the entity.</span></span> <span data-ttu-id="6d4ad-140">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6d4ad-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6d4ad-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d4ad-141">lastModifiedDateTime</span></span>|<span data-ttu-id="6d4ad-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d4ad-142">DateTimeOffset</span></span>|<span data-ttu-id="6d4ad-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="6d4ad-144">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="6d4ad-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6d4ad-145">Дефаултитем</span><span class="sxs-lookup"><span data-stu-id="6d4ad-145">defaultItem</span></span>|[<span data-ttu-id="6d4ad-146">Граупполиципресентатиондропдовнлиститем</span><span class="sxs-lookup"><span data-stu-id="6d4ad-146">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="6d4ad-147">Локализованное строковое значение, определяющее вариант списка элементов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-147">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="6d4ad-148">items</span><span class="sxs-lookup"><span data-stu-id="6d4ad-148">items</span></span>|<span data-ttu-id="6d4ad-149">Коллекция [граупполиципресентатиондропдовнлиститем](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6d4ad-149">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="6d4ad-150">Представляет набор локализованных отображаемых имен и связанных с ними значений.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-150">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="6d4ad-151">Обязательный</span><span class="sxs-lookup"><span data-stu-id="6d4ad-151">required</span></span>|<span data-ttu-id="6d4ad-152">Логический</span><span class="sxs-lookup"><span data-stu-id="6d4ad-152">Boolean</span></span>|<span data-ttu-id="6d4ad-153">Требование ввести значение в поле параметр.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-153">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="6d4ad-154">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-154">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="6d4ad-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d4ad-155">Response</span></span>
<span data-ttu-id="6d4ad-156">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатиондропдовнлист](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-156">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d4ad-157">Пример</span><span class="sxs-lookup"><span data-stu-id="6d4ad-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d4ad-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d4ad-158">Request</span></span>
<span data-ttu-id="6d4ad-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6d4ad-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d4ad-160">Response</span></span>
<span data-ttu-id="6d4ad-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d4ad-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




