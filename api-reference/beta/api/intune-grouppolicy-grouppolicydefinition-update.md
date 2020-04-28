---
title: Обновление Граупполицидефинитион
description: Обновление свойств объекта Граупполицидефинитион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5beddd3ed56da5865335d12394bdb0a6cf51fcd1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454539"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="421e5-103">Обновление Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="421e5-103">Update groupPolicyDefinition</span></span>

<span data-ttu-id="421e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="421e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="421e5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="421e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="421e5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="421e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="421e5-107">Обновление свойств объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="421e5-107">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="421e5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="421e5-108">Prerequisites</span></span>
<span data-ttu-id="421e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="421e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="421e5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="421e5-111">Permission type</span></span>|<span data-ttu-id="421e5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="421e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="421e5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="421e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="421e5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="421e5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="421e5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="421e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="421e5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="421e5-116">Not supported.</span></span>|
|<span data-ttu-id="421e5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="421e5-117">Application</span></span>|<span data-ttu-id="421e5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="421e5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="421e5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="421e5-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="421e5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="421e5-120">Request headers</span></span>
|<span data-ttu-id="421e5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="421e5-121">Header</span></span>|<span data-ttu-id="421e5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="421e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="421e5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="421e5-123">Authorization</span></span>|<span data-ttu-id="421e5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="421e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="421e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="421e5-125">Accept</span></span>|<span data-ttu-id="421e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="421e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="421e5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="421e5-127">Request body</span></span>
<span data-ttu-id="421e5-128">В тексте запроса добавьте представление объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="421e5-128">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="421e5-129">В следующей таблице приведены свойства, необходимые при создании [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="421e5-129">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="421e5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="421e5-130">Property</span></span>|<span data-ttu-id="421e5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="421e5-131">Type</span></span>|<span data-ttu-id="421e5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="421e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="421e5-133">класстипе</span><span class="sxs-lookup"><span data-stu-id="421e5-133">classType</span></span>|[<span data-ttu-id="421e5-134">граупполицидефинитионкласстипе</span><span class="sxs-lookup"><span data-stu-id="421e5-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="421e5-135">Определяет тип групп, к которым можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="421e5-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="421e5-136">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="421e5-136">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="421e5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="421e5-137">displayName</span></span>|<span data-ttu-id="421e5-138">Строка</span><span class="sxs-lookup"><span data-stu-id="421e5-138">String</span></span>|<span data-ttu-id="421e5-139">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="421e5-139">The localized policy name.</span></span>|
|<span data-ttu-id="421e5-140">експлаинтекст</span><span class="sxs-lookup"><span data-stu-id="421e5-140">explainText</span></span>|<span data-ttu-id="421e5-141">String</span><span class="sxs-lookup"><span data-stu-id="421e5-141">String</span></span>|<span data-ttu-id="421e5-142">Локализованное объяснение или текст справки, связанный с политикой.</span><span class="sxs-lookup"><span data-stu-id="421e5-142">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="421e5-143">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="421e5-143">The default value is empty.</span></span>|
|<span data-ttu-id="421e5-144">категорипас</span><span class="sxs-lookup"><span data-stu-id="421e5-144">categoryPath</span></span>|<span data-ttu-id="421e5-145">String</span><span class="sxs-lookup"><span data-stu-id="421e5-145">String</span></span>|<span data-ttu-id="421e5-146">Локализованный полный путь к категории для политики.</span><span class="sxs-lookup"><span data-stu-id="421e5-146">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="421e5-147">суппортедон</span><span class="sxs-lookup"><span data-stu-id="421e5-147">supportedOn</span></span>|<span data-ttu-id="421e5-148">String</span><span class="sxs-lookup"><span data-stu-id="421e5-148">String</span></span>|<span data-ttu-id="421e5-149">Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="421e5-149">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="421e5-150">полицитипе</span><span class="sxs-lookup"><span data-stu-id="421e5-150">policyType</span></span>|[<span data-ttu-id="421e5-151">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="421e5-151">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="421e5-152">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="421e5-152">Specifies the type of group policy.</span></span> <span data-ttu-id="421e5-153">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="421e5-153">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="421e5-154">граупполицикатегорид</span><span class="sxs-lookup"><span data-stu-id="421e5-154">groupPolicyCategoryId</span></span>|<span data-ttu-id="421e5-155">GUID</span><span class="sxs-lookup"><span data-stu-id="421e5-155">Guid</span></span>|<span data-ttu-id="421e5-156">Идентификатор категории родительской категории</span><span class="sxs-lookup"><span data-stu-id="421e5-156">The category id of the parent category</span></span>|
|<span data-ttu-id="421e5-157">id</span><span class="sxs-lookup"><span data-stu-id="421e5-157">id</span></span>|<span data-ttu-id="421e5-158">String</span><span class="sxs-lookup"><span data-stu-id="421e5-158">String</span></span>|<span data-ttu-id="421e5-159">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="421e5-159">Key of the entity.</span></span>|
|<span data-ttu-id="421e5-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="421e5-160">lastModifiedDateTime</span></span>|<span data-ttu-id="421e5-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="421e5-161">DateTimeOffset</span></span>|<span data-ttu-id="421e5-162">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="421e5-162">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="421e5-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="421e5-163">Response</span></span>
<span data-ttu-id="421e5-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="421e5-164">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="421e5-165">Пример</span><span class="sxs-lookup"><span data-stu-id="421e5-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="421e5-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="421e5-166">Request</span></span>
<span data-ttu-id="421e5-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="421e5-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="421e5-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="421e5-168">Response</span></span>
<span data-ttu-id="421e5-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="421e5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



