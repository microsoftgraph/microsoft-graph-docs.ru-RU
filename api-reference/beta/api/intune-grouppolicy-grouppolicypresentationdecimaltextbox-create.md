---
title: Создание ГраупполиципресентатиондеЦималтекстбокс
description: Создание нового объекта ГраупполиципресентатиондеЦималтекстбокс.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c5e051e6a6caea007bea9045dd0398f660dcd920
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969059"
---
# <a name="create-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="aaa5e-103">Создание ГраупполиципресентатиондеЦималтекстбокс</span><span class="sxs-lookup"><span data-stu-id="aaa5e-103">Create groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="aaa5e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aaa5e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaa5e-106">Создание нового объекта [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="aaa5e-106">Create a new [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aaa5e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aaa5e-107">Prerequisites</span></span>
<span data-ttu-id="aaa5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaa5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaa5e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aaa5e-110">Permission type</span></span>|<span data-ttu-id="aaa5e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aaa5e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaa5e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aaa5e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aaa5e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaa5e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="aaa5e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aaa5e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaa5e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-115">Not supported.</span></span>|
|<span data-ttu-id="aaa5e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aaa5e-116">Application</span></span>|<span data-ttu-id="aaa5e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaa5e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aaa5e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="aaa5e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aaa5e-119">Request headers</span></span>
|<span data-ttu-id="aaa5e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aaa5e-120">Header</span></span>|<span data-ttu-id="aaa5e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="aaa5e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaa5e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aaa5e-122">Authorization</span></span>|<span data-ttu-id="aaa5e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaa5e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="aaa5e-124">Accept</span></span>|<span data-ttu-id="aaa5e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aaa5e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaa5e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aaa5e-126">Request body</span></span>
<span data-ttu-id="aaa5e-127">В тексте запроса добавьте представление объекта ГраупполиципресентатиондеЦималтекстбокс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-127">In the request body, supply a JSON representation for the groupPolicyPresentationDecimalTextBox object.</span></span>

<span data-ttu-id="aaa5e-128">В следующей таблице приведены свойства, необходимые при создании ГраупполиципресентатиондеЦималтекстбокс.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-128">The following table shows the properties that are required when you create the groupPolicyPresentationDecimalTextBox.</span></span>

|<span data-ttu-id="aaa5e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="aaa5e-129">Property</span></span>|<span data-ttu-id="aaa5e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="aaa5e-130">Type</span></span>|<span data-ttu-id="aaa5e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="aaa5e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaa5e-132">label</span><span class="sxs-lookup"><span data-stu-id="aaa5e-132">label</span></span>|<span data-ttu-id="aaa5e-133">String</span><span class="sxs-lookup"><span data-stu-id="aaa5e-133">String</span></span>|<span data-ttu-id="aaa5e-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="aaa5e-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-135">The default value is empty.</span></span> <span data-ttu-id="aaa5e-136">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="aaa5e-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="aaa5e-137">id</span><span class="sxs-lookup"><span data-stu-id="aaa5e-137">id</span></span>|<span data-ttu-id="aaa5e-138">String</span><span class="sxs-lookup"><span data-stu-id="aaa5e-138">String</span></span>|<span data-ttu-id="aaa5e-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-139">Key of the entity.</span></span> <span data-ttu-id="aaa5e-140">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="aaa5e-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="aaa5e-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aaa5e-141">lastModifiedDateTime</span></span>|<span data-ttu-id="aaa5e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaa5e-142">DateTimeOffset</span></span>|<span data-ttu-id="aaa5e-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="aaa5e-144">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="aaa5e-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="aaa5e-145">Значение</span><span class="sxs-lookup"><span data-stu-id="aaa5e-145">defaultValue</span></span>|<span data-ttu-id="aaa5e-146">Int64</span><span class="sxs-lookup"><span data-stu-id="aaa5e-146">Int64</span></span>|<span data-ttu-id="aaa5e-147">Целое число без знака, задающее начальное значение для десятичного текстового поля.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-147">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="aaa5e-148">Значение по умолчанию равно 1.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-148">The default value is 1.</span></span>|
|<span data-ttu-id="aaa5e-149">повернуть</span><span class="sxs-lookup"><span data-stu-id="aaa5e-149">spin</span></span>|<span data-ttu-id="aaa5e-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="aaa5e-150">Boolean</span></span>|<span data-ttu-id="aaa5e-151">Если значение — true, создайте элемент управления "Счетчик"; в противном случае создайте текстовое поле для числового элемента.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-151">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="aaa5e-152">Значение по умолчанию: true.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-152">The default value is true.</span></span>|
|<span data-ttu-id="aaa5e-153">Спинстеп</span><span class="sxs-lookup"><span data-stu-id="aaa5e-153">spinStep</span></span>|<span data-ttu-id="aaa5e-154">Int64</span><span class="sxs-lookup"><span data-stu-id="aaa5e-154">Int64</span></span>|<span data-ttu-id="aaa5e-155">Целое число без знака, которое указывает приращение изменения элемента управления "Счетчик".</span><span class="sxs-lookup"><span data-stu-id="aaa5e-155">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="aaa5e-156">Значение по умолчанию равно 1.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-156">The default value is 1.</span></span>|
|<span data-ttu-id="aaa5e-157">Обязательный</span><span class="sxs-lookup"><span data-stu-id="aaa5e-157">required</span></span>|<span data-ttu-id="aaa5e-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="aaa5e-158">Boolean</span></span>|<span data-ttu-id="aaa5e-159">Требование ввести значение в поле параметр.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-159">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="aaa5e-160">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-160">The default value is false.</span></span>|
|<span data-ttu-id="aaa5e-161">minValue</span><span class="sxs-lookup"><span data-stu-id="aaa5e-161">minValue</span></span>|<span data-ttu-id="aaa5e-162">Int64</span><span class="sxs-lookup"><span data-stu-id="aaa5e-162">Int64</span></span>|<span data-ttu-id="aaa5e-163">Целое число без знака, задающее минимальное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-163">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="aaa5e-164">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-164">The default value is 0.</span></span>|
|<span data-ttu-id="aaa5e-165">maxValue</span><span class="sxs-lookup"><span data-stu-id="aaa5e-165">maxValue</span></span>|<span data-ttu-id="aaa5e-166">Int64</span><span class="sxs-lookup"><span data-stu-id="aaa5e-166">Int64</span></span>|<span data-ttu-id="aaa5e-167">Целое число без знака, задающее максимальное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-167">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="aaa5e-168">Значение по умолчанию — 9999.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-168">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="aaa5e-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaa5e-169">Response</span></span>
<span data-ttu-id="aaa5e-170">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-170">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaa5e-171">Пример</span><span class="sxs-lookup"><span data-stu-id="aaa5e-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="aaa5e-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="aaa5e-172">Request</span></span>
<span data-ttu-id="aaa5e-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aaa5e-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaa5e-174">Response</span></span>
<span data-ttu-id="aaa5e-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aaa5e-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




