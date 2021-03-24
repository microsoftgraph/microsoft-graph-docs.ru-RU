---
title: Update groupPolicyUploadedDefinition
description: Обновление свойств объекта groupPolicyUploadedDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f643d8f957590f2a619174ccc50545bdd5b53520
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135280"
---
# <a name="update-grouppolicyuploadeddefinition"></a><span data-ttu-id="c4c8c-103">Update groupPolicyUploadedDefinition</span><span class="sxs-lookup"><span data-stu-id="c4c8c-103">Update groupPolicyUploadedDefinition</span></span>

<span data-ttu-id="c4c8c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4c8c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4c8c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4c8c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4c8c-107">Обновление свойств объекта [groupPolicyUploadedDefinition.](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c4c8c-107">Update the properties of a [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4c8c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c4c8c-108">Prerequisites</span></span>
<span data-ttu-id="c4c8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4c8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4c8c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4c8c-111">Permission type</span></span>|<span data-ttu-id="c4c8c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4c8c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4c8c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4c8c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4c8c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4c8c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4c8c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4c8c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4c8c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-116">Not supported.</span></span>|
|<span data-ttu-id="c4c8c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c4c8c-117">Application</span></span>|<span data-ttu-id="c4c8c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4c8c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4c8c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4c8c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitions/{groupPolicyDefinitionId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions/{groupPolicyDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="c4c8c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c4c8c-120">Request headers</span></span>
|<span data-ttu-id="c4c8c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4c8c-121">Header</span></span>|<span data-ttu-id="c4c8c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c4c8c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4c8c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4c8c-123">Authorization</span></span>|<span data-ttu-id="c4c8c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4c8c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c4c8c-125">Accept</span></span>|<span data-ttu-id="c4c8c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4c8c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4c8c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4c8c-127">Request body</span></span>
<span data-ttu-id="c4c8c-128">В теле запроса поставляем представление JSON для [объекта groupPolicyUploadedDefinition.](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c4c8c-128">In the request body, supply a JSON representation for the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

<span data-ttu-id="c4c8c-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyUploadedDefinition.](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c4c8c-129">The following table shows the properties that are required when you create the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md).</span></span>

|<span data-ttu-id="c4c8c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4c8c-130">Property</span></span>|<span data-ttu-id="c4c8c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c4c8c-131">Type</span></span>|<span data-ttu-id="c4c8c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c4c8c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4c8c-133">classType</span><span class="sxs-lookup"><span data-stu-id="c4c8c-133">classType</span></span>|[<span data-ttu-id="c4c8c-134">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="c4c8c-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="c4c8c-135">Определяет тип групп, к которые можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="c4c8c-136">Унаследовано от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c4c8c-136">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="c4c8c-137">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-137">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="c4c8c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="c4c8c-138">displayName</span></span>|<span data-ttu-id="c4c8c-139">Строка</span><span class="sxs-lookup"><span data-stu-id="c4c8c-139">String</span></span>|<span data-ttu-id="c4c8c-140">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-140">The localized policy name.</span></span> <span data-ttu-id="c4c8c-141">Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c4c8c-141">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="c4c8c-142">explainText</span><span class="sxs-lookup"><span data-stu-id="c4c8c-142">explainText</span></span>|<span data-ttu-id="c4c8c-143">Строка</span><span class="sxs-lookup"><span data-stu-id="c4c8c-143">String</span></span>|<span data-ttu-id="c4c8c-144">Локализованный текст объяснения или справки, связанные с политикой.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-144">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="c4c8c-145">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-145">The default value is empty.</span></span> <span data-ttu-id="c4c8c-146">Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c4c8c-146">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="c4c8c-147">categoryPath</span><span class="sxs-lookup"><span data-stu-id="c4c8c-147">categoryPath</span></span>|<span data-ttu-id="c4c8c-148">Строка</span><span class="sxs-lookup"><span data-stu-id="c4c8c-148">String</span></span>|<span data-ttu-id="c4c8c-149">Путь к локализованным полным категориям для политики.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-149">The localized full category path for the policy.</span></span> <span data-ttu-id="c4c8c-150">Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c4c8c-150">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="c4c8c-151">supportedOn</span><span class="sxs-lookup"><span data-stu-id="c4c8c-151">supportedOn</span></span>|<span data-ttu-id="c4c8c-152">Строка</span><span class="sxs-lookup"><span data-stu-id="c4c8c-152">String</span></span>|<span data-ttu-id="c4c8c-153">Локализованная строка, используемая для указания того, на какую операционную систему или версию приложения влияет политика.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-153">Localized string used to specify what operating system or application version is affected by the policy.</span></span> <span data-ttu-id="c4c8c-154">Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c4c8c-154">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="c4c8c-155">policyType</span><span class="sxs-lookup"><span data-stu-id="c4c8c-155">policyType</span></span>|[<span data-ttu-id="c4c8c-156">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="c4c8c-156">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="c4c8c-157">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-157">Specifies the type of group policy.</span></span> <span data-ttu-id="c4c8c-158">Унаследовано от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c4c8c-158">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="c4c8c-159">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-159">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="c4c8c-160">groupPolicyCategoryId</span><span class="sxs-lookup"><span data-stu-id="c4c8c-160">groupPolicyCategoryId</span></span>|<span data-ttu-id="c4c8c-161">Guid</span><span class="sxs-lookup"><span data-stu-id="c4c8c-161">Guid</span></span>|<span data-ttu-id="c4c8c-162">ID категории родительской категории, унаследованной от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c4c8c-162">The category id of the parent category Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="c4c8c-163">id</span><span class="sxs-lookup"><span data-stu-id="c4c8c-163">id</span></span>|<span data-ttu-id="c4c8c-164">Строка</span><span class="sxs-lookup"><span data-stu-id="c4c8c-164">String</span></span>|<span data-ttu-id="c4c8c-165">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-165">Key of the entity.</span></span> <span data-ttu-id="c4c8c-166">Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c4c8c-166">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="c4c8c-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4c8c-167">lastModifiedDateTime</span></span>|<span data-ttu-id="c4c8c-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4c8c-168">DateTimeOffset</span></span>|<span data-ttu-id="c4c8c-169">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-169">The date and time the entity was last modified.</span></span> <span data-ttu-id="c4c8c-170">Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c4c8c-170">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c4c8c-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4c8c-171">Response</span></span>
<span data-ttu-id="c4c8c-172">В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-172">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4c8c-173">Пример</span><span class="sxs-lookup"><span data-stu-id="c4c8c-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4c8c-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4c8c-174">Request</span></span>
<span data-ttu-id="c4c8c-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d"
}
```

### <a name="response"></a><span data-ttu-id="c4c8c-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4c8c-176">Response</span></span>
<span data-ttu-id="c4c8c-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4c8c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 474

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
  "id": "a5f83119-3119-a5f8-1931-f8a51931f8a5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




