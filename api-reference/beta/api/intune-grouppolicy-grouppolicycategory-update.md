---
title: Обновление Граупполицикатегори
description: Обновление свойств объекта Граупполицикатегори.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: efa4bbb2f4ab8f485d68fd6ce48d13258919ff3c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454759"
---
# <a name="update-grouppolicycategory"></a><span data-ttu-id="2f159-103">Обновление Граупполицикатегори</span><span class="sxs-lookup"><span data-stu-id="2f159-103">Update groupPolicyCategory</span></span>

<span data-ttu-id="2f159-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f159-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f159-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f159-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f159-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f159-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f159-107">Обновление свойств объекта [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md) .</span><span class="sxs-lookup"><span data-stu-id="2f159-107">Update the properties of a [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f159-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2f159-108">Prerequisites</span></span>
<span data-ttu-id="2f159-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f159-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f159-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f159-111">Permission type</span></span>|<span data-ttu-id="2f159-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f159-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f159-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f159-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f159-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f159-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f159-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f159-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f159-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f159-116">Not supported.</span></span>|
|<span data-ttu-id="2f159-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f159-117">Application</span></span>|<span data-ttu-id="2f159-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f159-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f159-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f159-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2f159-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2f159-120">Request headers</span></span>
|<span data-ttu-id="2f159-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f159-121">Header</span></span>|<span data-ttu-id="2f159-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2f159-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f159-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f159-123">Authorization</span></span>|<span data-ttu-id="2f159-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f159-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f159-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2f159-125">Accept</span></span>|<span data-ttu-id="2f159-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f159-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f159-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2f159-127">Request body</span></span>
<span data-ttu-id="2f159-128">В тексте запроса добавьте представление объекта [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f159-128">In the request body, supply a JSON representation for the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object.</span></span>

<span data-ttu-id="2f159-129">В следующей таблице приведены свойства, необходимые при создании [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md).</span><span class="sxs-lookup"><span data-stu-id="2f159-129">The following table shows the properties that are required when you create the [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md).</span></span>

|<span data-ttu-id="2f159-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f159-130">Property</span></span>|<span data-ttu-id="2f159-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2f159-131">Type</span></span>|<span data-ttu-id="2f159-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2f159-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f159-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2f159-133">displayName</span></span>|<span data-ttu-id="2f159-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2f159-134">String</span></span>|<span data-ttu-id="2f159-135">Идентификатор строки отображаемого имени категории</span><span class="sxs-lookup"><span data-stu-id="2f159-135">The string id of the category's display name</span></span>|
|<span data-ttu-id="2f159-136">Корень</span><span class="sxs-lookup"><span data-stu-id="2f159-136">isRoot</span></span>|<span data-ttu-id="2f159-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f159-137">Boolean</span></span>|<span data-ttu-id="2f159-138">Определяет, является ли категория корневой категорией</span><span class="sxs-lookup"><span data-stu-id="2f159-138">Defines if the category is a root category</span></span>|
|<span data-ttu-id="2f159-139">id</span><span class="sxs-lookup"><span data-stu-id="2f159-139">id</span></span>|<span data-ttu-id="2f159-140">String</span><span class="sxs-lookup"><span data-stu-id="2f159-140">String</span></span>|<span data-ttu-id="2f159-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2f159-141">Key of the entity.</span></span>|
|<span data-ttu-id="2f159-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f159-142">lastModifiedDateTime</span></span>|<span data-ttu-id="2f159-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f159-143">DateTimeOffset</span></span>|<span data-ttu-id="2f159-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2f159-144">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="2f159-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f159-145">Response</span></span>
<span data-ttu-id="2f159-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицикатегори](../resources/intune-grouppolicy-grouppolicycategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f159-146">If successful, this method returns a `200 OK` response code and an updated [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f159-147">Пример</span><span class="sxs-lookup"><span data-stu-id="2f159-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f159-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f159-148">Request</span></span>
<span data-ttu-id="2f159-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f159-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f159-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f159-150">Response</span></span>
<span data-ttu-id="2f159-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f159-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



