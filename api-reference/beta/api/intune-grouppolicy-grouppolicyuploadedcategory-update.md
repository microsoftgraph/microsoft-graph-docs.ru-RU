---
title: Обновление Граупполициуплоадедкатегори
description: Обновление свойств объекта Граупполициуплоадедкатегори.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 148c698c6bbc466fc4aef10bb62b09f61386f362
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803773"
---
# <a name="update-grouppolicyuploadedcategory"></a><span data-ttu-id="20461-103">Обновление Граупполициуплоадедкатегори</span><span class="sxs-lookup"><span data-stu-id="20461-103">Update groupPolicyUploadedCategory</span></span>

> <span data-ttu-id="20461-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20461-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20461-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20461-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20461-106">Обновление свойств объекта [граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="20461-106">Update the properties of a [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20461-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="20461-107">Prerequisites</span></span>
<span data-ttu-id="20461-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20461-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20461-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20461-110">Permission type</span></span>|<span data-ttu-id="20461-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20461-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20461-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20461-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20461-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20461-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="20461-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20461-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20461-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20461-115">Not supported.</span></span>|
|<span data-ttu-id="20461-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="20461-116">Application</span></span>|<span data-ttu-id="20461-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20461-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20461-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20461-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/parent
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/children/{groupPolicyCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="20461-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="20461-119">Request headers</span></span>
|<span data-ttu-id="20461-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20461-120">Header</span></span>|<span data-ttu-id="20461-121">Значение</span><span class="sxs-lookup"><span data-stu-id="20461-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20461-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="20461-122">Authorization</span></span>|<span data-ttu-id="20461-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20461-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20461-124">Accept</span><span class="sxs-lookup"><span data-stu-id="20461-124">Accept</span></span>|<span data-ttu-id="20461-125">application/json</span><span class="sxs-lookup"><span data-stu-id="20461-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20461-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20461-126">Request body</span></span>
<span data-ttu-id="20461-127">В тексте запроса добавьте представление объекта [граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20461-127">In the request body, supply a JSON representation for the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

<span data-ttu-id="20461-128">В следующей таблице приведены свойства, необходимые при создании [граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).</span><span class="sxs-lookup"><span data-stu-id="20461-128">The following table shows the properties that are required when you create the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).</span></span>

|<span data-ttu-id="20461-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="20461-129">Property</span></span>|<span data-ttu-id="20461-130">Тип</span><span class="sxs-lookup"><span data-stu-id="20461-130">Type</span></span>|<span data-ttu-id="20461-131">Описание</span><span class="sxs-lookup"><span data-stu-id="20461-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20461-132">displayName</span><span class="sxs-lookup"><span data-stu-id="20461-132">displayName</span></span>|<span data-ttu-id="20461-133">Строка</span><span class="sxs-lookup"><span data-stu-id="20461-133">String</span></span>|<span data-ttu-id="20461-134">Идентификатор строки отображаемого имени категории, унаследованной от [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="20461-134">The string id of the category's display name Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="20461-135">Корень</span><span class="sxs-lookup"><span data-stu-id="20461-135">isRoot</span></span>|<span data-ttu-id="20461-136">Логический</span><span class="sxs-lookup"><span data-stu-id="20461-136">Boolean</span></span>|<span data-ttu-id="20461-137">Определяет, является ли категория корневой категорией, унаследованной от [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="20461-137">Defines if the category is a root category Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="20461-138">id</span><span class="sxs-lookup"><span data-stu-id="20461-138">id</span></span>|<span data-ttu-id="20461-139">String</span><span class="sxs-lookup"><span data-stu-id="20461-139">String</span></span>|<span data-ttu-id="20461-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="20461-140">Key of the entity.</span></span> <span data-ttu-id="20461-141">Наследуется от [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="20461-141">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="20461-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20461-142">lastModifiedDateTime</span></span>|<span data-ttu-id="20461-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20461-143">DateTimeOffset</span></span>|<span data-ttu-id="20461-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="20461-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="20461-145">Наследуется от [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="20461-145">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="20461-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="20461-146">Response</span></span>
<span data-ttu-id="20461-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="20461-147">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20461-148">Пример</span><span class="sxs-lookup"><span data-stu-id="20461-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="20461-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="20461-149">Request</span></span>
<span data-ttu-id="20461-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20461-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}
Content-type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedCategory",
  "displayName": "Display Name value",
  "isRoot": true
}
```

### <a name="response"></a><span data-ttu-id="20461-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="20461-151">Response</span></span>
<span data-ttu-id="20461-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20461-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 241

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedCategory",
  "displayName": "Display Name value",
  "isRoot": true,
  "id": "7e373e80-3e80-7e37-803e-377e803e377e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




