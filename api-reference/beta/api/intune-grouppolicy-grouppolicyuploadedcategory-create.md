---
title: Создание groupPolicyUploadedCategory
description: Создайте новый объект GroupPolicyUploadedCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7996f9e28deeefd2dcac04d3496dc67a216708e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157089"
---
# <a name="create-grouppolicyuploadedcategory"></a><span data-ttu-id="040fb-103">Создание groupPolicyUploadedCategory</span><span class="sxs-lookup"><span data-stu-id="040fb-103">Create groupPolicyUploadedCategory</span></span>

<span data-ttu-id="040fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="040fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="040fb-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="040fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="040fb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="040fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="040fb-107">Создайте новый [объект GroupPolicyUploadedCategory.](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)</span><span class="sxs-lookup"><span data-stu-id="040fb-107">Create a new [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="040fb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="040fb-108">Prerequisites</span></span>
<span data-ttu-id="040fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="040fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="040fb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="040fb-111">Permission type</span></span>|<span data-ttu-id="040fb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="040fb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="040fb-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="040fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="040fb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="040fb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="040fb-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="040fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="040fb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="040fb-116">Not supported.</span></span>|
|<span data-ttu-id="040fb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="040fb-117">Application</span></span>|<span data-ttu-id="040fb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="040fb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="040fb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="040fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyCategories
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/children
```

## <a name="request-headers"></a><span data-ttu-id="040fb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="040fb-120">Request headers</span></span>
|<span data-ttu-id="040fb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="040fb-121">Header</span></span>|<span data-ttu-id="040fb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="040fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="040fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="040fb-123">Authorization</span></span>|<span data-ttu-id="040fb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="040fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="040fb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="040fb-125">Accept</span></span>|<span data-ttu-id="040fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="040fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="040fb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="040fb-127">Request body</span></span>
<span data-ttu-id="040fb-128">В теле запроса поставляем представление JSON для объекта groupPolicyUploadedCategory.</span><span class="sxs-lookup"><span data-stu-id="040fb-128">In the request body, supply a JSON representation for the groupPolicyUploadedCategory object.</span></span>

<span data-ttu-id="040fb-129">В следующей таблице показаны свойства, необходимые при создании groupPolicyUploadedCategory.</span><span class="sxs-lookup"><span data-stu-id="040fb-129">The following table shows the properties that are required when you create the groupPolicyUploadedCategory.</span></span>

|<span data-ttu-id="040fb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="040fb-130">Property</span></span>|<span data-ttu-id="040fb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="040fb-131">Type</span></span>|<span data-ttu-id="040fb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="040fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="040fb-133">displayName</span><span class="sxs-lookup"><span data-stu-id="040fb-133">displayName</span></span>|<span data-ttu-id="040fb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="040fb-134">String</span></span>|<span data-ttu-id="040fb-135">Строковой id имени отображения категории, унаследованной от [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="040fb-135">The string id of the category's display name Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="040fb-136">isRoot</span><span class="sxs-lookup"><span data-stu-id="040fb-136">isRoot</span></span>|<span data-ttu-id="040fb-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="040fb-137">Boolean</span></span>|<span data-ttu-id="040fb-138">Определяет, является ли категория корневой категорией, унаследованной от [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="040fb-138">Defines if the category is a root category Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="040fb-139">id</span><span class="sxs-lookup"><span data-stu-id="040fb-139">id</span></span>|<span data-ttu-id="040fb-140">Строка</span><span class="sxs-lookup"><span data-stu-id="040fb-140">String</span></span>|<span data-ttu-id="040fb-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="040fb-141">Key of the entity.</span></span> <span data-ttu-id="040fb-142">Унаследованный от [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="040fb-142">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="040fb-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="040fb-143">lastModifiedDateTime</span></span>|<span data-ttu-id="040fb-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="040fb-144">DateTimeOffset</span></span>|<span data-ttu-id="040fb-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="040fb-145">The date and time the entity was last modified.</span></span> <span data-ttu-id="040fb-146">Унаследованный от [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="040fb-146">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="040fb-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="040fb-147">Response</span></span>
<span data-ttu-id="040fb-148">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="040fb-148">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="040fb-149">Пример</span><span class="sxs-lookup"><span data-stu-id="040fb-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="040fb-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="040fb-150">Request</span></span>
<span data-ttu-id="040fb-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="040fb-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories
Content-type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedCategory",
  "displayName": "Display Name value",
  "isRoot": true
}
```

### <a name="response"></a><span data-ttu-id="040fb-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="040fb-152">Response</span></span>
<span data-ttu-id="040fb-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="040fb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




