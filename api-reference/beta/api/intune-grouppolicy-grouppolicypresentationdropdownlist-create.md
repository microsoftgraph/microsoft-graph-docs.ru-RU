---
title: Создание groupPolicyPresentationDropdownList
description: Создание нового объекта groupPolicyPresentationDropdownList.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 415ccd634e4206b2849fc5feecc4131d2f417d16
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431741"
---
# <a name="create-grouppolicypresentationdropdownlist"></a><span data-ttu-id="62372-103">Создание groupPolicyPresentationDropdownList</span><span class="sxs-lookup"><span data-stu-id="62372-103">Create groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="62372-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="62372-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="62372-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62372-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62372-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62372-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62372-107">Создание нового объекта [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .</span><span class="sxs-lookup"><span data-stu-id="62372-107">Create a new [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62372-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="62372-108">Prerequisites</span></span>
<span data-ttu-id="62372-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="62372-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="62372-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62372-111">Permission type</span></span>|<span data-ttu-id="62372-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62372-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62372-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62372-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62372-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62372-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="62372-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62372-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62372-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62372-116">Not supported.</span></span>|
|<span data-ttu-id="62372-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62372-117">Application</span></span>|<span data-ttu-id="62372-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62372-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62372-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62372-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="62372-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62372-120">Request headers</span></span>
|<span data-ttu-id="62372-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62372-121">Header</span></span>|<span data-ttu-id="62372-122">Значение</span><span class="sxs-lookup"><span data-stu-id="62372-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62372-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="62372-123">Authorization</span></span>|<span data-ttu-id="62372-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="62372-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62372-125">Accept</span><span class="sxs-lookup"><span data-stu-id="62372-125">Accept</span></span>|<span data-ttu-id="62372-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62372-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62372-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62372-127">Request body</span></span>
<span data-ttu-id="62372-128">В тексте запроса укажите представление JSON для объекта groupPolicyPresentationDropdownList.</span><span class="sxs-lookup"><span data-stu-id="62372-128">In the request body, supply a JSON representation for the groupPolicyPresentationDropdownList object.</span></span>

<span data-ttu-id="62372-129">В следующей таблице показаны свойства, которые необходимы для создания groupPolicyPresentationDropdownList.</span><span class="sxs-lookup"><span data-stu-id="62372-129">The following table shows the properties that are required when you create the groupPolicyPresentationDropdownList.</span></span>

|<span data-ttu-id="62372-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="62372-130">Property</span></span>|<span data-ttu-id="62372-131">Тип</span><span class="sxs-lookup"><span data-stu-id="62372-131">Type</span></span>|<span data-ttu-id="62372-132">Описание</span><span class="sxs-lookup"><span data-stu-id="62372-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62372-133">label</span><span class="sxs-lookup"><span data-stu-id="62372-133">label</span></span>|<span data-ttu-id="62372-134">String</span><span class="sxs-lookup"><span data-stu-id="62372-134">String</span></span>|<span data-ttu-id="62372-135">Метка локализованный текст для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="62372-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="62372-136">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="62372-136">The default value is empty.</span></span> <span data-ttu-id="62372-137">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="62372-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="62372-138">id</span><span class="sxs-lookup"><span data-stu-id="62372-138">id</span></span>|<span data-ttu-id="62372-139">String</span><span class="sxs-lookup"><span data-stu-id="62372-139">String</span></span>|<span data-ttu-id="62372-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="62372-140">Key of the entity.</span></span> <span data-ttu-id="62372-141">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="62372-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="62372-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62372-142">lastModifiedDateTime</span></span>|<span data-ttu-id="62372-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62372-143">DateTimeOffset</span></span>|<span data-ttu-id="62372-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="62372-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="62372-145">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="62372-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="62372-146">defaultItem</span><span class="sxs-lookup"><span data-stu-id="62372-146">defaultItem</span></span>|[<span data-ttu-id="62372-147">groupPolicyPresentationDropdownListItem</span><span class="sxs-lookup"><span data-stu-id="62372-147">groupPolicyPresentationDropdownListItem</span></span>](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|<span data-ttu-id="62372-148">Локализованное строковое значение, указывающее вариант по умолчанию из списка элементов.</span><span class="sxs-lookup"><span data-stu-id="62372-148">Localized string value identifying the default choice of the list of items.</span></span>|
|<span data-ttu-id="62372-149">items</span><span class="sxs-lookup"><span data-stu-id="62372-149">items</span></span>|<span data-ttu-id="62372-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="62372-150">[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) collection</span></span>|<span data-ttu-id="62372-151">Представляет набор локализованные отображаемые имена и связанных с ними значений.</span><span class="sxs-lookup"><span data-stu-id="62372-151">Represents a set of localized display names and their associated values.</span></span>|
|<span data-ttu-id="62372-152">Обязательный</span><span class="sxs-lookup"><span data-stu-id="62372-152">required</span></span>|<span data-ttu-id="62372-153">Логический</span><span class="sxs-lookup"><span data-stu-id="62372-153">Boolean</span></span>|<span data-ttu-id="62372-154">Требование ввести значение в поле параметра.</span><span class="sxs-lookup"><span data-stu-id="62372-154">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="62372-155">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="62372-155">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="62372-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="62372-156">Response</span></span>
<span data-ttu-id="62372-157">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="62372-157">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62372-158">Пример</span><span class="sxs-lookup"><span data-stu-id="62372-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="62372-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="62372-159">Request</span></span>
<span data-ttu-id="62372-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62372-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="62372-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="62372-161">Response</span></span>
<span data-ttu-id="62372-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="62372-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




