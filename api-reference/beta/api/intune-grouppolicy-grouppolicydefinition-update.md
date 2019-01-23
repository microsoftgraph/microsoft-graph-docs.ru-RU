---
title: Обновление groupPolicyDefinition
description: Обновление свойства объекта groupPolicyDefinition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eeb3e32f1870eac8491989426081df2ae41e4d42
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430639"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="44ec9-103">Обновление groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="44ec9-103">Update groupPolicyDefinition</span></span>

> <span data-ttu-id="44ec9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="44ec9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="44ec9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44ec9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44ec9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44ec9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44ec9-107">Обновление свойства объекта [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="44ec9-107">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44ec9-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="44ec9-108">Prerequisites</span></span>
<span data-ttu-id="44ec9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="44ec9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="44ec9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44ec9-111">Permission type</span></span>|<span data-ttu-id="44ec9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44ec9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44ec9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44ec9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44ec9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44ec9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="44ec9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44ec9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44ec9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44ec9-116">Not supported.</span></span>|
|<span data-ttu-id="44ec9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44ec9-117">Application</span></span>|<span data-ttu-id="44ec9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44ec9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44ec9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44ec9-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="44ec9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44ec9-120">Request headers</span></span>
|<span data-ttu-id="44ec9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44ec9-121">Header</span></span>|<span data-ttu-id="44ec9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="44ec9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44ec9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44ec9-123">Authorization</span></span>|<span data-ttu-id="44ec9-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="44ec9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44ec9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="44ec9-125">Accept</span></span>|<span data-ttu-id="44ec9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44ec9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44ec9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44ec9-127">Request body</span></span>
<span data-ttu-id="44ec9-128">В тексте запроса укажите представление JSON для объекта [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="44ec9-128">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="44ec9-129">В следующей таблице показаны свойства, которые необходимы для создания [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="44ec9-129">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="44ec9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="44ec9-130">Property</span></span>|<span data-ttu-id="44ec9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="44ec9-131">Type</span></span>|<span data-ttu-id="44ec9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="44ec9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44ec9-133">classType</span><span class="sxs-lookup"><span data-stu-id="44ec9-133">classType</span></span>|[<span data-ttu-id="44ec9-134">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="44ec9-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="44ec9-135">Идентифицирует тип групп, которые могут применена политика.</span><span class="sxs-lookup"><span data-stu-id="44ec9-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="44ec9-136">Возможные значения: `user`, `machine`, `both`.</span><span class="sxs-lookup"><span data-stu-id="44ec9-136">Possible values are: `user`, `machine`, `both`.</span></span>|
|<span data-ttu-id="44ec9-137">displayName</span><span class="sxs-lookup"><span data-stu-id="44ec9-137">displayName</span></span>|<span data-ttu-id="44ec9-138">String</span><span class="sxs-lookup"><span data-stu-id="44ec9-138">String</span></span>|<span data-ttu-id="44ec9-139">Имя политики локализованные.</span><span class="sxs-lookup"><span data-stu-id="44ec9-139">The localized policy name.</span></span>|
|<span data-ttu-id="44ec9-140">explainText</span><span class="sxs-lookup"><span data-stu-id="44ec9-140">explainText</span></span>|<span data-ttu-id="44ec9-141">String</span><span class="sxs-lookup"><span data-stu-id="44ec9-141">String</span></span>|<span data-ttu-id="44ec9-142">Локализованные объяснение или справки текст, связанного с политикой.</span><span class="sxs-lookup"><span data-stu-id="44ec9-142">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="44ec9-143">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="44ec9-143">The default value is empty.</span></span>|
|<span data-ttu-id="44ec9-144">categoryPath</span><span class="sxs-lookup"><span data-stu-id="44ec9-144">categoryPath</span></span>|<span data-ttu-id="44ec9-145">String</span><span class="sxs-lookup"><span data-stu-id="44ec9-145">String</span></span>|<span data-ttu-id="44ec9-146">Локализованные категории полный путь для политики.</span><span class="sxs-lookup"><span data-stu-id="44ec9-146">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="44ec9-147">supportedOn</span><span class="sxs-lookup"><span data-stu-id="44ec9-147">supportedOn</span></span>|<span data-ttu-id="44ec9-148">String</span><span class="sxs-lookup"><span data-stu-id="44ec9-148">String</span></span>|<span data-ttu-id="44ec9-149">Локализованные строки, используется, чтобы указать, какие приложения версия операционной системы или определяется политики.</span><span class="sxs-lookup"><span data-stu-id="44ec9-149">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="44ec9-150">policyType</span><span class="sxs-lookup"><span data-stu-id="44ec9-150">policyType</span></span>|[<span data-ttu-id="44ec9-151">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="44ec9-151">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="44ec9-152">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="44ec9-152">Specifies the type of group policy.</span></span> <span data-ttu-id="44ec9-153">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="44ec9-153">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="44ec9-154">id</span><span class="sxs-lookup"><span data-stu-id="44ec9-154">id</span></span>|<span data-ttu-id="44ec9-155">String</span><span class="sxs-lookup"><span data-stu-id="44ec9-155">String</span></span>|<span data-ttu-id="44ec9-156">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="44ec9-156">Key of the entity.</span></span>|
|<span data-ttu-id="44ec9-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44ec9-157">lastModifiedDateTime</span></span>|<span data-ttu-id="44ec9-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44ec9-158">DateTimeOffset</span></span>|<span data-ttu-id="44ec9-159">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="44ec9-159">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="44ec9-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="44ec9-160">Response</span></span>
<span data-ttu-id="44ec9-161">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="44ec9-161">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44ec9-162">Пример</span><span class="sxs-lookup"><span data-stu-id="44ec9-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="44ec9-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="44ec9-163">Request</span></span>
<span data-ttu-id="44ec9-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44ec9-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="44ec9-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="44ec9-165">Response</span></span>
<span data-ttu-id="44ec9-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="44ec9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




