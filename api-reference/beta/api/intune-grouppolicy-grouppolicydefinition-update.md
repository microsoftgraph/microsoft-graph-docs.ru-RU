---
title: Обновление Граупполицидефинитион
description: Обновление свойств объекта Граупполицидефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7bb2f8568e67a768f7192f9a3ac11610ffb02e10
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984774"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="04642-103">Обновление Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="04642-103">Update groupPolicyDefinition</span></span>

> <span data-ttu-id="04642-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04642-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04642-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04642-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04642-106">Обновление свойств объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="04642-106">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04642-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="04642-107">Prerequisites</span></span>
<span data-ttu-id="04642-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04642-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04642-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04642-110">Permission type</span></span>|<span data-ttu-id="04642-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04642-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04642-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04642-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04642-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04642-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="04642-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04642-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04642-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04642-115">Not supported.</span></span>|
|<span data-ttu-id="04642-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04642-116">Application</span></span>|<span data-ttu-id="04642-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04642-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04642-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04642-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="04642-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04642-119">Request headers</span></span>
|<span data-ttu-id="04642-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04642-120">Header</span></span>|<span data-ttu-id="04642-121">Значение</span><span class="sxs-lookup"><span data-stu-id="04642-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04642-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04642-122">Authorization</span></span>|<span data-ttu-id="04642-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04642-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04642-124">Accept</span><span class="sxs-lookup"><span data-stu-id="04642-124">Accept</span></span>|<span data-ttu-id="04642-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04642-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04642-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="04642-126">Request body</span></span>
<span data-ttu-id="04642-127">В тексте запроса добавьте представление объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04642-127">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="04642-128">В следующей таблице приведены свойства, необходимые при создании [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="04642-128">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="04642-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="04642-129">Property</span></span>|<span data-ttu-id="04642-130">Тип</span><span class="sxs-lookup"><span data-stu-id="04642-130">Type</span></span>|<span data-ttu-id="04642-131">Описание</span><span class="sxs-lookup"><span data-stu-id="04642-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04642-132">Класстипе</span><span class="sxs-lookup"><span data-stu-id="04642-132">classType</span></span>|[<span data-ttu-id="04642-133">Граупполицидефинитионкласстипе</span><span class="sxs-lookup"><span data-stu-id="04642-133">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="04642-134">Определяет тип групп, к которым можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="04642-134">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="04642-135">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="04642-135">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="04642-136">displayName</span><span class="sxs-lookup"><span data-stu-id="04642-136">displayName</span></span>|<span data-ttu-id="04642-137">Строка</span><span class="sxs-lookup"><span data-stu-id="04642-137">String</span></span>|<span data-ttu-id="04642-138">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="04642-138">The localized policy name.</span></span>|
|<span data-ttu-id="04642-139">Експлаинтекст</span><span class="sxs-lookup"><span data-stu-id="04642-139">explainText</span></span>|<span data-ttu-id="04642-140">String</span><span class="sxs-lookup"><span data-stu-id="04642-140">String</span></span>|<span data-ttu-id="04642-141">Локализованное объяснение или текст справки, связанный с политикой.</span><span class="sxs-lookup"><span data-stu-id="04642-141">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="04642-142">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="04642-142">The default value is empty.</span></span>|
|<span data-ttu-id="04642-143">Категорипас</span><span class="sxs-lookup"><span data-stu-id="04642-143">categoryPath</span></span>|<span data-ttu-id="04642-144">String</span><span class="sxs-lookup"><span data-stu-id="04642-144">String</span></span>|<span data-ttu-id="04642-145">Локализованный полный путь к категории для политики.</span><span class="sxs-lookup"><span data-stu-id="04642-145">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="04642-146">Суппортедон</span><span class="sxs-lookup"><span data-stu-id="04642-146">supportedOn</span></span>|<span data-ttu-id="04642-147">String</span><span class="sxs-lookup"><span data-stu-id="04642-147">String</span></span>|<span data-ttu-id="04642-148">Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="04642-148">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="04642-149">Полицитипе</span><span class="sxs-lookup"><span data-stu-id="04642-149">policyType</span></span>|[<span data-ttu-id="04642-150">Граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="04642-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="04642-151">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="04642-151">Specifies the type of group policy.</span></span> <span data-ttu-id="04642-152">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="04642-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="04642-153">id</span><span class="sxs-lookup"><span data-stu-id="04642-153">id</span></span>|<span data-ttu-id="04642-154">String</span><span class="sxs-lookup"><span data-stu-id="04642-154">String</span></span>|<span data-ttu-id="04642-155">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="04642-155">Key of the entity.</span></span>|
|<span data-ttu-id="04642-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04642-156">lastModifiedDateTime</span></span>|<span data-ttu-id="04642-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04642-157">DateTimeOffset</span></span>|<span data-ttu-id="04642-158">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="04642-158">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="04642-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="04642-159">Response</span></span>
<span data-ttu-id="04642-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04642-160">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04642-161">Пример</span><span class="sxs-lookup"><span data-stu-id="04642-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="04642-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="04642-162">Request</span></span>
<span data-ttu-id="04642-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04642-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04642-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="04642-164">Response</span></span>
<span data-ttu-id="04642-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04642-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





