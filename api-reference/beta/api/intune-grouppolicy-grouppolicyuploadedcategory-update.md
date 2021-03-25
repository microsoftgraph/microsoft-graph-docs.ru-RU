---
title: Update groupPolicyUploadedCategory
description: Обновление свойств объекта groupPolicyUploadedCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 907df2881555cf651442bffd29c2cd98b0e25d0e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157019"
---
# <a name="update-grouppolicyuploadedcategory"></a><span data-ttu-id="bcc30-103">Update groupPolicyUploadedCategory</span><span class="sxs-lookup"><span data-stu-id="bcc30-103">Update groupPolicyUploadedCategory</span></span>

<span data-ttu-id="bcc30-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcc30-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bcc30-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcc30-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcc30-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bcc30-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcc30-107">Обновление свойств объекта [groupPolicyUploadedCategory.](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)</span><span class="sxs-lookup"><span data-stu-id="bcc30-107">Update the properties of a [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcc30-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bcc30-108">Prerequisites</span></span>
<span data-ttu-id="bcc30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcc30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcc30-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcc30-111">Permission type</span></span>|<span data-ttu-id="bcc30-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcc30-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcc30-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcc30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bcc30-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcc30-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bcc30-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcc30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcc30-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcc30-116">Not supported.</span></span>|
|<span data-ttu-id="bcc30-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bcc30-117">Application</span></span>|<span data-ttu-id="bcc30-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcc30-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcc30-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcc30-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="bcc30-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bcc30-120">Request headers</span></span>
|<span data-ttu-id="bcc30-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bcc30-121">Header</span></span>|<span data-ttu-id="bcc30-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bcc30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcc30-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcc30-123">Authorization</span></span>|<span data-ttu-id="bcc30-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcc30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcc30-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bcc30-125">Accept</span></span>|<span data-ttu-id="bcc30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bcc30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcc30-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcc30-127">Request body</span></span>
<span data-ttu-id="bcc30-128">В теле запроса поставляем представление JSON для [объекта groupPolicyUploadedCategory.](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)</span><span class="sxs-lookup"><span data-stu-id="bcc30-128">In the request body, supply a JSON representation for the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object.</span></span>

<span data-ttu-id="bcc30-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyUploadedCategory.](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)</span><span class="sxs-lookup"><span data-stu-id="bcc30-129">The following table shows the properties that are required when you create the [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).</span></span>

|<span data-ttu-id="bcc30-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bcc30-130">Property</span></span>|<span data-ttu-id="bcc30-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bcc30-131">Type</span></span>|<span data-ttu-id="bcc30-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bcc30-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcc30-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bcc30-133">displayName</span></span>|<span data-ttu-id="bcc30-134">Строка</span><span class="sxs-lookup"><span data-stu-id="bcc30-134">String</span></span>|<span data-ttu-id="bcc30-135">Строковой id имени отображения категории, унаследованной от [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="bcc30-135">The string id of the category's display name Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="bcc30-136">isRoot</span><span class="sxs-lookup"><span data-stu-id="bcc30-136">isRoot</span></span>|<span data-ttu-id="bcc30-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="bcc30-137">Boolean</span></span>|<span data-ttu-id="bcc30-138">Определяет, является ли категория корневой категорией, унаследованной от [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="bcc30-138">Defines if the category is a root category Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="bcc30-139">id</span><span class="sxs-lookup"><span data-stu-id="bcc30-139">id</span></span>|<span data-ttu-id="bcc30-140">Строка</span><span class="sxs-lookup"><span data-stu-id="bcc30-140">String</span></span>|<span data-ttu-id="bcc30-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bcc30-141">Key of the entity.</span></span> <span data-ttu-id="bcc30-142">Унаследованный от [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="bcc30-142">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|
|<span data-ttu-id="bcc30-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bcc30-143">lastModifiedDateTime</span></span>|<span data-ttu-id="bcc30-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcc30-144">DateTimeOffset</span></span>|<span data-ttu-id="bcc30-145">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bcc30-145">The date and time the entity was last modified.</span></span> <span data-ttu-id="bcc30-146">Унаследованный от [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="bcc30-146">Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="bcc30-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcc30-147">Response</span></span>
<span data-ttu-id="bcc30-148">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bcc30-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcc30-149">Пример</span><span class="sxs-lookup"><span data-stu-id="bcc30-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcc30-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcc30-150">Request</span></span>
<span data-ttu-id="bcc30-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcc30-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bcc30-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcc30-152">Response</span></span>
<span data-ttu-id="bcc30-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bcc30-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




