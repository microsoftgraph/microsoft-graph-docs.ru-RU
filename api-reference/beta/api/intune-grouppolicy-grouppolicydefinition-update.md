---
title: Обновление Граупполицидефинитион
description: Обновление свойств объекта Граупполицидефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c9470b2affadb3ea0cdd38f1dbbb8dd9d44fa966
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465168"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="c9643-103">Обновление Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="c9643-103">Update groupPolicyDefinition</span></span>

<span data-ttu-id="c9643-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c9643-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9643-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9643-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9643-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9643-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9643-107">Обновление свойств объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="c9643-107">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9643-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c9643-108">Prerequisites</span></span>
<span data-ttu-id="c9643-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9643-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9643-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9643-111">Permission type</span></span>|<span data-ttu-id="c9643-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9643-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9643-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9643-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9643-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9643-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c9643-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9643-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9643-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9643-116">Not supported.</span></span>|
|<span data-ttu-id="c9643-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9643-117">Application</span></span>|<span data-ttu-id="c9643-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9643-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9643-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9643-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions/{groupPolicyDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="c9643-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c9643-120">Request headers</span></span>
|<span data-ttu-id="c9643-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9643-121">Header</span></span>|<span data-ttu-id="c9643-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c9643-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9643-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9643-123">Authorization</span></span>|<span data-ttu-id="c9643-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9643-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9643-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c9643-125">Accept</span></span>|<span data-ttu-id="c9643-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9643-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9643-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9643-127">Request body</span></span>
<span data-ttu-id="c9643-128">В тексте запроса добавьте представление объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9643-128">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="c9643-129">В следующей таблице приведены свойства, необходимые при создании [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c9643-129">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="c9643-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9643-130">Property</span></span>|<span data-ttu-id="c9643-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c9643-131">Type</span></span>|<span data-ttu-id="c9643-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c9643-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9643-133">класстипе</span><span class="sxs-lookup"><span data-stu-id="c9643-133">classType</span></span>|[<span data-ttu-id="c9643-134">граупполицидефинитионкласстипе</span><span class="sxs-lookup"><span data-stu-id="c9643-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="c9643-135">Определяет тип групп, к которым можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="c9643-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="c9643-136">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="c9643-136">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="c9643-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c9643-137">displayName</span></span>|<span data-ttu-id="c9643-138">Строка</span><span class="sxs-lookup"><span data-stu-id="c9643-138">String</span></span>|<span data-ttu-id="c9643-139">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="c9643-139">The localized policy name.</span></span>|
|<span data-ttu-id="c9643-140">експлаинтекст</span><span class="sxs-lookup"><span data-stu-id="c9643-140">explainText</span></span>|<span data-ttu-id="c9643-141">String</span><span class="sxs-lookup"><span data-stu-id="c9643-141">String</span></span>|<span data-ttu-id="c9643-142">Локализованное объяснение или текст справки, связанный с политикой.</span><span class="sxs-lookup"><span data-stu-id="c9643-142">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="c9643-143">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="c9643-143">The default value is empty.</span></span>|
|<span data-ttu-id="c9643-144">категорипас</span><span class="sxs-lookup"><span data-stu-id="c9643-144">categoryPath</span></span>|<span data-ttu-id="c9643-145">String</span><span class="sxs-lookup"><span data-stu-id="c9643-145">String</span></span>|<span data-ttu-id="c9643-146">Локализованный полный путь к категории для политики.</span><span class="sxs-lookup"><span data-stu-id="c9643-146">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="c9643-147">суппортедон</span><span class="sxs-lookup"><span data-stu-id="c9643-147">supportedOn</span></span>|<span data-ttu-id="c9643-148">String</span><span class="sxs-lookup"><span data-stu-id="c9643-148">String</span></span>|<span data-ttu-id="c9643-149">Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="c9643-149">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="c9643-150">полицитипе</span><span class="sxs-lookup"><span data-stu-id="c9643-150">policyType</span></span>|[<span data-ttu-id="c9643-151">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="c9643-151">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="c9643-152">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="c9643-152">Specifies the type of group policy.</span></span> <span data-ttu-id="c9643-153">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="c9643-153">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="c9643-154">id</span><span class="sxs-lookup"><span data-stu-id="c9643-154">id</span></span>|<span data-ttu-id="c9643-155">String</span><span class="sxs-lookup"><span data-stu-id="c9643-155">String</span></span>|<span data-ttu-id="c9643-156">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c9643-156">Key of the entity.</span></span>|
|<span data-ttu-id="c9643-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9643-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c9643-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9643-158">DateTimeOffset</span></span>|<span data-ttu-id="c9643-159">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c9643-159">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="c9643-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9643-160">Response</span></span>
<span data-ttu-id="c9643-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9643-161">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9643-162">Пример</span><span class="sxs-lookup"><span data-stu-id="c9643-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9643-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9643-163">Request</span></span>
<span data-ttu-id="c9643-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9643-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
Content-type: application/json
Content-length: 285

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested"
}
```

### <a name="response"></a><span data-ttu-id="c9643-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9643-165">Response</span></span>
<span data-ttu-id="c9643-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9643-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "id": "f9607947-7947-f960-4779-60f9477960f9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





