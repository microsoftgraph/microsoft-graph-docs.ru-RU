---
title: Обновление groupPolicyPresentationDropdownList
description: Обновление свойств объекта groupPolicyPresentationDropdownList.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 42bbf30c40f8597804817a35ed32eb3859868e36
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135420"
---
# <a name="update-grouppolicypresentationdropdownlist"></a><span data-ttu-id="8509c-103">Обновление groupPolicyPresentationDropdownList</span><span class="sxs-lookup"><span data-stu-id="8509c-103">Update groupPolicyPresentationDropdownList</span></span>

<span data-ttu-id="8509c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8509c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8509c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8509c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8509c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8509c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8509c-107">Обновление свойств объекта [groupPolicyPresentationDropdownList.](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)</span><span class="sxs-lookup"><span data-stu-id="8509c-107">Update the properties of a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8509c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8509c-108">Prerequisites</span></span>
<span data-ttu-id="8509c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8509c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8509c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8509c-111">Permission type</span></span>|<span data-ttu-id="8509c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8509c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8509c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8509c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8509c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8509c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8509c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8509c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8509c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8509c-116">Not supported.</span></span>|
|<span data-ttu-id="8509c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8509c-117">Application</span></span>|<span data-ttu-id="8509c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8509c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8509c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8509c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="8509c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8509c-120">Request headers</span></span>
|<span data-ttu-id="8509c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8509c-121">Header</span></span>|<span data-ttu-id="8509c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8509c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8509c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8509c-123">Authorization</span></span>|<span data-ttu-id="8509c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8509c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8509c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8509c-125">Accept</span></span>|<span data-ttu-id="8509c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8509c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8509c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8509c-127">Request body</span></span>
<span data-ttu-id="8509c-128">В теле запроса поставляем представление JSON для [объекта GroupPolicyPresentationDropdownList.](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)</span><span class="sxs-lookup"><span data-stu-id="8509c-128">In the request body, supply a JSON representation for the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

<span data-ttu-id="8509c-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyPresentationDropdownList.](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)</span><span class="sxs-lookup"><span data-stu-id="8509c-129">The following table shows the properties that are required when you create the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span></span>

|<span data-ttu-id="8509c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8509c-130">Property</span></span>|<span data-ttu-id="8509c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8509c-131">Type</span></span>|<span data-ttu-id="8509c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8509c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8509c-133">label</span><span class="sxs-lookup"><span data-stu-id="8509c-133">label</span></span>|<span data-ttu-id="8509c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8509c-134">String</span></span>|<span data-ttu-id="8509c-135">Локализованная текстовая метка для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="8509c-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="8509c-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="8509c-136">The default value is empty.</span></span> <span data-ttu-id="8509c-137">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8509c-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8509c-138">id</span><span class="sxs-lookup"><span data-stu-id="8509c-138">id</span></span>|<span data-ttu-id="8509c-139">Строка</span><span class="sxs-lookup"><span data-stu-id="8509c-139">String</span></span>|<span data-ttu-id="8509c-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8509c-140">Key of the entity.</span></span> <span data-ttu-id="8509c-141">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8509c-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8509c-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8509c-142">lastModifiedDateTime</span></span>|<span data-ttu-id="8509c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8509c-143">DateTimeOffset</span></span>|<span data-ttu-id="8509c-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8509c-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="8509c-145">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8509c-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8509c-146">defaultItem</span><span class="sxs-lookup"><span data-stu-id="8509c-146">defaultItem</span></span>|[<span data-ttu-id="8509c-147">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="8509c-147">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="8509c-148">Локализованное значение строки, определяющие выбор списка элементов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8509c-148">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="8509c-149">items</span><span class="sxs-lookup"><span data-stu-id="8509c-149">items</span></span>|<span data-ttu-id="8509c-150">[коллекция groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)</span><span class="sxs-lookup"><span data-stu-id="8509c-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="8509c-151">Представляет набор локализованных имен отображения и связанных с ними значений.</span><span class="sxs-lookup"><span data-stu-id="8509c-151">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="8509c-152">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8509c-152">required</span></span>|<span data-ttu-id="8509c-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="8509c-153">Boolean</span></span>|<span data-ttu-id="8509c-154">Требование ввести значение в поле параметра.</span><span class="sxs-lookup"><span data-stu-id="8509c-154">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="8509c-155">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="8509c-155">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="8509c-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="8509c-156">Response</span></span>
<span data-ttu-id="8509c-157">В случае успешного завершения этот метод возвращает код ответа и обновленный объект `200 OK` [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8509c-157">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8509c-158">Пример</span><span class="sxs-lookup"><span data-stu-id="8509c-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="8509c-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="8509c-159">Request</span></span>
<span data-ttu-id="8509c-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8509c-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8509c-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="8509c-161">Response</span></span>
<span data-ttu-id="8509c-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8509c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




