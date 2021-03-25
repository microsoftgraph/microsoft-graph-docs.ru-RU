---
title: Update groupPolicyCategory
description: Обновление свойств объекта groupPolicyCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a70edcb1f05ceb19a7dbb7a65d2d4b501a724dc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153484"
---
# <a name="update-grouppolicycategory"></a><span data-ttu-id="95e81-103">Update groupPolicyCategory</span><span class="sxs-lookup"><span data-stu-id="95e81-103">Update groupPolicyCategory</span></span>

<span data-ttu-id="95e81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95e81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95e81-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95e81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95e81-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95e81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95e81-107">Обновление свойств объекта [groupPolicyCategory.](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="95e81-107">Update the properties of a [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95e81-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="95e81-108">Prerequisites</span></span>
<span data-ttu-id="95e81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95e81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95e81-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95e81-111">Permission type</span></span>|<span data-ttu-id="95e81-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95e81-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95e81-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95e81-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95e81-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e81-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95e81-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95e81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95e81-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95e81-116">Not supported.</span></span>|
|<span data-ttu-id="95e81-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="95e81-117">Application</span></span>|<span data-ttu-id="95e81-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e81-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95e81-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95e81-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="95e81-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="95e81-120">Request headers</span></span>
|<span data-ttu-id="95e81-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95e81-121">Header</span></span>|<span data-ttu-id="95e81-122">Значение</span><span class="sxs-lookup"><span data-stu-id="95e81-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95e81-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="95e81-123">Authorization</span></span>|<span data-ttu-id="95e81-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95e81-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95e81-125">Accept</span><span class="sxs-lookup"><span data-stu-id="95e81-125">Accept</span></span>|<span data-ttu-id="95e81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95e81-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95e81-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95e81-127">Request body</span></span>
<span data-ttu-id="95e81-128">В теле запроса поставляем представление JSON для [объекта GroupPolicyCategory.](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="95e81-128">In the request body, supply a JSON representation for the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>

<span data-ttu-id="95e81-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyCategory.](../resources/intune-grouppolicy-grouppolicycategory.md)</span><span class="sxs-lookup"><span data-stu-id="95e81-129">The following table shows the properties that are required when you create the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md).</span></span>

|<span data-ttu-id="95e81-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="95e81-130">Property</span></span>|<span data-ttu-id="95e81-131">Тип</span><span class="sxs-lookup"><span data-stu-id="95e81-131">Type</span></span>|<span data-ttu-id="95e81-132">Описание</span><span class="sxs-lookup"><span data-stu-id="95e81-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95e81-133">displayName</span><span class="sxs-lookup"><span data-stu-id="95e81-133">displayName</span></span>|<span data-ttu-id="95e81-134">Строка</span><span class="sxs-lookup"><span data-stu-id="95e81-134">String</span></span>|<span data-ttu-id="95e81-135">Строковой id имени отображения категории</span><span class="sxs-lookup"><span data-stu-id="95e81-135">The string id of the category's display name</span></span>|
|<span data-ttu-id="95e81-136">isRoot</span><span class="sxs-lookup"><span data-stu-id="95e81-136">isRoot</span></span>|<span data-ttu-id="95e81-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="95e81-137">Boolean</span></span>|<span data-ttu-id="95e81-138">Определяет, является ли категория корневой.</span><span class="sxs-lookup"><span data-stu-id="95e81-138">Defines if the category is a root category</span></span>|
|<span data-ttu-id="95e81-139">id</span><span class="sxs-lookup"><span data-stu-id="95e81-139">id</span></span>|<span data-ttu-id="95e81-140">Строка</span><span class="sxs-lookup"><span data-stu-id="95e81-140">String</span></span>|<span data-ttu-id="95e81-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="95e81-141">Key of the entity.</span></span>|
|<span data-ttu-id="95e81-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95e81-142">lastModifiedDateTime</span></span>|<span data-ttu-id="95e81-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95e81-143">DateTimeOffset</span></span>|<span data-ttu-id="95e81-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="95e81-144">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="95e81-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="95e81-145">Response</span></span>
<span data-ttu-id="95e81-146">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект GroupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="95e81-146">If successful, this method returns a `200 OK` response code and an updated [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95e81-147">Пример</span><span class="sxs-lookup"><span data-stu-id="95e81-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="95e81-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="95e81-148">Request</span></span>
<span data-ttu-id="95e81-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95e81-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories/{groupPolicyCategoryId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "displayName": "Display Name value",
  "isRoot": true
}
```

### <a name="response"></a><span data-ttu-id="95e81-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="95e81-150">Response</span></span>
<span data-ttu-id="95e81-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95e81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "displayName": "Display Name value",
  "isRoot": true,
  "id": "d0641e36-1e36-d064-361e-64d0361e64d0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




