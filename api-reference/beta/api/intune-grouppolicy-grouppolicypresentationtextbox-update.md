---
title: Обновление Граупполиципресентатионтекстбокс
description: Обновление свойств объекта Граупполиципресентатионтекстбокс.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca072271258c2c7512ba8270bcc590975812b815
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962024"
---
# <a name="update-grouppolicypresentationtextbox"></a><span data-ttu-id="bd572-103">Обновление Граупполиципресентатионтекстбокс</span><span class="sxs-lookup"><span data-stu-id="bd572-103">Update groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="bd572-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd572-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd572-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd572-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd572-106">Обновление свойств объекта [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="bd572-106">Update the properties of a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd572-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bd572-107">Prerequisites</span></span>
<span data-ttu-id="bd572-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd572-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd572-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd572-110">Permission type</span></span>|<span data-ttu-id="bd572-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd572-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd572-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd572-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bd572-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd572-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bd572-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd572-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd572-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd572-115">Not supported.</span></span>|
|<span data-ttu-id="bd572-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd572-116">Application</span></span>|<span data-ttu-id="bd572-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd572-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd572-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd572-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="bd572-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd572-119">Request headers</span></span>
|<span data-ttu-id="bd572-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd572-120">Header</span></span>|<span data-ttu-id="bd572-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bd572-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd572-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd572-122">Authorization</span></span>|<span data-ttu-id="bd572-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd572-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd572-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bd572-124">Accept</span></span>|<span data-ttu-id="bd572-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bd572-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd572-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd572-126">Request body</span></span>
<span data-ttu-id="bd572-127">В тексте запроса добавьте представление объекта [Граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd572-127">In the request body, supply a JSON representation for the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

<span data-ttu-id="bd572-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span><span class="sxs-lookup"><span data-stu-id="bd572-128">The following table shows the properties that are required when you create the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span></span>

|<span data-ttu-id="bd572-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd572-129">Property</span></span>|<span data-ttu-id="bd572-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bd572-130">Type</span></span>|<span data-ttu-id="bd572-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bd572-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd572-132">label</span><span class="sxs-lookup"><span data-stu-id="bd572-132">label</span></span>|<span data-ttu-id="bd572-133">String</span><span class="sxs-lookup"><span data-stu-id="bd572-133">String</span></span>|<span data-ttu-id="bd572-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="bd572-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="bd572-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="bd572-135">The default value is empty.</span></span> <span data-ttu-id="bd572-136">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="bd572-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="bd572-137">id</span><span class="sxs-lookup"><span data-stu-id="bd572-137">id</span></span>|<span data-ttu-id="bd572-138">String</span><span class="sxs-lookup"><span data-stu-id="bd572-138">String</span></span>|<span data-ttu-id="bd572-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bd572-139">Key of the entity.</span></span> <span data-ttu-id="bd572-140">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="bd572-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="bd572-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd572-141">lastModifiedDateTime</span></span>|<span data-ttu-id="bd572-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd572-142">DateTimeOffset</span></span>|<span data-ttu-id="bd572-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bd572-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="bd572-144">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="bd572-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="bd572-145">Значение</span><span class="sxs-lookup"><span data-stu-id="bd572-145">defaultValue</span></span>|<span data-ttu-id="bd572-146">String</span><span class="sxs-lookup"><span data-stu-id="bd572-146">String</span></span>|<span data-ttu-id="bd572-147">Локализованная строка по умолчанию, отображаемая в текстовом поле.</span><span class="sxs-lookup"><span data-stu-id="bd572-147">Localized default string displayed in the text box.</span></span> <span data-ttu-id="bd572-148">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="bd572-148">The default value is empty.</span></span>|
|<span data-ttu-id="bd572-149">Обязательный</span><span class="sxs-lookup"><span data-stu-id="bd572-149">required</span></span>|<span data-ttu-id="bd572-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd572-150">Boolean</span></span>|<span data-ttu-id="bd572-151">Требование ввести значение в текстовое поле.</span><span class="sxs-lookup"><span data-stu-id="bd572-151">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="bd572-152">Значение по умолчанию − ложь.</span><span class="sxs-lookup"><span data-stu-id="bd572-152">Default value is false.</span></span>|
|<span data-ttu-id="bd572-153">maxLength</span><span class="sxs-lookup"><span data-stu-id="bd572-153">maxLength</span></span>|<span data-ttu-id="bd572-154">Int64</span><span class="sxs-lookup"><span data-stu-id="bd572-154">Int64</span></span>|<span data-ttu-id="bd572-155">Целое число без знака, задающее максимальное количество текстовых символов.</span><span class="sxs-lookup"><span data-stu-id="bd572-155">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="bd572-156">Значение по умолчанию — 1023.</span><span class="sxs-lookup"><span data-stu-id="bd572-156">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="bd572-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd572-157">Response</span></span>
<span data-ttu-id="bd572-158">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd572-158">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd572-159">Пример</span><span class="sxs-lookup"><span data-stu-id="bd572-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd572-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd572-160">Request</span></span>
<span data-ttu-id="bd572-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd572-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="bd572-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd572-162">Response</span></span>
<span data-ttu-id="bd572-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd572-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 294

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```




