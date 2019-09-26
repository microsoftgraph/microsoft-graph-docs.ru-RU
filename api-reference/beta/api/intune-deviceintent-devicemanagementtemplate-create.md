---
title: Создание Девицеманажементтемплате
description: Создание нового объекта Девицеманажементтемплате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 71f43ce3b9d1245c3a55156bae394d8f56acf148
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37189041"
---
# <a name="create-devicemanagementtemplate"></a><span data-ttu-id="1f8cd-103">Создание Девицеманажементтемплате</span><span class="sxs-lookup"><span data-stu-id="1f8cd-103">Create deviceManagementTemplate</span></span>

> <span data-ttu-id="1f8cd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f8cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f8cd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f8cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f8cd-106">Создание нового объекта [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="1f8cd-106">Create a new [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f8cd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1f8cd-107">Prerequisites</span></span>
<span data-ttu-id="1f8cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f8cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f8cd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f8cd-110">Permission type</span></span>|<span data-ttu-id="1f8cd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f8cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f8cd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f8cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f8cd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f8cd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f8cd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f8cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f8cd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f8cd-115">Not supported.</span></span>|
|<span data-ttu-id="1f8cd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f8cd-116">Application</span></span>|<span data-ttu-id="1f8cd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f8cd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f8cd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f8cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="1f8cd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f8cd-119">Request headers</span></span>
|<span data-ttu-id="1f8cd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f8cd-120">Header</span></span>|<span data-ttu-id="1f8cd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1f8cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f8cd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f8cd-122">Authorization</span></span>|<span data-ttu-id="1f8cd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f8cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f8cd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1f8cd-124">Accept</span></span>|<span data-ttu-id="1f8cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f8cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f8cd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1f8cd-126">Request body</span></span>
<span data-ttu-id="1f8cd-127">В тексте запроса добавьте представление объекта Девицеманажементтемплате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f8cd-127">In the request body, supply a JSON representation for the deviceManagementTemplate object.</span></span>

<span data-ttu-id="1f8cd-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементтемплате.</span><span class="sxs-lookup"><span data-stu-id="1f8cd-128">The following table shows the properties that are required when you create the deviceManagementTemplate.</span></span>

|<span data-ttu-id="1f8cd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f8cd-129">Property</span></span>|<span data-ttu-id="1f8cd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1f8cd-130">Type</span></span>|<span data-ttu-id="1f8cd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1f8cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f8cd-132">id</span><span class="sxs-lookup"><span data-stu-id="1f8cd-132">id</span></span>|<span data-ttu-id="1f8cd-133">String</span><span class="sxs-lookup"><span data-stu-id="1f8cd-133">String</span></span>|<span data-ttu-id="1f8cd-134">Идентификатор шаблона</span><span class="sxs-lookup"><span data-stu-id="1f8cd-134">The template ID</span></span>|
|<span data-ttu-id="1f8cd-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1f8cd-135">displayName</span></span>|<span data-ttu-id="1f8cd-136">Строка</span><span class="sxs-lookup"><span data-stu-id="1f8cd-136">String</span></span>|<span data-ttu-id="1f8cd-137">Отображаемое имя шаблона</span><span class="sxs-lookup"><span data-stu-id="1f8cd-137">The template's display name</span></span>|
|<span data-ttu-id="1f8cd-138">description</span><span class="sxs-lookup"><span data-stu-id="1f8cd-138">description</span></span>|<span data-ttu-id="1f8cd-139">String</span><span class="sxs-lookup"><span data-stu-id="1f8cd-139">String</span></span>|<span data-ttu-id="1f8cd-140">Описание шаблона</span><span class="sxs-lookup"><span data-stu-id="1f8cd-140">The template's description</span></span>|
|<span data-ttu-id="1f8cd-141">versionInfo</span><span class="sxs-lookup"><span data-stu-id="1f8cd-141">versionInfo</span></span>|<span data-ttu-id="1f8cd-142">String.</span><span class="sxs-lookup"><span data-stu-id="1f8cd-142">String</span></span>|<span data-ttu-id="1f8cd-143">Сведения о версии шаблона</span><span class="sxs-lookup"><span data-stu-id="1f8cd-143">The template's version information</span></span>|
|<span data-ttu-id="1f8cd-144">нерекомендуемый</span><span class="sxs-lookup"><span data-stu-id="1f8cd-144">isDeprecated</span></span>|<span data-ttu-id="1f8cd-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="1f8cd-145">Boolean</span></span>|<span data-ttu-id="1f8cd-146">Шаблон устарел или не является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="1f8cd-146">The template is deprecated or not.</span></span> <span data-ttu-id="1f8cd-147">Не удается создать объект "удержания" из устаревшего шаблона.</span><span class="sxs-lookup"><span data-stu-id="1f8cd-147">Intents cannot be created from a deprecated template.</span></span>|
|<span data-ttu-id="1f8cd-148">интенткаунт</span><span class="sxs-lookup"><span data-stu-id="1f8cd-148">intentCount</span></span>|<span data-ttu-id="1f8cd-149">Int32</span><span class="sxs-lookup"><span data-stu-id="1f8cd-149">Int32</span></span>|<span data-ttu-id="1f8cd-150">Количество целей, созданных на основе этого шаблона.</span><span class="sxs-lookup"><span data-stu-id="1f8cd-150">Number of Intents created from this template.</span></span>|
|<span data-ttu-id="1f8cd-151">TemplateType — тип</span><span class="sxs-lookup"><span data-stu-id="1f8cd-151">templateType</span></span>|[<span data-ttu-id="1f8cd-152">девицеманажементтемплатетипе</span><span class="sxs-lookup"><span data-stu-id="1f8cd-152">deviceManagementTemplateType</span></span>](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|<span data-ttu-id="1f8cd-153">Тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="1f8cd-153">The template's type.</span></span> <span data-ttu-id="1f8cd-154">Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`.</span><span class="sxs-lookup"><span data-stu-id="1f8cd-154">Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`.</span></span>|
|<span data-ttu-id="1f8cd-155">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f8cd-155">publishedDateTime</span></span>|<span data-ttu-id="1f8cd-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f8cd-156">DateTimeOffset</span></span>|<span data-ttu-id="1f8cd-157">При публикации шаблона</span><span class="sxs-lookup"><span data-stu-id="1f8cd-157">When the template was published</span></span>|



## <a name="response"></a><span data-ttu-id="1f8cd-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f8cd-158">Response</span></span>
<span data-ttu-id="1f8cd-159">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1f8cd-159">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f8cd-160">Пример</span><span class="sxs-lookup"><span data-stu-id="1f8cd-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f8cd-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f8cd-161">Request</span></span>
<span data-ttu-id="1f8cd-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f8cd-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a><span data-ttu-id="1f8cd-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f8cd-163">Response</span></span>
<span data-ttu-id="1f8cd-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f8cd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 383

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```




