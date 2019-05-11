---
title: Обновление Граупполицидефинитион
description: Обновление свойств объекта Граупполицидефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf706f941ef7535bbd0a89d3d126790e44d95853
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33905121"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="0c31c-103">Обновление Граупполицидефинитион</span><span class="sxs-lookup"><span data-stu-id="0c31c-103">Update groupPolicyDefinition</span></span>

> <span data-ttu-id="0c31c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c31c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c31c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c31c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c31c-106">Обновление свойств объекта [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="0c31c-106">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c31c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0c31c-107">Prerequisites</span></span>
<span data-ttu-id="0c31c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c31c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c31c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c31c-110">Permission type</span></span>|<span data-ttu-id="0c31c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c31c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c31c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c31c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c31c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c31c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0c31c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c31c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c31c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c31c-115">Not supported.</span></span>|
|<span data-ttu-id="0c31c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c31c-116">Application</span></span>|<span data-ttu-id="0c31c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c31c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c31c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c31c-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0c31c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c31c-119">Request headers</span></span>
|<span data-ttu-id="0c31c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c31c-120">Header</span></span>|<span data-ttu-id="0c31c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0c31c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c31c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c31c-122">Authorization</span></span>|<span data-ttu-id="0c31c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c31c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c31c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0c31c-124">Accept</span></span>|<span data-ttu-id="0c31c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c31c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c31c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c31c-126">Request body</span></span>
<span data-ttu-id="0c31c-127">В тексте запроса добавьте представление объекта [Граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c31c-127">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="0c31c-128">В следующей таблице приведены свойства, необходимые при создании [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0c31c-128">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="0c31c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c31c-129">Property</span></span>|<span data-ttu-id="0c31c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0c31c-130">Type</span></span>|<span data-ttu-id="0c31c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0c31c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c31c-132">Класстипе</span><span class="sxs-lookup"><span data-stu-id="0c31c-132">classType</span></span>|[<span data-ttu-id="0c31c-133">Граупполицидефинитионкласстипе</span><span class="sxs-lookup"><span data-stu-id="0c31c-133">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="0c31c-134">Определяет тип групп, к которым можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="0c31c-134">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="0c31c-135">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="0c31c-135">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="0c31c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0c31c-136">displayName</span></span>|<span data-ttu-id="0c31c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="0c31c-137">String</span></span>|<span data-ttu-id="0c31c-138">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="0c31c-138">The localized policy name.</span></span>|
|<span data-ttu-id="0c31c-139">Експлаинтекст</span><span class="sxs-lookup"><span data-stu-id="0c31c-139">explainText</span></span>|<span data-ttu-id="0c31c-140">Строка</span><span class="sxs-lookup"><span data-stu-id="0c31c-140">String</span></span>|<span data-ttu-id="0c31c-141">Локализованное объяснение или текст справки, связанный с политикой.</span><span class="sxs-lookup"><span data-stu-id="0c31c-141">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="0c31c-142">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="0c31c-142">The default value is empty.</span></span>|
|<span data-ttu-id="0c31c-143">Категорипас</span><span class="sxs-lookup"><span data-stu-id="0c31c-143">categoryPath</span></span>|<span data-ttu-id="0c31c-144">Строка</span><span class="sxs-lookup"><span data-stu-id="0c31c-144">String</span></span>|<span data-ttu-id="0c31c-145">Локализованный полный путь к категории для политики.</span><span class="sxs-lookup"><span data-stu-id="0c31c-145">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="0c31c-146">Суппортедон</span><span class="sxs-lookup"><span data-stu-id="0c31c-146">supportedOn</span></span>|<span data-ttu-id="0c31c-147">Строка</span><span class="sxs-lookup"><span data-stu-id="0c31c-147">String</span></span>|<span data-ttu-id="0c31c-148">Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="0c31c-148">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="0c31c-149">Полицитипе</span><span class="sxs-lookup"><span data-stu-id="0c31c-149">policyType</span></span>|[<span data-ttu-id="0c31c-150">Граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="0c31c-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="0c31c-151">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="0c31c-151">Specifies the type of group policy.</span></span> <span data-ttu-id="0c31c-152">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="0c31c-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="0c31c-153">id</span><span class="sxs-lookup"><span data-stu-id="0c31c-153">id</span></span>|<span data-ttu-id="0c31c-154">String</span><span class="sxs-lookup"><span data-stu-id="0c31c-154">String</span></span>|<span data-ttu-id="0c31c-155">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0c31c-155">Key of the entity.</span></span>|
|<span data-ttu-id="0c31c-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c31c-156">lastModifiedDateTime</span></span>|<span data-ttu-id="0c31c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c31c-157">DateTimeOffset</span></span>|<span data-ttu-id="0c31c-158">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0c31c-158">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="0c31c-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c31c-159">Response</span></span>
<span data-ttu-id="0c31c-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0c31c-160">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c31c-161">Пример</span><span class="sxs-lookup"><span data-stu-id="0c31c-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c31c-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c31c-162">Request</span></span>
<span data-ttu-id="0c31c-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c31c-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c31c-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c31c-164">Response</span></span>
<span data-ttu-id="0c31c-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c31c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




