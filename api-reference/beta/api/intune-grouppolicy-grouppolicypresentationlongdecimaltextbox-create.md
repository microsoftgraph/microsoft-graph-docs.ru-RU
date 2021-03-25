---
title: Создание groupPolicyPresentationLongDecimalTextBox
description: Создайте новый объект groupPolicyPresentationLongDecimalTextBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5de88999c439ef4a7b6ec8d9316dd32cfd54e94d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153309"
---
# <a name="create-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="d546a-103">Создание groupPolicyPresentationLongDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="d546a-103">Create groupPolicyPresentationLongDecimalTextBox</span></span>

<span data-ttu-id="d546a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d546a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d546a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d546a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d546a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d546a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d546a-107">Создайте новый [объект groupPolicyPresentationLongDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)</span><span class="sxs-lookup"><span data-stu-id="d546a-107">Create a new [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d546a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d546a-108">Prerequisites</span></span>
<span data-ttu-id="d546a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d546a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d546a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d546a-111">Permission type</span></span>|<span data-ttu-id="d546a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d546a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d546a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d546a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d546a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d546a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d546a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d546a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d546a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d546a-116">Not supported.</span></span>|
|<span data-ttu-id="d546a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d546a-117">Application</span></span>|<span data-ttu-id="d546a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d546a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d546a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d546a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="d546a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d546a-120">Request headers</span></span>
|<span data-ttu-id="d546a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d546a-121">Header</span></span>|<span data-ttu-id="d546a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d546a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d546a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d546a-123">Authorization</span></span>|<span data-ttu-id="d546a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d546a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d546a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d546a-125">Accept</span></span>|<span data-ttu-id="d546a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d546a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d546a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d546a-127">Request body</span></span>
<span data-ttu-id="d546a-128">В тексте запроса предопределите представление JSON для объекта GroupPolicyPresentationLongDecimalTextBox.</span><span class="sxs-lookup"><span data-stu-id="d546a-128">In the request body, supply a JSON representation for the groupPolicyPresentationLongDecimalTextBox object.</span></span>

<span data-ttu-id="d546a-129">В следующей таблице показаны свойства, необходимые при создании группыPolicyPresentationLongDecimalTextBox.</span><span class="sxs-lookup"><span data-stu-id="d546a-129">The following table shows the properties that are required when you create the groupPolicyPresentationLongDecimalTextBox.</span></span>

|<span data-ttu-id="d546a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d546a-130">Property</span></span>|<span data-ttu-id="d546a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d546a-131">Type</span></span>|<span data-ttu-id="d546a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d546a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d546a-133">label</span><span class="sxs-lookup"><span data-stu-id="d546a-133">label</span></span>|<span data-ttu-id="d546a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d546a-134">String</span></span>|<span data-ttu-id="d546a-135">Локализованная текстовая метка для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="d546a-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="d546a-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="d546a-136">The default value is empty.</span></span> <span data-ttu-id="d546a-137">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d546a-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d546a-138">id</span><span class="sxs-lookup"><span data-stu-id="d546a-138">id</span></span>|<span data-ttu-id="d546a-139">Строка</span><span class="sxs-lookup"><span data-stu-id="d546a-139">String</span></span>|<span data-ttu-id="d546a-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d546a-140">Key of the entity.</span></span> <span data-ttu-id="d546a-141">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d546a-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d546a-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d546a-142">lastModifiedDateTime</span></span>|<span data-ttu-id="d546a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d546a-143">DateTimeOffset</span></span>|<span data-ttu-id="d546a-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d546a-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="d546a-145">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d546a-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d546a-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="d546a-146">defaultValue</span></span>|<span data-ttu-id="d546a-147">Int64</span><span class="sxs-lookup"><span data-stu-id="d546a-147">Int64</span></span>|<span data-ttu-id="d546a-148">Неподписаный полный ящик, который указывает начальное значение десятичной текстовой коробки.</span><span class="sxs-lookup"><span data-stu-id="d546a-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="d546a-149">Значение по умолчанию равно 1.</span><span class="sxs-lookup"><span data-stu-id="d546a-149">The default value is 1.</span></span>|
|<span data-ttu-id="d546a-150">spin</span><span class="sxs-lookup"><span data-stu-id="d546a-150">spin</span></span>|<span data-ttu-id="d546a-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="d546a-151">Boolean</span></span>|<span data-ttu-id="d546a-152">Если верно, создайте управление спином; в противном случае создайте текстовое поле для числовой записи.</span><span class="sxs-lookup"><span data-stu-id="d546a-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="d546a-153">Значение по умолчанию: true.</span><span class="sxs-lookup"><span data-stu-id="d546a-153">The default value is true.</span></span>|
|<span data-ttu-id="d546a-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="d546a-154">spinStep</span></span>|<span data-ttu-id="d546a-155">Int64</span><span class="sxs-lookup"><span data-stu-id="d546a-155">Int64</span></span>|<span data-ttu-id="d546a-156">Неподписавая часть, указывляемая на приращение изменений для управления спином.</span><span class="sxs-lookup"><span data-stu-id="d546a-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="d546a-157">Значение по умолчанию равно 1.</span><span class="sxs-lookup"><span data-stu-id="d546a-157">The default value is 1.</span></span>|
|<span data-ttu-id="d546a-158">Обязательный</span><span class="sxs-lookup"><span data-stu-id="d546a-158">required</span></span>|<span data-ttu-id="d546a-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="d546a-159">Boolean</span></span>|<span data-ttu-id="d546a-160">Требование ввести значение в поле параметра.</span><span class="sxs-lookup"><span data-stu-id="d546a-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="d546a-161">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="d546a-161">The default value is false.</span></span>|
|<span data-ttu-id="d546a-162">minValue</span><span class="sxs-lookup"><span data-stu-id="d546a-162">minValue</span></span>|<span data-ttu-id="d546a-163">Int64</span><span class="sxs-lookup"><span data-stu-id="d546a-163">Int64</span></span>|<span data-ttu-id="d546a-164">Неподписаный длинный, который указывает минимально допустимые значения.</span><span class="sxs-lookup"><span data-stu-id="d546a-164">An unsigned long that specifies the minimum allowed value.</span></span> <span data-ttu-id="d546a-165">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="d546a-165">The default value is 0.</span></span>|
|<span data-ttu-id="d546a-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="d546a-166">maxValue</span></span>|<span data-ttu-id="d546a-167">Int64</span><span class="sxs-lookup"><span data-stu-id="d546a-167">Int64</span></span>|<span data-ttu-id="d546a-168">Неподписаное длинное значение, которое указывает максимально допустимые значения.</span><span class="sxs-lookup"><span data-stu-id="d546a-168">An unsigned long that specifies the maximum allowed value.</span></span> <span data-ttu-id="d546a-169">Значение по умолчанию — 9999.</span><span class="sxs-lookup"><span data-stu-id="d546a-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="d546a-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="d546a-170">Response</span></span>
<span data-ttu-id="d546a-171">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d546a-171">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d546a-172">Пример</span><span class="sxs-lookup"><span data-stu-id="d546a-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="d546a-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="d546a-173">Request</span></span>
<span data-ttu-id="d546a-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d546a-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d546a-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="d546a-175">Response</span></span>
<span data-ttu-id="d546a-p111">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d546a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




