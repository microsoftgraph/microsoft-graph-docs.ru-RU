---
title: Обновление groupPolicyDefinitionFile
description: Обновление свойства объекта groupPolicyDefinitionFile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be713dba2d503f19cd565fe5e53d252ed20667e0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430791"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="bf1bf-103">Обновление groupPolicyDefinitionFile</span><span class="sxs-lookup"><span data-stu-id="bf1bf-103">Update groupPolicyDefinitionFile</span></span>

> <span data-ttu-id="bf1bf-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bf1bf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf1bf-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf1bf-107">Обновление свойства объекта [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="bf1bf-107">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf1bf-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="bf1bf-108">Prerequisites</span></span>
<span data-ttu-id="bf1bf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bf1bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bf1bf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf1bf-111">Permission type</span></span>|<span data-ttu-id="bf1bf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf1bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf1bf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf1bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf1bf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf1bf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bf1bf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf1bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf1bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-116">Not supported.</span></span>|
|<span data-ttu-id="bf1bf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf1bf-117">Application</span></span>|<span data-ttu-id="bf1bf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf1bf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf1bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="bf1bf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf1bf-120">Request headers</span></span>
|<span data-ttu-id="bf1bf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf1bf-121">Header</span></span>|<span data-ttu-id="bf1bf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bf1bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf1bf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf1bf-123">Authorization</span></span>|<span data-ttu-id="bf1bf-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bf1bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf1bf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bf1bf-125">Accept</span></span>|<span data-ttu-id="bf1bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bf1bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf1bf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf1bf-127">Request body</span></span>
<span data-ttu-id="bf1bf-128">В тексте запроса укажите представление JSON для объекта [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="bf1bf-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="bf1bf-129">В следующей таблице показаны свойства, которые необходимы для создания [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span><span class="sxs-lookup"><span data-stu-id="bf1bf-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="bf1bf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf1bf-130">Property</span></span>|<span data-ttu-id="bf1bf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bf1bf-131">Type</span></span>|<span data-ttu-id="bf1bf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bf1bf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf1bf-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bf1bf-133">displayName</span></span>|<span data-ttu-id="bf1bf-134">String</span><span class="sxs-lookup"><span data-stu-id="bf1bf-134">String</span></span>|<span data-ttu-id="bf1bf-135">Локализованные понятное имя файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-135">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="bf1bf-136">description</span><span class="sxs-lookup"><span data-stu-id="bf1bf-136">description</span></span>|<span data-ttu-id="bf1bf-137">String</span><span class="sxs-lookup"><span data-stu-id="bf1bf-137">String</span></span>|<span data-ttu-id="bf1bf-138">Локализованное описание параметров политики в ADMX-файле.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-138">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="bf1bf-139">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-139">The default value is empty.</span></span>|
|<span data-ttu-id="bf1bf-140">languageCodes</span><span class="sxs-lookup"><span data-stu-id="bf1bf-140">languageCodes</span></span>|<span data-ttu-id="bf1bf-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bf1bf-141">String collection</span></span>|<span data-ttu-id="bf1bf-142">Коды поддерживаемых языков для файлов ADMX.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-142">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="bf1bf-143">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="bf1bf-143">targetPrefix</span></span>|<span data-ttu-id="bf1bf-144">String</span><span class="sxs-lookup"><span data-stu-id="bf1bf-144">String</span></span>|<span data-ttu-id="bf1bf-145">Задает логическое имя, которое относится к области имен файлах.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-145">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="bf1bf-146">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="bf1bf-146">targetNamespace</span></span>|<span data-ttu-id="bf1bf-147">String</span><span class="sxs-lookup"><span data-stu-id="bf1bf-147">String</span></span>|<span data-ttu-id="bf1bf-148">Указывает URI, используемый для идентификации пространства имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-148">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="bf1bf-149">policyType</span><span class="sxs-lookup"><span data-stu-id="bf1bf-149">policyType</span></span>|[<span data-ttu-id="bf1bf-150">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="bf1bf-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="bf1bf-151">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-151">Specifies the type of group policy.</span></span> <span data-ttu-id="bf1bf-152">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="bf1bf-153">id</span><span class="sxs-lookup"><span data-stu-id="bf1bf-153">id</span></span>|<span data-ttu-id="bf1bf-154">String</span><span class="sxs-lookup"><span data-stu-id="bf1bf-154">String</span></span>|<span data-ttu-id="bf1bf-155">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-155">Key of the entity.</span></span>|
|<span data-ttu-id="bf1bf-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf1bf-156">lastModifiedDateTime</span></span>|<span data-ttu-id="bf1bf-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf1bf-157">DateTimeOffset</span></span>|<span data-ttu-id="bf1bf-158">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-158">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="bf1bf-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf1bf-159">Response</span></span>
<span data-ttu-id="bf1bf-160">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-160">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf1bf-161">Пример</span><span class="sxs-lookup"><span data-stu-id="bf1bf-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf1bf-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf1bf-162">Request</span></span>
<span data-ttu-id="bf1bf-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested"
}
```

### <a name="response"></a><span data-ttu-id="bf1bf-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf1bf-164">Response</span></span>
<span data-ttu-id="bf1bf-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bf1bf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 438

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "id": "940aa2a1-a2a1-940a-a1a2-0a94a1a20a94",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




