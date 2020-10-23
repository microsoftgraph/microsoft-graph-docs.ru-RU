---
title: Обновление Граупполицидефинитион
description: Обновление свойств объекта Граупполицидефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 57b905857bbe119bba925dae478df403e6069a79
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735423"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="2073f-103">Обновление Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="2073f-103">Update groupPolicyDefinition</span></span>

<span data-ttu-id="2073f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2073f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2073f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2073f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2073f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2073f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2073f-107">Обновление свойств объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="2073f-107">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2073f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2073f-108">Prerequisites</span></span>
<span data-ttu-id="2073f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2073f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2073f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2073f-111">Permission type</span></span>|<span data-ttu-id="2073f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2073f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2073f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2073f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2073f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2073f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2073f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2073f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2073f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2073f-116">Not supported.</span></span>|
|<span data-ttu-id="2073f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2073f-117">Application</span></span>|<span data-ttu-id="2073f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2073f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2073f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2073f-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2073f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2073f-120">Request headers</span></span>
|<span data-ttu-id="2073f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2073f-121">Header</span></span>|<span data-ttu-id="2073f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2073f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2073f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2073f-123">Authorization</span></span>|<span data-ttu-id="2073f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2073f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2073f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2073f-125">Accept</span></span>|<span data-ttu-id="2073f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2073f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2073f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2073f-127">Request body</span></span>
<span data-ttu-id="2073f-128">В тексте запроса добавьте представление объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2073f-128">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="2073f-129">В следующей таблице приведены свойства, необходимые при создании [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="2073f-129">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="2073f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2073f-130">Property</span></span>|<span data-ttu-id="2073f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2073f-131">Type</span></span>|<span data-ttu-id="2073f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2073f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2073f-133">класстипе</span><span class="sxs-lookup"><span data-stu-id="2073f-133">classType</span></span>|[<span data-ttu-id="2073f-134">граупполицидефинитионкласстипе</span><span class="sxs-lookup"><span data-stu-id="2073f-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="2073f-135">Определяет тип групп, к которым можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="2073f-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="2073f-136">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="2073f-136">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="2073f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2073f-137">displayName</span></span>|<span data-ttu-id="2073f-138">Строка</span><span class="sxs-lookup"><span data-stu-id="2073f-138">String</span></span>|<span data-ttu-id="2073f-139">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="2073f-139">The localized policy name.</span></span>|
|<span data-ttu-id="2073f-140">експлаинтекст</span><span class="sxs-lookup"><span data-stu-id="2073f-140">explainText</span></span>|<span data-ttu-id="2073f-141">Строка</span><span class="sxs-lookup"><span data-stu-id="2073f-141">String</span></span>|<span data-ttu-id="2073f-142">Локализованное объяснение или текст справки, связанный с политикой.</span><span class="sxs-lookup"><span data-stu-id="2073f-142">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="2073f-143">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="2073f-143">The default value is empty.</span></span>|
|<span data-ttu-id="2073f-144">категорипас</span><span class="sxs-lookup"><span data-stu-id="2073f-144">categoryPath</span></span>|<span data-ttu-id="2073f-145">Строка</span><span class="sxs-lookup"><span data-stu-id="2073f-145">String</span></span>|<span data-ttu-id="2073f-146">Локализованный полный путь к категории для политики.</span><span class="sxs-lookup"><span data-stu-id="2073f-146">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="2073f-147">суппортедон</span><span class="sxs-lookup"><span data-stu-id="2073f-147">supportedOn</span></span>|<span data-ttu-id="2073f-148">Строка</span><span class="sxs-lookup"><span data-stu-id="2073f-148">String</span></span>|<span data-ttu-id="2073f-149">Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="2073f-149">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="2073f-150">полицитипе</span><span class="sxs-lookup"><span data-stu-id="2073f-150">policyType</span></span>|[<span data-ttu-id="2073f-151">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="2073f-151">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="2073f-152">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="2073f-152">Specifies the type of group policy.</span></span> <span data-ttu-id="2073f-153">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="2073f-153">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="2073f-154">граупполицикатегорид</span><span class="sxs-lookup"><span data-stu-id="2073f-154">groupPolicyCategoryId</span></span>|<span data-ttu-id="2073f-155">Guid</span><span class="sxs-lookup"><span data-stu-id="2073f-155">Guid</span></span>|<span data-ttu-id="2073f-156">Идентификатор категории родительской категории</span><span class="sxs-lookup"><span data-stu-id="2073f-156">The category id of the parent category</span></span>|
|<span data-ttu-id="2073f-157">id</span><span class="sxs-lookup"><span data-stu-id="2073f-157">id</span></span>|<span data-ttu-id="2073f-158">Строка</span><span class="sxs-lookup"><span data-stu-id="2073f-158">String</span></span>|<span data-ttu-id="2073f-159">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2073f-159">Key of the entity.</span></span>|
|<span data-ttu-id="2073f-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2073f-160">lastModifiedDateTime</span></span>|<span data-ttu-id="2073f-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2073f-161">DateTimeOffset</span></span>|<span data-ttu-id="2073f-162">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2073f-162">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="2073f-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="2073f-163">Response</span></span>
<span data-ttu-id="2073f-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2073f-164">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2073f-165">Пример</span><span class="sxs-lookup"><span data-stu-id="2073f-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="2073f-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="2073f-166">Request</span></span>
<span data-ttu-id="2073f-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2073f-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2073f-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="2073f-168">Response</span></span>
<span data-ttu-id="2073f-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2073f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





