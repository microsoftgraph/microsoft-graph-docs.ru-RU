---
title: Создание ГраупполиципресентатиондеЦималтекстбокс
description: Создание нового объекта ГраупполиципресентатиондеЦималтекстбокс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9231a4387badafe48cde53fc5ec087222aa19c0b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078719"
---
# <a name="create-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="346a8-103">Создание ГраупполиципресентатиондеЦималтекстбокс</span><span class="sxs-lookup"><span data-stu-id="346a8-103">Create groupPolicyPresentationDecimalTextBox</span></span>

<span data-ttu-id="346a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="346a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="346a8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="346a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="346a8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="346a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="346a8-107">Создание нового объекта [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="346a8-107">Create a new [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="346a8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="346a8-108">Prerequisites</span></span>
<span data-ttu-id="346a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="346a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="346a8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="346a8-111">Permission type</span></span>|<span data-ttu-id="346a8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="346a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="346a8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="346a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="346a8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="346a8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="346a8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="346a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="346a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="346a8-116">Not supported.</span></span>|
|<span data-ttu-id="346a8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="346a8-117">Application</span></span>|<span data-ttu-id="346a8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="346a8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="346a8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="346a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="346a8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="346a8-120">Request headers</span></span>
|<span data-ttu-id="346a8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="346a8-121">Header</span></span>|<span data-ttu-id="346a8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="346a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="346a8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="346a8-123">Authorization</span></span>|<span data-ttu-id="346a8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="346a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="346a8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="346a8-125">Accept</span></span>|<span data-ttu-id="346a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="346a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="346a8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="346a8-127">Request body</span></span>
<span data-ttu-id="346a8-128">В тексте запроса добавьте представление объекта ГраупполиципресентатиондеЦималтекстбокс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="346a8-128">In the request body, supply a JSON representation for the groupPolicyPresentationDecimalTextBox object.</span></span>

<span data-ttu-id="346a8-129">В следующей таблице приведены свойства, необходимые при создании ГраупполиципресентатиондеЦималтекстбокс.</span><span class="sxs-lookup"><span data-stu-id="346a8-129">The following table shows the properties that are required when you create the groupPolicyPresentationDecimalTextBox.</span></span>

|<span data-ttu-id="346a8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="346a8-130">Property</span></span>|<span data-ttu-id="346a8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="346a8-131">Type</span></span>|<span data-ttu-id="346a8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="346a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="346a8-133">label</span><span class="sxs-lookup"><span data-stu-id="346a8-133">label</span></span>|<span data-ttu-id="346a8-134">String</span><span class="sxs-lookup"><span data-stu-id="346a8-134">String</span></span>|<span data-ttu-id="346a8-135">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="346a8-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="346a8-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="346a8-136">The default value is empty.</span></span> <span data-ttu-id="346a8-137">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="346a8-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="346a8-138">id</span><span class="sxs-lookup"><span data-stu-id="346a8-138">id</span></span>|<span data-ttu-id="346a8-139">String</span><span class="sxs-lookup"><span data-stu-id="346a8-139">String</span></span>|<span data-ttu-id="346a8-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="346a8-140">Key of the entity.</span></span> <span data-ttu-id="346a8-141">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="346a8-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="346a8-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="346a8-142">lastModifiedDateTime</span></span>|<span data-ttu-id="346a8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="346a8-143">DateTimeOffset</span></span>|<span data-ttu-id="346a8-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="346a8-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="346a8-145">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="346a8-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="346a8-146">Значение</span><span class="sxs-lookup"><span data-stu-id="346a8-146">defaultValue</span></span>|<span data-ttu-id="346a8-147">Int64</span><span class="sxs-lookup"><span data-stu-id="346a8-147">Int64</span></span>|<span data-ttu-id="346a8-148">Целое число без знака, задающее начальное значение для десятичного текстового поля.</span><span class="sxs-lookup"><span data-stu-id="346a8-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="346a8-149">Значение по умолчанию равно 1.</span><span class="sxs-lookup"><span data-stu-id="346a8-149">The default value is 1.</span></span>|
|<span data-ttu-id="346a8-150">повернуть</span><span class="sxs-lookup"><span data-stu-id="346a8-150">spin</span></span>|<span data-ttu-id="346a8-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="346a8-151">Boolean</span></span>|<span data-ttu-id="346a8-152">Если значение — true, создайте элемент управления "Счетчик"; в противном случае создайте текстовое поле для числового элемента.</span><span class="sxs-lookup"><span data-stu-id="346a8-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="346a8-153">Значение по умолчанию: true.</span><span class="sxs-lookup"><span data-stu-id="346a8-153">The default value is true.</span></span>|
|<span data-ttu-id="346a8-154">спинстеп</span><span class="sxs-lookup"><span data-stu-id="346a8-154">spinStep</span></span>|<span data-ttu-id="346a8-155">Int64</span><span class="sxs-lookup"><span data-stu-id="346a8-155">Int64</span></span>|<span data-ttu-id="346a8-156">Целое число без знака, которое указывает приращение изменения элемента управления "Счетчик".</span><span class="sxs-lookup"><span data-stu-id="346a8-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="346a8-157">Значение по умолчанию равно 1.</span><span class="sxs-lookup"><span data-stu-id="346a8-157">The default value is 1.</span></span>|
|<span data-ttu-id="346a8-158">Обязательный</span><span class="sxs-lookup"><span data-stu-id="346a8-158">required</span></span>|<span data-ttu-id="346a8-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="346a8-159">Boolean</span></span>|<span data-ttu-id="346a8-160">Требование ввести значение в поле параметр.</span><span class="sxs-lookup"><span data-stu-id="346a8-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="346a8-161">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="346a8-161">The default value is false.</span></span>|
|<span data-ttu-id="346a8-162">minValue</span><span class="sxs-lookup"><span data-stu-id="346a8-162">minValue</span></span>|<span data-ttu-id="346a8-163">Int64</span><span class="sxs-lookup"><span data-stu-id="346a8-163">Int64</span></span>|<span data-ttu-id="346a8-164">Целое число без знака, задающее минимальное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="346a8-164">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="346a8-165">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="346a8-165">The default value is 0.</span></span>|
|<span data-ttu-id="346a8-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="346a8-166">maxValue</span></span>|<span data-ttu-id="346a8-167">Int64</span><span class="sxs-lookup"><span data-stu-id="346a8-167">Int64</span></span>|<span data-ttu-id="346a8-168">Целое число без знака, задающее максимальное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="346a8-168">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="346a8-169">Значение по умолчанию — 9999.</span><span class="sxs-lookup"><span data-stu-id="346a8-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="346a8-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="346a8-170">Response</span></span>
<span data-ttu-id="346a8-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="346a8-171">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="346a8-172">Пример</span><span class="sxs-lookup"><span data-stu-id="346a8-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="346a8-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="346a8-173">Request</span></span>
<span data-ttu-id="346a8-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="346a8-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 221

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "Label value",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```

### <a name="response"></a><span data-ttu-id="346a8-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="346a8-175">Response</span></span>
<span data-ttu-id="346a8-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="346a8-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 334

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "Label value",
  "id": "988daea7-aea7-988d-a7ae-8d98a7ae8d98",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```






