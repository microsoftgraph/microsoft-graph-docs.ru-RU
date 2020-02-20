---
title: Создание Граупполициуплоадеддефинитион
description: Создание нового объекта Граупполициуплоадеддефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 18254611d04bb408aa798b2df892d30a9ac14994
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161331"
---
# <a name="create-grouppolicyuploadeddefinition"></a><span data-ttu-id="12c5c-103">Создание Граупполициуплоадеддефинитион</span><span class="sxs-lookup"><span data-stu-id="12c5c-103">Create groupPolicyUploadedDefinition</span></span>

> <span data-ttu-id="12c5c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12c5c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12c5c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12c5c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12c5c-106">Создание нового объекта [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="12c5c-106">Create a new [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12c5c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="12c5c-107">Prerequisites</span></span>
<span data-ttu-id="12c5c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12c5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12c5c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12c5c-110">Permission type</span></span>|<span data-ttu-id="12c5c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12c5c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12c5c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12c5c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12c5c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12c5c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="12c5c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12c5c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12c5c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12c5c-115">Not supported.</span></span>|
|<span data-ttu-id="12c5c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12c5c-116">Application</span></span>|<span data-ttu-id="12c5c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12c5c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12c5c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12c5c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyDefinitions
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions
```

## <a name="request-headers"></a><span data-ttu-id="12c5c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="12c5c-119">Request headers</span></span>
|<span data-ttu-id="12c5c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12c5c-120">Header</span></span>|<span data-ttu-id="12c5c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="12c5c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12c5c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12c5c-122">Authorization</span></span>|<span data-ttu-id="12c5c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12c5c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12c5c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="12c5c-124">Accept</span></span>|<span data-ttu-id="12c5c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12c5c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12c5c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12c5c-126">Request body</span></span>
<span data-ttu-id="12c5c-127">В тексте запроса добавьте представление объекта Граупполициуплоадеддефинитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12c5c-127">In the request body, supply a JSON representation for the groupPolicyUploadedDefinition object.</span></span>

<span data-ttu-id="12c5c-128">В следующей таблице приведены свойства, необходимые при создании Граупполициуплоадеддефинитион.</span><span class="sxs-lookup"><span data-stu-id="12c5c-128">The following table shows the properties that are required when you create the groupPolicyUploadedDefinition.</span></span>

|<span data-ttu-id="12c5c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="12c5c-129">Property</span></span>|<span data-ttu-id="12c5c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="12c5c-130">Type</span></span>|<span data-ttu-id="12c5c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="12c5c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12c5c-132">класстипе</span><span class="sxs-lookup"><span data-stu-id="12c5c-132">classType</span></span>|[<span data-ttu-id="12c5c-133">граупполицидефинитионкласстипе</span><span class="sxs-lookup"><span data-stu-id="12c5c-133">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="12c5c-134">Определяет тип групп, к которым можно применить политику.</span><span class="sxs-lookup"><span data-stu-id="12c5c-134">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="12c5c-135">Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="12c5c-135">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="12c5c-136">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="12c5c-136">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="12c5c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="12c5c-137">displayName</span></span>|<span data-ttu-id="12c5c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="12c5c-138">String</span></span>|<span data-ttu-id="12c5c-139">Имя локализованной политики.</span><span class="sxs-lookup"><span data-stu-id="12c5c-139">The localized policy name.</span></span> <span data-ttu-id="12c5c-140">Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12c5c-140">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="12c5c-141">експлаинтекст</span><span class="sxs-lookup"><span data-stu-id="12c5c-141">explainText</span></span>|<span data-ttu-id="12c5c-142">String</span><span class="sxs-lookup"><span data-stu-id="12c5c-142">String</span></span>|<span data-ttu-id="12c5c-143">Локализованное объяснение или текст справки, связанный с политикой.</span><span class="sxs-lookup"><span data-stu-id="12c5c-143">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="12c5c-144">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="12c5c-144">The default value is empty.</span></span> <span data-ttu-id="12c5c-145">Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12c5c-145">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="12c5c-146">категорипас</span><span class="sxs-lookup"><span data-stu-id="12c5c-146">categoryPath</span></span>|<span data-ttu-id="12c5c-147">String</span><span class="sxs-lookup"><span data-stu-id="12c5c-147">String</span></span>|<span data-ttu-id="12c5c-148">Локализованный полный путь к категории для политики.</span><span class="sxs-lookup"><span data-stu-id="12c5c-148">The localized full category path for the policy.</span></span> <span data-ttu-id="12c5c-149">Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12c5c-149">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="12c5c-150">суппортедон</span><span class="sxs-lookup"><span data-stu-id="12c5c-150">supportedOn</span></span>|<span data-ttu-id="12c5c-151">String</span><span class="sxs-lookup"><span data-stu-id="12c5c-151">String</span></span>|<span data-ttu-id="12c5c-152">Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика.</span><span class="sxs-lookup"><span data-stu-id="12c5c-152">Localized string used to specify what operating system or application version is affected by the policy.</span></span> <span data-ttu-id="12c5c-153">Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12c5c-153">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="12c5c-154">полицитипе</span><span class="sxs-lookup"><span data-stu-id="12c5c-154">policyType</span></span>|[<span data-ttu-id="12c5c-155">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="12c5c-155">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="12c5c-156">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="12c5c-156">Specifies the type of group policy.</span></span> <span data-ttu-id="12c5c-157">Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="12c5c-157">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span> <span data-ttu-id="12c5c-158">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="12c5c-158">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="12c5c-159">id</span><span class="sxs-lookup"><span data-stu-id="12c5c-159">id</span></span>|<span data-ttu-id="12c5c-160">String</span><span class="sxs-lookup"><span data-stu-id="12c5c-160">String</span></span>|<span data-ttu-id="12c5c-161">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="12c5c-161">Key of the entity.</span></span> <span data-ttu-id="12c5c-162">Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12c5c-162">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|
|<span data-ttu-id="12c5c-163">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12c5c-163">lastModifiedDateTime</span></span>|<span data-ttu-id="12c5c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12c5c-164">DateTimeOffset</span></span>|<span data-ttu-id="12c5c-165">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="12c5c-165">The date and time the entity was last modified.</span></span> <span data-ttu-id="12c5c-166">Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="12c5c-166">Inherited from [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="12c5c-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="12c5c-167">Response</span></span>
<span data-ttu-id="12c5c-168">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12c5c-168">If successful, this method returns a `201 Created` response code and a [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12c5c-169">Пример</span><span class="sxs-lookup"><span data-stu-id="12c5c-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="12c5c-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="12c5c-170">Request</span></span>
<span data-ttu-id="12c5c-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12c5c-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions
Content-type: application/json
Content-length: 293

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested"
}
```

### <a name="response"></a><span data-ttu-id="12c5c-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="12c5c-172">Response</span></span>
<span data-ttu-id="12c5c-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12c5c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 406

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "id": "a5f83119-3119-a5f8-1931-f8a51931f8a5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





