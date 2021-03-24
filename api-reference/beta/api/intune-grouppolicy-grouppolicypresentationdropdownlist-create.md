---
title: Создание groupPolicyPresentationDropdownList
description: Создайте новый объект GroupPolicyPresentationDropdownList.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ecc4d8d45f223e225c00ab027c1326b46f5cb869
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149634"
---
# <a name="create-grouppolicypresentationdropdownlist"></a><span data-ttu-id="b9f1a-103">Создание groupPolicyPresentationDropdownList</span><span class="sxs-lookup"><span data-stu-id="b9f1a-103">Create groupPolicyPresentationDropdownList</span></span>

<span data-ttu-id="b9f1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9f1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9f1a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9f1a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9f1a-107">Создайте новый [объект GroupPolicyPresentationDropdownList.](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)</span><span class="sxs-lookup"><span data-stu-id="b9f1a-107">Create a new [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9f1a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b9f1a-108">Prerequisites</span></span>
<span data-ttu-id="b9f1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9f1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9f1a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9f1a-111">Permission type</span></span>|<span data-ttu-id="b9f1a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9f1a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9f1a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9f1a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9f1a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9f1a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9f1a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9f1a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9f1a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-116">Not supported.</span></span>|
|<span data-ttu-id="b9f1a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b9f1a-117">Application</span></span>|<span data-ttu-id="b9f1a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9f1a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9f1a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9f1a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="b9f1a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b9f1a-120">Request headers</span></span>
|<span data-ttu-id="b9f1a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b9f1a-121">Header</span></span>|<span data-ttu-id="b9f1a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b9f1a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9f1a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9f1a-123">Authorization</span></span>|<span data-ttu-id="b9f1a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9f1a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b9f1a-125">Accept</span></span>|<span data-ttu-id="b9f1a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9f1a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9f1a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9f1a-127">Request body</span></span>
<span data-ttu-id="b9f1a-128">В теле запроса поставляем представление JSON для объекта GroupPolicyPresentationDropdownList.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-128">In the request body, supply a JSON representation for the groupPolicyPresentationDropdownList object.</span></span>

<span data-ttu-id="b9f1a-129">В следующей таблице показаны свойства, необходимые при создании groupPolicyPresentationDropdownList.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-129">The following table shows the properties that are required when you create the groupPolicyPresentationDropdownList.</span></span>

|<span data-ttu-id="b9f1a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9f1a-130">Property</span></span>|<span data-ttu-id="b9f1a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b9f1a-131">Type</span></span>|<span data-ttu-id="b9f1a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b9f1a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9f1a-133">label</span><span class="sxs-lookup"><span data-stu-id="b9f1a-133">label</span></span>|<span data-ttu-id="b9f1a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b9f1a-134">String</span></span>|<span data-ttu-id="b9f1a-135">Локализованная текстовая метка для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="b9f1a-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-136">The default value is empty.</span></span> <span data-ttu-id="b9f1a-137">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b9f1a-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b9f1a-138">id</span><span class="sxs-lookup"><span data-stu-id="b9f1a-138">id</span></span>|<span data-ttu-id="b9f1a-139">Строка</span><span class="sxs-lookup"><span data-stu-id="b9f1a-139">String</span></span>|<span data-ttu-id="b9f1a-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-140">Key of the entity.</span></span> <span data-ttu-id="b9f1a-141">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b9f1a-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b9f1a-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9f1a-142">lastModifiedDateTime</span></span>|<span data-ttu-id="b9f1a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9f1a-143">DateTimeOffset</span></span>|<span data-ttu-id="b9f1a-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="b9f1a-145">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b9f1a-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="b9f1a-146">defaultItem</span><span class="sxs-lookup"><span data-stu-id="b9f1a-146">defaultItem</span></span>|[<span data-ttu-id="b9f1a-147">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="b9f1a-147">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="b9f1a-148">Локализованное значение строки, определяющие выбор списка элементов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-148">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="b9f1a-149">items</span><span class="sxs-lookup"><span data-stu-id="b9f1a-149">items</span></span>|<span data-ttu-id="b9f1a-150">[коллекция groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b9f1a-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="b9f1a-151">Представляет набор локализованных имен отображения и связанных с ними значений.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-151">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="b9f1a-152">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b9f1a-152">required</span></span>|<span data-ttu-id="b9f1a-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9f1a-153">Boolean</span></span>|<span data-ttu-id="b9f1a-154">Требование ввести значение в поле параметра.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-154">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="b9f1a-155">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-155">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="b9f1a-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9f1a-156">Response</span></span>
<span data-ttu-id="b9f1a-157">В случае успешного завершения этот метод возвращает код ответа и `201 Created` [объект GroupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-157">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9f1a-158">Пример</span><span class="sxs-lookup"><span data-stu-id="b9f1a-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9f1a-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9f1a-159">Request</span></span>
<span data-ttu-id="b9f1a-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b9f1a-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9f1a-161">Response</span></span>
<span data-ttu-id="b9f1a-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9f1a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




