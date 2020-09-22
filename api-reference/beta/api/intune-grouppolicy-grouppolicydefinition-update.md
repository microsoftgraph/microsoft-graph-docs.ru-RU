---
title: Обновление Граупполицидефинитион
description: Обновление свойств объекта Граупполицидефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3616219253638d603375135aacc88b05045e3c4d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48068317"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="0c37e-103">Обновление Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="0c37e-103">Update groupPolicyDefinition</span></span>

<span data-ttu-id="0c37e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c37e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c37e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c37e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c37e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c37e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c37e-107">Обновление свойств объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="0c37e-107">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c37e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0c37e-108">Prerequisites</span></span>
<span data-ttu-id="0c37e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c37e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c37e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c37e-111">Permission type</span></span>|<span data-ttu-id="0c37e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c37e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c37e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c37e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c37e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c37e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c37e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c37e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c37e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c37e-116">Not supported.</span></span>|
|<span data-ttu-id="0c37e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c37e-117">Application</span></span>|<span data-ttu-id="0c37e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c37e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c37e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c37e-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0c37e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0c37e-120">Request headers</span></span>
|<span data-ttu-id="0c37e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c37e-121">Header</span></span>|<span data-ttu-id="0c37e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0c37e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c37e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c37e-123">Authorization</span></span>|<span data-ttu-id="0c37e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c37e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c37e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0c37e-125">Accept</span></span>|<span data-ttu-id="0c37e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c37e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c37e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c37e-127">Request body</span></span>
<span data-ttu-id="0c37e-128">В тексте запроса добавьте представление объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c37e-128">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="0c37e-129">В следующей таблице приведены свойства, необходимые при создании [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0c37e-129">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="0c37e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c37e-130">Property</span></span>|<span data-ttu-id="0c37e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0c37e-131">Type</span></span>|<span data-ttu-id="0c37e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0c37e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c37e-133">класстипе</span><span class="sxs-lookup"><span data-stu-id="0c37e-133">classType</span></span>|[<span data-ttu-id="0c37e-134">граупполицидефинитионкласстипе</span><span class="sxs-lookup"><span data-stu-id="0c37e-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="0c37e-135">Определяет тип групп, к которым можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="0c37e-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="0c37e-136">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="0c37e-136">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="0c37e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0c37e-137">displayName</span></span>|<span data-ttu-id="0c37e-138">String</span><span class="sxs-lookup"><span data-stu-id="0c37e-138">String</span></span>|<span data-ttu-id="0c37e-139">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="0c37e-139">The localized policy name.</span></span>|
|<span data-ttu-id="0c37e-140">експлаинтекст</span><span class="sxs-lookup"><span data-stu-id="0c37e-140">explainText</span></span>|<span data-ttu-id="0c37e-141">String</span><span class="sxs-lookup"><span data-stu-id="0c37e-141">String</span></span>|<span data-ttu-id="0c37e-142">Локализованное объяснение или текст справки, связанный с политикой.</span><span class="sxs-lookup"><span data-stu-id="0c37e-142">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="0c37e-143">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="0c37e-143">The default value is empty.</span></span>|
|<span data-ttu-id="0c37e-144">категорипас</span><span class="sxs-lookup"><span data-stu-id="0c37e-144">categoryPath</span></span>|<span data-ttu-id="0c37e-145">String</span><span class="sxs-lookup"><span data-stu-id="0c37e-145">String</span></span>|<span data-ttu-id="0c37e-146">Локализованный полный путь к категории для политики.</span><span class="sxs-lookup"><span data-stu-id="0c37e-146">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="0c37e-147">суппортедон</span><span class="sxs-lookup"><span data-stu-id="0c37e-147">supportedOn</span></span>|<span data-ttu-id="0c37e-148">String</span><span class="sxs-lookup"><span data-stu-id="0c37e-148">String</span></span>|<span data-ttu-id="0c37e-149">Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="0c37e-149">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="0c37e-150">полицитипе</span><span class="sxs-lookup"><span data-stu-id="0c37e-150">policyType</span></span>|[<span data-ttu-id="0c37e-151">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="0c37e-151">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="0c37e-152">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="0c37e-152">Specifies the type of group policy.</span></span> <span data-ttu-id="0c37e-153">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="0c37e-153">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="0c37e-154">граупполицикатегорид</span><span class="sxs-lookup"><span data-stu-id="0c37e-154">groupPolicyCategoryId</span></span>|<span data-ttu-id="0c37e-155">Guid</span><span class="sxs-lookup"><span data-stu-id="0c37e-155">Guid</span></span>|<span data-ttu-id="0c37e-156">Идентификатор категории родительской категории</span><span class="sxs-lookup"><span data-stu-id="0c37e-156">The category id of the parent category</span></span>|
|<span data-ttu-id="0c37e-157">id</span><span class="sxs-lookup"><span data-stu-id="0c37e-157">id</span></span>|<span data-ttu-id="0c37e-158">String</span><span class="sxs-lookup"><span data-stu-id="0c37e-158">String</span></span>|<span data-ttu-id="0c37e-159">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0c37e-159">Key of the entity.</span></span>|
|<span data-ttu-id="0c37e-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c37e-160">lastModifiedDateTime</span></span>|<span data-ttu-id="0c37e-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c37e-161">DateTimeOffset</span></span>|<span data-ttu-id="0c37e-162">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0c37e-162">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="0c37e-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c37e-163">Response</span></span>
<span data-ttu-id="0c37e-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0c37e-164">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c37e-165">Пример</span><span class="sxs-lookup"><span data-stu-id="0c37e-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c37e-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c37e-166">Request</span></span>
<span data-ttu-id="0c37e-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c37e-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c37e-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c37e-168">Response</span></span>
<span data-ttu-id="0c37e-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c37e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






