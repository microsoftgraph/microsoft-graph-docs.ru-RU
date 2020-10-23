---
title: Создание ГраупполиципресентатионлонгдеЦималтекстбокс
description: Создание нового объекта ГраупполиципресентатионлонгдеЦималтекстбокс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f96507c8d354acda092e910b5f496f979a4c265
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730947"
---
# <a name="create-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="9d36c-103">Создание ГраупполиципресентатионлонгдеЦималтекстбокс</span><span class="sxs-lookup"><span data-stu-id="9d36c-103">Create groupPolicyPresentationLongDecimalTextBox</span></span>

<span data-ttu-id="9d36c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d36c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d36c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d36c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d36c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d36c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d36c-107">Создание нового объекта [граупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="9d36c-107">Create a new [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d36c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9d36c-108">Prerequisites</span></span>
<span data-ttu-id="9d36c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d36c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d36c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d36c-111">Permission type</span></span>|<span data-ttu-id="9d36c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d36c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d36c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d36c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d36c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d36c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9d36c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d36c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d36c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d36c-116">Not supported.</span></span>|
|<span data-ttu-id="9d36c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d36c-117">Application</span></span>|<span data-ttu-id="9d36c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d36c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d36c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d36c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="9d36c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9d36c-120">Request headers</span></span>
|<span data-ttu-id="9d36c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d36c-121">Header</span></span>|<span data-ttu-id="9d36c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9d36c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d36c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d36c-123">Authorization</span></span>|<span data-ttu-id="9d36c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d36c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d36c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9d36c-125">Accept</span></span>|<span data-ttu-id="9d36c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d36c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d36c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9d36c-127">Request body</span></span>
<span data-ttu-id="9d36c-128">В тексте запроса добавьте представление объекта ГраупполиципресентатионлонгдеЦималтекстбокс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d36c-128">In the request body, supply a JSON representation for the groupPolicyPresentationLongDecimalTextBox object.</span></span>

<span data-ttu-id="9d36c-129">В следующей таблице приведены свойства, необходимые при создании ГраупполиципресентатионлонгдеЦималтекстбокс.</span><span class="sxs-lookup"><span data-stu-id="9d36c-129">The following table shows the properties that are required when you create the groupPolicyPresentationLongDecimalTextBox.</span></span>

|<span data-ttu-id="9d36c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d36c-130">Property</span></span>|<span data-ttu-id="9d36c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9d36c-131">Type</span></span>|<span data-ttu-id="9d36c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9d36c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d36c-133">label</span><span class="sxs-lookup"><span data-stu-id="9d36c-133">label</span></span>|<span data-ttu-id="9d36c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9d36c-134">String</span></span>|<span data-ttu-id="9d36c-135">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="9d36c-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="9d36c-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="9d36c-136">The default value is empty.</span></span> <span data-ttu-id="9d36c-137">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9d36c-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9d36c-138">id</span><span class="sxs-lookup"><span data-stu-id="9d36c-138">id</span></span>|<span data-ttu-id="9d36c-139">Строка</span><span class="sxs-lookup"><span data-stu-id="9d36c-139">String</span></span>|<span data-ttu-id="9d36c-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9d36c-140">Key of the entity.</span></span> <span data-ttu-id="9d36c-141">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9d36c-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9d36c-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d36c-142">lastModifiedDateTime</span></span>|<span data-ttu-id="9d36c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d36c-143">DateTimeOffset</span></span>|<span data-ttu-id="9d36c-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9d36c-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="9d36c-145">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9d36c-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9d36c-146">Значение</span><span class="sxs-lookup"><span data-stu-id="9d36c-146">defaultValue</span></span>|<span data-ttu-id="9d36c-147">Int64</span><span class="sxs-lookup"><span data-stu-id="9d36c-147">Int64</span></span>|<span data-ttu-id="9d36c-148">Целое число без знака, задающее начальное значение для десятичного текстового поля.</span><span class="sxs-lookup"><span data-stu-id="9d36c-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="9d36c-149">Значение по умолчанию равно 1.</span><span class="sxs-lookup"><span data-stu-id="9d36c-149">The default value is 1.</span></span>|
|<span data-ttu-id="9d36c-150">повернуть</span><span class="sxs-lookup"><span data-stu-id="9d36c-150">spin</span></span>|<span data-ttu-id="9d36c-151">Логический</span><span class="sxs-lookup"><span data-stu-id="9d36c-151">Boolean</span></span>|<span data-ttu-id="9d36c-152">Если значение — true, создайте элемент управления "Счетчик"; в противном случае создайте текстовое поле для числового элемента.</span><span class="sxs-lookup"><span data-stu-id="9d36c-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="9d36c-153">Значение по умолчанию: true.</span><span class="sxs-lookup"><span data-stu-id="9d36c-153">The default value is true.</span></span>|
|<span data-ttu-id="9d36c-154">спинстеп</span><span class="sxs-lookup"><span data-stu-id="9d36c-154">spinStep</span></span>|<span data-ttu-id="9d36c-155">Int64</span><span class="sxs-lookup"><span data-stu-id="9d36c-155">Int64</span></span>|<span data-ttu-id="9d36c-156">Целое число без знака, которое указывает приращение изменения элемента управления "Счетчик".</span><span class="sxs-lookup"><span data-stu-id="9d36c-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="9d36c-157">Значение по умолчанию равно 1.</span><span class="sxs-lookup"><span data-stu-id="9d36c-157">The default value is 1.</span></span>|
|<span data-ttu-id="9d36c-158">Обязательный</span><span class="sxs-lookup"><span data-stu-id="9d36c-158">required</span></span>|<span data-ttu-id="9d36c-159">Логический</span><span class="sxs-lookup"><span data-stu-id="9d36c-159">Boolean</span></span>|<span data-ttu-id="9d36c-160">Требование ввести значение в поле параметр.</span><span class="sxs-lookup"><span data-stu-id="9d36c-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="9d36c-161">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="9d36c-161">The default value is false.</span></span>|
|<span data-ttu-id="9d36c-162">minValue</span><span class="sxs-lookup"><span data-stu-id="9d36c-162">minValue</span></span>|<span data-ttu-id="9d36c-163">Int64</span><span class="sxs-lookup"><span data-stu-id="9d36c-163">Int64</span></span>|<span data-ttu-id="9d36c-164">Длинное целое число без знака, задающее минимальное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="9d36c-164">An unsigned long that specifies the minimum allowed value.</span></span> <span data-ttu-id="9d36c-165">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="9d36c-165">The default value is 0.</span></span>|
|<span data-ttu-id="9d36c-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="9d36c-166">maxValue</span></span>|<span data-ttu-id="9d36c-167">Int64</span><span class="sxs-lookup"><span data-stu-id="9d36c-167">Int64</span></span>|<span data-ttu-id="9d36c-168">Длинное целое число без знака, задающее максимальное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="9d36c-168">An unsigned long that specifies the maximum allowed value.</span></span> <span data-ttu-id="9d36c-169">Значение по умолчанию — 9999.</span><span class="sxs-lookup"><span data-stu-id="9d36c-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="9d36c-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d36c-170">Response</span></span>
<span data-ttu-id="9d36c-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d36c-171">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d36c-172">Пример</span><span class="sxs-lookup"><span data-stu-id="9d36c-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d36c-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d36c-173">Request</span></span>
<span data-ttu-id="9d36c-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d36c-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
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

### <a name="response"></a><span data-ttu-id="9d36c-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d36c-175">Response</span></span>
<span data-ttu-id="9d36c-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d36c-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





