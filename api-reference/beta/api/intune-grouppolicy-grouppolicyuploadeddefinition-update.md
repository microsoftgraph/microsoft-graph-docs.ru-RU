---
title: Обновление Граупполициуплоадеддефинитион
description: Обновление свойств объекта Граупполициуплоадеддефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4103b13e8dc7c34c0fb7b9fe90c1e7d01c0f3c06
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49224979"
---
# <a name="update-grouppolicyuploadeddefinition"></a><span data-ttu-id="0af4d-103">Обновление Граупполициуплоадеддефинитион</span><span class="sxs-lookup"><span data-stu-id="0af4d-103">Update groupPolicyUploadedDefinition</span></span>

<span data-ttu-id="0af4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0af4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0af4d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0af4d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0af4d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0af4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0af4d-107">Обновление свойств объекта [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="0af4d-107">Update the properties of a [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0af4d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0af4d-108">Prerequisites</span></span>
<span data-ttu-id="0af4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0af4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0af4d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0af4d-111">Permission type</span></span>|<span data-ttu-id="0af4d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0af4d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0af4d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0af4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0af4d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0af4d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0af4d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0af4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0af4d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0af4d-116">Not supported.</span></span>|
|<span data-ttu-id="0af4d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0af4d-117">Application</span></span>|<span data-ttu-id="0af4d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0af4d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0af4d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0af4d-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0af4d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0af4d-120">Request headers</span></span>
|<span data-ttu-id="0af4d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0af4d-121">Header</span></span>|<span data-ttu-id="0af4d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0af4d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0af4d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0af4d-123">Authorization</span></span>|<span data-ttu-id="0af4d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0af4d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0af4d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0af4d-125">Accept</span></span>|<span data-ttu-id="0af4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0af4d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0af4d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0af4d-127">Request body</span></span>
<span data-ttu-id="0af4d-128">В тексте запроса добавьте представление объекта [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0af4d-128">In the request body, supply a JSON representation for the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

<span data-ttu-id="0af4d-129">В следующей таблице приведены свойства, необходимые при создании [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0af4d-129">The following table shows the properties that are required when you create the [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md).</span></span>

|<span data-ttu-id="0af4d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0af4d-130">Property</span></span>|<span data-ttu-id="0af4d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0af4d-131">Type</span></span>|<span data-ttu-id="0af4d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0af4d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0af4d-133">класстипе</span><span class="sxs-lookup"><span data-stu-id="0af4d-133">classType</span></span>|[<span data-ttu-id="0af4d-134">граупполицидефинитионкласстипе</span><span class="sxs-lookup"><span data-stu-id="0af4d-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="0af4d-135">Определяет тип групп, к которым можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="0af4d-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="0af4d-136">Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0af4d-136">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="0af4d-137">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="0af4d-137">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="0af4d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0af4d-138">displayName</span></span>|<span data-ttu-id="0af4d-139">String</span><span class="sxs-lookup"><span data-stu-id="0af4d-139">String</span></span>|<span data-ttu-id="0af4d-140">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="0af4d-140">The localized policy name.</span></span> <span data-ttu-id="0af4d-141">Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0af4d-141">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="0af4d-142">експлаинтекст</span><span class="sxs-lookup"><span data-stu-id="0af4d-142">explainText</span></span>|<span data-ttu-id="0af4d-143">String</span><span class="sxs-lookup"><span data-stu-id="0af4d-143">String</span></span>|<span data-ttu-id="0af4d-144">Локализованное объяснение или текст справки, связанный с политикой.</span><span class="sxs-lookup"><span data-stu-id="0af4d-144">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="0af4d-145">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="0af4d-145">The default value is empty.</span></span> <span data-ttu-id="0af4d-146">Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0af4d-146">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="0af4d-147">категорипас</span><span class="sxs-lookup"><span data-stu-id="0af4d-147">categoryPath</span></span>|<span data-ttu-id="0af4d-148">String</span><span class="sxs-lookup"><span data-stu-id="0af4d-148">String</span></span>|<span data-ttu-id="0af4d-149">Локализованный полный путь к категории для политики.</span><span class="sxs-lookup"><span data-stu-id="0af4d-149">The localized full category path for the policy.</span></span> <span data-ttu-id="0af4d-150">Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0af4d-150">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="0af4d-151">суппортедон</span><span class="sxs-lookup"><span data-stu-id="0af4d-151">supportedOn</span></span>|<span data-ttu-id="0af4d-152">String</span><span class="sxs-lookup"><span data-stu-id="0af4d-152">String</span></span>|<span data-ttu-id="0af4d-153">Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="0af4d-153">Localized string used to specify what operating system or application version is affected by the policy.</span></span> <span data-ttu-id="0af4d-154">Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0af4d-154">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="0af4d-155">полицитипе</span><span class="sxs-lookup"><span data-stu-id="0af4d-155">policyType</span></span>|[<span data-ttu-id="0af4d-156">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="0af4d-156">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="0af4d-157">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="0af4d-157">Specifies the type of group policy.</span></span> <span data-ttu-id="0af4d-158">Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0af4d-158">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="0af4d-159">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="0af4d-159">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="0af4d-160">граупполицикатегорид</span><span class="sxs-lookup"><span data-stu-id="0af4d-160">groupPolicyCategoryId</span></span>|<span data-ttu-id="0af4d-161">Guid</span><span class="sxs-lookup"><span data-stu-id="0af4d-161">Guid</span></span>|<span data-ttu-id="0af4d-162">Идентификатор категории родительской категории, унаследованной от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0af4d-162">The category id of the parent category Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="0af4d-163">id</span><span class="sxs-lookup"><span data-stu-id="0af4d-163">id</span></span>|<span data-ttu-id="0af4d-164">String</span><span class="sxs-lookup"><span data-stu-id="0af4d-164">String</span></span>|<span data-ttu-id="0af4d-165">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0af4d-165">Key of the entity.</span></span> <span data-ttu-id="0af4d-166">Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0af4d-166">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="0af4d-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0af4d-167">lastModifiedDateTime</span></span>|<span data-ttu-id="0af4d-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0af4d-168">DateTimeOffset</span></span>|<span data-ttu-id="0af4d-169">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0af4d-169">The date and time the entity was last modified.</span></span> <span data-ttu-id="0af4d-170">Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0af4d-170">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0af4d-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="0af4d-171">Response</span></span>
<span data-ttu-id="0af4d-172">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0af4d-172">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0af4d-173">Пример</span><span class="sxs-lookup"><span data-stu-id="0af4d-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="0af4d-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="0af4d-174">Request</span></span>
<span data-ttu-id="0af4d-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0af4d-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0af4d-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="0af4d-176">Response</span></span>
<span data-ttu-id="0af4d-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0af4d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




