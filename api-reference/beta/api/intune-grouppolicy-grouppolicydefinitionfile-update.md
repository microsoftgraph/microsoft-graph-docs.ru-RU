---
title: Обновление Граупполицидефинитионфиле
description: Обновление свойств объекта Граупполицидефинитионфиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e25862f0005a4ec87dfae46ace5eddfde7f5dd93
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465060"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="d98fd-103">Обновление Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="d98fd-103">Update groupPolicyDefinitionFile</span></span>

<span data-ttu-id="d98fd-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d98fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d98fd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d98fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d98fd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d98fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d98fd-107">Обновление свойств объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="d98fd-107">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d98fd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d98fd-108">Prerequisites</span></span>
<span data-ttu-id="d98fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d98fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d98fd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d98fd-111">Permission type</span></span>|<span data-ttu-id="d98fd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d98fd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d98fd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d98fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d98fd-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d98fd-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d98fd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d98fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d98fd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d98fd-116">Not supported.</span></span>|
|<span data-ttu-id="d98fd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d98fd-117">Application</span></span>|<span data-ttu-id="d98fd-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d98fd-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d98fd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d98fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="d98fd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d98fd-120">Request headers</span></span>
|<span data-ttu-id="d98fd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d98fd-121">Header</span></span>|<span data-ttu-id="d98fd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d98fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d98fd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d98fd-123">Authorization</span></span>|<span data-ttu-id="d98fd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d98fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d98fd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d98fd-125">Accept</span></span>|<span data-ttu-id="d98fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d98fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d98fd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d98fd-127">Request body</span></span>
<span data-ttu-id="d98fd-128">В тексте запроса добавьте представление объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d98fd-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="d98fd-129">В следующей таблице приведены свойства, необходимые при создании [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span><span class="sxs-lookup"><span data-stu-id="d98fd-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="d98fd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d98fd-130">Property</span></span>|<span data-ttu-id="d98fd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d98fd-131">Type</span></span>|<span data-ttu-id="d98fd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d98fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d98fd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d98fd-133">displayName</span></span>|<span data-ttu-id="d98fd-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d98fd-134">String</span></span>|<span data-ttu-id="d98fd-135">Локализованное понятное имя файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="d98fd-135">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="d98fd-136">description</span><span class="sxs-lookup"><span data-stu-id="d98fd-136">description</span></span>|<span data-ttu-id="d98fd-137">String</span><span class="sxs-lookup"><span data-stu-id="d98fd-137">String</span></span>|<span data-ttu-id="d98fd-138">Локализованное описание параметров политики в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="d98fd-138">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="d98fd-139">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="d98fd-139">The default value is empty.</span></span>|
|<span data-ttu-id="d98fd-140">лангуажекодес</span><span class="sxs-lookup"><span data-stu-id="d98fd-140">languageCodes</span></span>|<span data-ttu-id="d98fd-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d98fd-141">String collection</span></span>|<span data-ttu-id="d98fd-142">Поддерживаемые коды языков для ADMX.</span><span class="sxs-lookup"><span data-stu-id="d98fd-142">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="d98fd-143">таржетпрефикс</span><span class="sxs-lookup"><span data-stu-id="d98fd-143">targetPrefix</span></span>|<span data-ttu-id="d98fd-144">String</span><span class="sxs-lookup"><span data-stu-id="d98fd-144">String</span></span>|<span data-ttu-id="d98fd-145">Задает логическое имя, которое ссылается на пространство имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="d98fd-145">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="d98fd-146">Атрибут</span><span class="sxs-lookup"><span data-stu-id="d98fd-146">targetNamespace</span></span>|<span data-ttu-id="d98fd-147">String</span><span class="sxs-lookup"><span data-stu-id="d98fd-147">String</span></span>|<span data-ttu-id="d98fd-148">Указывает универсальный код ресурса (URI), используемый для идентификации пространства имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="d98fd-148">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="d98fd-149">полицитипе</span><span class="sxs-lookup"><span data-stu-id="d98fd-149">policyType</span></span>|[<span data-ttu-id="d98fd-150">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="d98fd-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="d98fd-151">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="d98fd-151">Specifies the type of group policy.</span></span> <span data-ttu-id="d98fd-152">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="d98fd-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="d98fd-153">последним</span><span class="sxs-lookup"><span data-stu-id="d98fd-153">revision</span></span>|<span data-ttu-id="d98fd-154">String</span><span class="sxs-lookup"><span data-stu-id="d98fd-154">String</span></span>|<span data-ttu-id="d98fd-155">Версия редакции, связанная с файлом.</span><span class="sxs-lookup"><span data-stu-id="d98fd-155">The revision version associated with the file.</span></span>|
|<span data-ttu-id="d98fd-156">id</span><span class="sxs-lookup"><span data-stu-id="d98fd-156">id</span></span>|<span data-ttu-id="d98fd-157">String</span><span class="sxs-lookup"><span data-stu-id="d98fd-157">String</span></span>|<span data-ttu-id="d98fd-158">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d98fd-158">Key of the entity.</span></span>|
|<span data-ttu-id="d98fd-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d98fd-159">lastModifiedDateTime</span></span>|<span data-ttu-id="d98fd-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d98fd-160">DateTimeOffset</span></span>|<span data-ttu-id="d98fd-161">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d98fd-161">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="d98fd-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="d98fd-162">Response</span></span>
<span data-ttu-id="d98fd-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d98fd-163">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d98fd-164">Пример</span><span class="sxs-lookup"><span data-stu-id="d98fd-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="d98fd-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="d98fd-165">Request</span></span>
<span data-ttu-id="d98fd-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d98fd-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
Content-type: application/json
Content-length: 358

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
  "revision": "Revision value"
}
```

### <a name="response"></a><span data-ttu-id="d98fd-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="d98fd-167">Response</span></span>
<span data-ttu-id="d98fd-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d98fd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

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
  "revision": "Revision value",
  "id": "940aa2a1-a2a1-940a-a1a2-0a94a1a20a94",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





