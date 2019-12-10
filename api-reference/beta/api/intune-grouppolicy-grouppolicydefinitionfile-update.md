---
title: Обновление Граупполицидефинитионфиле
description: Обновление свойств объекта Граупполицидефинитионфиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10cd3947e0fca3cc243e6f93459cec57f5b47512
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943132"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="6c303-103">Обновление Граупполицидефинитионфиле</span><span class="sxs-lookup"><span data-stu-id="6c303-103">Update groupPolicyDefinitionFile</span></span>

> <span data-ttu-id="6c303-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c303-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c303-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c303-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c303-106">Обновление свойств объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .</span><span class="sxs-lookup"><span data-stu-id="6c303-106">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c303-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6c303-107">Prerequisites</span></span>
<span data-ttu-id="6c303-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c303-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c303-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c303-110">Permission type</span></span>|<span data-ttu-id="6c303-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c303-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c303-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c303-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c303-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c303-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6c303-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c303-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c303-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c303-115">Not supported.</span></span>|
|<span data-ttu-id="6c303-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c303-116">Application</span></span>|<span data-ttu-id="6c303-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c303-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c303-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c303-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="6c303-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6c303-119">Request headers</span></span>
|<span data-ttu-id="6c303-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c303-120">Header</span></span>|<span data-ttu-id="6c303-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6c303-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c303-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c303-122">Authorization</span></span>|<span data-ttu-id="6c303-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c303-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c303-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6c303-124">Accept</span></span>|<span data-ttu-id="6c303-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c303-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c303-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6c303-126">Request body</span></span>
<span data-ttu-id="6c303-127">В тексте запроса добавьте представление объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c303-127">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="6c303-128">В следующей таблице приведены свойства, необходимые при создании [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span><span class="sxs-lookup"><span data-stu-id="6c303-128">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="6c303-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c303-129">Property</span></span>|<span data-ttu-id="6c303-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6c303-130">Type</span></span>|<span data-ttu-id="6c303-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6c303-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c303-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6c303-132">displayName</span></span>|<span data-ttu-id="6c303-133">Строка</span><span class="sxs-lookup"><span data-stu-id="6c303-133">String</span></span>|<span data-ttu-id="6c303-134">Локализованное понятное имя файла ADMX.</span><span class="sxs-lookup"><span data-stu-id="6c303-134">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="6c303-135">description</span><span class="sxs-lookup"><span data-stu-id="6c303-135">description</span></span>|<span data-ttu-id="6c303-136">String</span><span class="sxs-lookup"><span data-stu-id="6c303-136">String</span></span>|<span data-ttu-id="6c303-137">Локализованное описание параметров политики в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="6c303-137">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="6c303-138">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="6c303-138">The default value is empty.</span></span>|
|<span data-ttu-id="6c303-139">лангуажекодес</span><span class="sxs-lookup"><span data-stu-id="6c303-139">languageCodes</span></span>|<span data-ttu-id="6c303-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6c303-140">String collection</span></span>|<span data-ttu-id="6c303-141">Поддерживаемые коды языков для ADMX.</span><span class="sxs-lookup"><span data-stu-id="6c303-141">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="6c303-142">таржетпрефикс</span><span class="sxs-lookup"><span data-stu-id="6c303-142">targetPrefix</span></span>|<span data-ttu-id="6c303-143">Строка</span><span class="sxs-lookup"><span data-stu-id="6c303-143">String</span></span>|<span data-ttu-id="6c303-144">Задает логическое имя, которое ссылается на пространство имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="6c303-144">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="6c303-145">Атрибут</span><span class="sxs-lookup"><span data-stu-id="6c303-145">targetNamespace</span></span>|<span data-ttu-id="6c303-146">Строка</span><span class="sxs-lookup"><span data-stu-id="6c303-146">String</span></span>|<span data-ttu-id="6c303-147">Указывает универсальный код ресурса (URI), используемый для идентификации пространства имен в файле ADMX.</span><span class="sxs-lookup"><span data-stu-id="6c303-147">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="6c303-148">полицитипе</span><span class="sxs-lookup"><span data-stu-id="6c303-148">policyType</span></span>|[<span data-ttu-id="6c303-149">граупполицитипе</span><span class="sxs-lookup"><span data-stu-id="6c303-149">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="6c303-150">Указывает тип групповой политики.</span><span class="sxs-lookup"><span data-stu-id="6c303-150">Specifies the type of group policy.</span></span> <span data-ttu-id="6c303-151">Возможные значения: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="6c303-151">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="6c303-152">последним</span><span class="sxs-lookup"><span data-stu-id="6c303-152">revision</span></span>|<span data-ttu-id="6c303-153">Строка</span><span class="sxs-lookup"><span data-stu-id="6c303-153">String</span></span>|<span data-ttu-id="6c303-154">Версия редакции, связанная с файлом.</span><span class="sxs-lookup"><span data-stu-id="6c303-154">The revision version associated with the file.</span></span>|
|<span data-ttu-id="6c303-155">id</span><span class="sxs-lookup"><span data-stu-id="6c303-155">id</span></span>|<span data-ttu-id="6c303-156">String</span><span class="sxs-lookup"><span data-stu-id="6c303-156">String</span></span>|<span data-ttu-id="6c303-157">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6c303-157">Key of the entity.</span></span>|
|<span data-ttu-id="6c303-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c303-158">lastModifiedDateTime</span></span>|<span data-ttu-id="6c303-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c303-159">DateTimeOffset</span></span>|<span data-ttu-id="6c303-160">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6c303-160">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="6c303-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c303-161">Response</span></span>
<span data-ttu-id="6c303-162">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c303-162">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c303-163">Пример</span><span class="sxs-lookup"><span data-stu-id="6c303-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c303-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c303-164">Request</span></span>
<span data-ttu-id="6c303-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c303-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6c303-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c303-166">Response</span></span>
<span data-ttu-id="6c303-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c303-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





