---
title: Обновление Граупполициуплоадедкатегори
description: Обновление свойств объекта Граупполициуплоадедкатегори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 03d6bdffff214ad7e095475adbd116644029a5bd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735409"
---
# <a name="update-grouppolicyuploadedcategory"></a><span data-ttu-id="197a1-103">Обновление Граупполициуплоадедкатегори</span><span class="sxs-lookup"><span data-stu-id="197a1-103">Update groupPolicyUploadedCategory</span></span>

<span data-ttu-id="197a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="197a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="197a1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="197a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="197a1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="197a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="197a1-107">Обновление свойств объекта [граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="197a1-107">Update the properties of a [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="197a1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="197a1-108">Prerequisites</span></span>
<span data-ttu-id="197a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="197a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="197a1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="197a1-111">Permission type</span></span>|<span data-ttu-id="197a1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="197a1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="197a1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="197a1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="197a1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="197a1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="197a1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="197a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="197a1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="197a1-116">Not supported.</span></span>|
|<span data-ttu-id="197a1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="197a1-117">Application</span></span>|<span data-ttu-id="197a1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="197a1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="197a1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="197a1-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="197a1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="197a1-120">Request headers</span></span>
|<span data-ttu-id="197a1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="197a1-121">Header</span></span>|<span data-ttu-id="197a1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="197a1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="197a1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="197a1-123">Authorization</span></span>|<span data-ttu-id="197a1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="197a1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="197a1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="197a1-125">Accept</span></span>|<span data-ttu-id="197a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="197a1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="197a1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="197a1-127">Request body</span></span>
<span data-ttu-id="197a1-128">В тексте запроса добавьте представление объекта [граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="197a1-128">In the request body, supply a JSON representation for the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

<span data-ttu-id="197a1-129">В следующей таблице приведены свойства, необходимые при создании [граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).</span><span class="sxs-lookup"><span data-stu-id="197a1-129">The following table shows the properties that are required when you create the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).</span></span>

|<span data-ttu-id="197a1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="197a1-130">Property</span></span>|<span data-ttu-id="197a1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="197a1-131">Type</span></span>|<span data-ttu-id="197a1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="197a1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="197a1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="197a1-133">displayName</span></span>|<span data-ttu-id="197a1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="197a1-134">String</span></span>|<span data-ttu-id="197a1-135">Идентификатор строки отображаемого имени категории, унаследованной от [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="197a1-135">The string id of the category's display name Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="197a1-136">Корень</span><span class="sxs-lookup"><span data-stu-id="197a1-136">isRoot</span></span>|<span data-ttu-id="197a1-137">Логический</span><span class="sxs-lookup"><span data-stu-id="197a1-137">Boolean</span></span>|<span data-ttu-id="197a1-138">Определяет, является ли категория корневой категорией, унаследованной от [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="197a1-138">Defines if the category is a root category Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="197a1-139">id</span><span class="sxs-lookup"><span data-stu-id="197a1-139">id</span></span>|<span data-ttu-id="197a1-140">Строка</span><span class="sxs-lookup"><span data-stu-id="197a1-140">String</span></span>|<span data-ttu-id="197a1-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="197a1-141">Key of the entity.</span></span> <span data-ttu-id="197a1-142">Наследуется от [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="197a1-142">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="197a1-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="197a1-143">lastModifiedDateTime</span></span>|<span data-ttu-id="197a1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="197a1-144">DateTimeOffset</span></span>|<span data-ttu-id="197a1-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="197a1-145">The date and time the entity was last modified.</span></span> <span data-ttu-id="197a1-146">Наследуется от [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="197a1-146">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="197a1-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="197a1-147">Response</span></span>
<span data-ttu-id="197a1-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициуплоадедкатегори](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="197a1-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="197a1-149">Пример</span><span class="sxs-lookup"><span data-stu-id="197a1-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="197a1-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="197a1-150">Request</span></span>
<span data-ttu-id="197a1-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="197a1-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="197a1-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="197a1-152">Response</span></span>
<span data-ttu-id="197a1-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="197a1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





