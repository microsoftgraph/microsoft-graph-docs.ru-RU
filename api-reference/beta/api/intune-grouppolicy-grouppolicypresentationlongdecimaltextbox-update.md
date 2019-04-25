---
title: Обновление ГраупполиципресентатионлонгдеЦималтекстбокс
description: Обновление свойств объекта ГраупполиципресентатионлонгдеЦималтекстбокс.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 361236a90b5e65027bf45fac7bff4382c6458daa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32530937"
---
# <a name="update-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="081a4-103">Обновление ГраупполиципресентатионлонгдеЦималтекстбокс</span><span class="sxs-lookup"><span data-stu-id="081a4-103">Update groupPolicyPresentationLongDecimalTextBox</span></span>

> <span data-ttu-id="081a4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="081a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="081a4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="081a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="081a4-106">Обновление свойств объекта [граупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="081a4-106">Update the properties of a [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="081a4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="081a4-107">Prerequisites</span></span>
<span data-ttu-id="081a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="081a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="081a4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="081a4-110">Permission type</span></span>|<span data-ttu-id="081a4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="081a4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="081a4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="081a4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="081a4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="081a4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="081a4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="081a4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="081a4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="081a4-115">Not supported.</span></span>|
|<span data-ttu-id="081a4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="081a4-116">Application</span></span>|<span data-ttu-id="081a4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="081a4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="081a4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="081a4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="081a4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="081a4-119">Request headers</span></span>
|<span data-ttu-id="081a4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="081a4-120">Header</span></span>|<span data-ttu-id="081a4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="081a4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="081a4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="081a4-122">Authorization</span></span>|<span data-ttu-id="081a4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="081a4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="081a4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="081a4-124">Accept</span></span>|<span data-ttu-id="081a4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="081a4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="081a4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="081a4-126">Request body</span></span>
<span data-ttu-id="081a4-127">В тексте запроса добавьте представление объекта [ГраупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="081a4-127">In the request body, supply a JSON representation for the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

<span data-ttu-id="081a4-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).</span><span class="sxs-lookup"><span data-stu-id="081a4-128">The following table shows the properties that are required when you create the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).</span></span>

|<span data-ttu-id="081a4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="081a4-129">Property</span></span>|<span data-ttu-id="081a4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="081a4-130">Type</span></span>|<span data-ttu-id="081a4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="081a4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="081a4-132">label</span><span class="sxs-lookup"><span data-stu-id="081a4-132">label</span></span>|<span data-ttu-id="081a4-133">String</span><span class="sxs-lookup"><span data-stu-id="081a4-133">String</span></span>|<span data-ttu-id="081a4-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="081a4-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="081a4-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="081a4-135">The default value is empty.</span></span> <span data-ttu-id="081a4-136">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="081a4-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="081a4-137">id</span><span class="sxs-lookup"><span data-stu-id="081a4-137">id</span></span>|<span data-ttu-id="081a4-138">String</span><span class="sxs-lookup"><span data-stu-id="081a4-138">String</span></span>|<span data-ttu-id="081a4-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="081a4-139">Key of the entity.</span></span> <span data-ttu-id="081a4-140">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="081a4-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="081a4-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="081a4-141">lastModifiedDateTime</span></span>|<span data-ttu-id="081a4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="081a4-142">DateTimeOffset</span></span>|<span data-ttu-id="081a4-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="081a4-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="081a4-144">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="081a4-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="081a4-145">Значение</span><span class="sxs-lookup"><span data-stu-id="081a4-145">defaultValue</span></span>|<span data-ttu-id="081a4-146">Int64</span><span class="sxs-lookup"><span data-stu-id="081a4-146">Int64</span></span>|<span data-ttu-id="081a4-147">Целое число без знака, задающее начальное значение для десятичного текстового поля.</span><span class="sxs-lookup"><span data-stu-id="081a4-147">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="081a4-148">Значение по умолчанию равно 1.</span><span class="sxs-lookup"><span data-stu-id="081a4-148">The default value is 1.</span></span>|
|<span data-ttu-id="081a4-149">повернуть</span><span class="sxs-lookup"><span data-stu-id="081a4-149">spin</span></span>|<span data-ttu-id="081a4-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="081a4-150">Boolean</span></span>|<span data-ttu-id="081a4-151">Если значение — true, создайте элемент управления "Счетчик"; в противном случае создайте текстовое поле для числового элемента.</span><span class="sxs-lookup"><span data-stu-id="081a4-151">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="081a4-152">Значение по умолчанию: true.</span><span class="sxs-lookup"><span data-stu-id="081a4-152">The default value is true.</span></span>|
|<span data-ttu-id="081a4-153">Спинстеп</span><span class="sxs-lookup"><span data-stu-id="081a4-153">spinStep</span></span>|<span data-ttu-id="081a4-154">Int64</span><span class="sxs-lookup"><span data-stu-id="081a4-154">Int64</span></span>|<span data-ttu-id="081a4-155">Целое число без знака, которое указывает приращение изменения элемента управления "Счетчик".</span><span class="sxs-lookup"><span data-stu-id="081a4-155">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="081a4-156">Значение по умолчанию равно 1.</span><span class="sxs-lookup"><span data-stu-id="081a4-156">The default value is 1.</span></span>|
|<span data-ttu-id="081a4-157">Обязательный</span><span class="sxs-lookup"><span data-stu-id="081a4-157">required</span></span>|<span data-ttu-id="081a4-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="081a4-158">Boolean</span></span>|<span data-ttu-id="081a4-159">Требование ввести значение в поле параметр.</span><span class="sxs-lookup"><span data-stu-id="081a4-159">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="081a4-160">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="081a4-160">The default value is false.</span></span>|
|<span data-ttu-id="081a4-161">minValue</span><span class="sxs-lookup"><span data-stu-id="081a4-161">minValue</span></span>|<span data-ttu-id="081a4-162">Int64</span><span class="sxs-lookup"><span data-stu-id="081a4-162">Int64</span></span>|<span data-ttu-id="081a4-163">Длинное целое число без знака, задающее минимальное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="081a4-163">An unsigned long that specifies the minimum allowed value.</span></span> <span data-ttu-id="081a4-164">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="081a4-164">The default value is 0.</span></span>|
|<span data-ttu-id="081a4-165">maxValue</span><span class="sxs-lookup"><span data-stu-id="081a4-165">maxValue</span></span>|<span data-ttu-id="081a4-166">Int64</span><span class="sxs-lookup"><span data-stu-id="081a4-166">Int64</span></span>|<span data-ttu-id="081a4-167">Длинное целое число без знака, задающее максимальное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="081a4-167">An unsigned long that specifies the maximum allowed value.</span></span> <span data-ttu-id="081a4-168">Значение по умолчанию — 9999.</span><span class="sxs-lookup"><span data-stu-id="081a4-168">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="081a4-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="081a4-169">Response</span></span>
<span data-ttu-id="081a4-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="081a4-170">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="081a4-171">Пример</span><span class="sxs-lookup"><span data-stu-id="081a4-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="081a4-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="081a4-172">Request</span></span>
<span data-ttu-id="081a4-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="081a4-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 225

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "Label value",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```

### <a name="response"></a><span data-ttu-id="081a4-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="081a4-174">Response</span></span>
<span data-ttu-id="081a4-p111">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="081a4-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 338

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "Label value",
  "id": "754d8495-8495-754d-9584-4d7595844d75",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```





