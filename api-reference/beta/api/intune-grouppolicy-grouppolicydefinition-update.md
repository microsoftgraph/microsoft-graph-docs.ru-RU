---
title: Обновление Граупполицидефинитион
description: Обновление свойств объекта Граупполицидефинитион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 02010b63320f295dad8ec5d5c579d5aa19d0a062
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804431"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="6c6d6-103">Обновление Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="6c6d6-103">Update groupPolicyDefinition</span></span>

> <span data-ttu-id="6c6d6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c6d6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c6d6-106">Обновление свойств объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="6c6d6-106">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c6d6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6c6d6-107">Prerequisites</span></span>
<span data-ttu-id="6c6d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c6d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c6d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c6d6-110">Permission type</span></span>|<span data-ttu-id="6c6d6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c6d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c6d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c6d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c6d6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c6d6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6c6d6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c6d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c6d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-115">Not supported.</span></span>|
|<span data-ttu-id="6c6d6-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6c6d6-116">Application</span></span>|<span data-ttu-id="6c6d6-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c6d6-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c6d6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c6d6-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="6c6d6-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6c6d6-119">Request headers</span></span>
|<span data-ttu-id="6c6d6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c6d6-120">Header</span></span>|<span data-ttu-id="6c6d6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6c6d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c6d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c6d6-122">Authorization</span></span>|<span data-ttu-id="6c6d6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c6d6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6c6d6-124">Accept</span></span>|<span data-ttu-id="6c6d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c6d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c6d6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c6d6-126">Request body</span></span>
<span data-ttu-id="6c6d6-127">В тексте запроса добавьте представление объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-127">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="6c6d6-128">В следующей таблице приведены свойства, необходимые при создании [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6c6d6-128">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="6c6d6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c6d6-129">Property</span></span>|<span data-ttu-id="6c6d6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6c6d6-130">Type</span></span>|<span data-ttu-id="6c6d6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6c6d6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c6d6-132">класстипе</span><span class="sxs-lookup"><span data-stu-id="6c6d6-132">classType</span></span>|[<span data-ttu-id="6c6d6-133">граупполицидефинитионкласстипе</span><span class="sxs-lookup"><span data-stu-id="6c6d6-133">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="6c6d6-134">Определяет тип групп, к которым можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-134">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="6c6d6-135">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-135">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="6c6d6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6c6d6-136">displayName</span></span>|<span data-ttu-id="6c6d6-137">Строка</span><span class="sxs-lookup"><span data-stu-id="6c6d6-137">String</span></span>|<span data-ttu-id="6c6d6-138">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-138">The localized policy name.</span></span>|
|<span data-ttu-id="6c6d6-139">експлаинтекст</span><span class="sxs-lookup"><span data-stu-id="6c6d6-139">explainText</span></span>|<span data-ttu-id="6c6d6-140">String</span><span class="sxs-lookup"><span data-stu-id="6c6d6-140">String</span></span>|<span data-ttu-id="6c6d6-141">Локализованное объяснение или текст справки, связанный с политикой.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-141">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="6c6d6-142">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-142">The default value is empty.</span></span>|
|<span data-ttu-id="6c6d6-143">категорипас</span><span class="sxs-lookup"><span data-stu-id="6c6d6-143">categoryPath</span></span>|<span data-ttu-id="6c6d6-144">String</span><span class="sxs-lookup"><span data-stu-id="6c6d6-144">String</span></span>|<span data-ttu-id="6c6d6-145">Локализованный полный путь к категории для политики.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-145">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="6c6d6-146">суппортедон</span><span class="sxs-lookup"><span data-stu-id="6c6d6-146">supportedOn</span></span>|<span data-ttu-id="6c6d6-147">String</span><span class="sxs-lookup"><span data-stu-id="6c6d6-147">String</span></span>|<span data-ttu-id="6c6d6-148">Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-148">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="6c6d6-149">полицитипе</span><span class="sxs-lookup"><span data-stu-id="6c6d6-149">policyType</span></span>|[<span data-ttu-id="6c6d6-150">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="6c6d6-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="6c6d6-151">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-151">Specifies the type of group policy.</span></span> <span data-ttu-id="6c6d6-152">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="6c6d6-153">граупполицикатегорид</span><span class="sxs-lookup"><span data-stu-id="6c6d6-153">groupPolicyCategoryId</span></span>|<span data-ttu-id="6c6d6-154">GUID</span><span class="sxs-lookup"><span data-stu-id="6c6d6-154">Guid</span></span>|<span data-ttu-id="6c6d6-155">Идентификатор категории родительской категории</span><span class="sxs-lookup"><span data-stu-id="6c6d6-155">The category id of the parent category</span></span>|
|<span data-ttu-id="6c6d6-156">id</span><span class="sxs-lookup"><span data-stu-id="6c6d6-156">id</span></span>|<span data-ttu-id="6c6d6-157">String</span><span class="sxs-lookup"><span data-stu-id="6c6d6-157">String</span></span>|<span data-ttu-id="6c6d6-158">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-158">Key of the entity.</span></span>|
|<span data-ttu-id="6c6d6-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c6d6-159">lastModifiedDateTime</span></span>|<span data-ttu-id="6c6d6-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c6d6-160">DateTimeOffset</span></span>|<span data-ttu-id="6c6d6-161">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-161">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="6c6d6-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c6d6-162">Response</span></span>
<span data-ttu-id="6c6d6-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-163">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c6d6-164">Пример</span><span class="sxs-lookup"><span data-stu-id="6c6d6-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c6d6-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c6d6-165">Request</span></span>
<span data-ttu-id="6c6d6-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
Content-type: application/json
Content-length: 353

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d"
}
```

### <a name="response"></a><span data-ttu-id="6c6d6-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c6d6-167">Response</span></span>
<span data-ttu-id="6c6d6-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c6d6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 466

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
  "id": "f9607947-7947-f960-4779-60f9477960f9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




