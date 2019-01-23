---
title: Обновление groupPolicyPresentationLongDecimalTextBox
description: Обновление свойства объекта groupPolicyPresentationLongDecimalTextBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b0b206a557ebd4715aede7e8becbeae672c8bea4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428919"
---
# <a name="update-grouppolicypresentationlongdecimaltextbox"></a><span data-ttu-id="bfe54-103">Обновление groupPolicyPresentationLongDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="bfe54-103">Update groupPolicyPresentationLongDecimalTextBox</span></span>

> <span data-ttu-id="bfe54-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bfe54-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bfe54-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfe54-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bfe54-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bfe54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfe54-107">Обновление свойства объекта [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="bfe54-107">Update the properties of a [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bfe54-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="bfe54-108">Prerequisites</span></span>
<span data-ttu-id="bfe54-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bfe54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bfe54-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfe54-111">Permission type</span></span>|<span data-ttu-id="bfe54-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfe54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfe54-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfe54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bfe54-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfe54-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bfe54-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfe54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfe54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfe54-116">Not supported.</span></span>|
|<span data-ttu-id="bfe54-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bfe54-117">Application</span></span>|<span data-ttu-id="bfe54-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfe54-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfe54-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfe54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="bfe54-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfe54-120">Request headers</span></span>
|<span data-ttu-id="bfe54-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bfe54-121">Header</span></span>|<span data-ttu-id="bfe54-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bfe54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfe54-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bfe54-123">Authorization</span></span>|<span data-ttu-id="bfe54-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bfe54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfe54-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bfe54-125">Accept</span></span>|<span data-ttu-id="bfe54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bfe54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfe54-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bfe54-127">Request body</span></span>
<span data-ttu-id="bfe54-128">В тексте запроса укажите представление JSON для объекта [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="bfe54-128">In the request body, supply a JSON representation for the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object.</span></span>

<span data-ttu-id="bfe54-129">В следующей таблице показаны свойства, которые необходимы для создания [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).</span><span class="sxs-lookup"><span data-stu-id="bfe54-129">The following table shows the properties that are required when you create the [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).</span></span>

|<span data-ttu-id="bfe54-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfe54-130">Property</span></span>|<span data-ttu-id="bfe54-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bfe54-131">Type</span></span>|<span data-ttu-id="bfe54-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bfe54-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfe54-133">label</span><span class="sxs-lookup"><span data-stu-id="bfe54-133">label</span></span>|<span data-ttu-id="bfe54-134">String</span><span class="sxs-lookup"><span data-stu-id="bfe54-134">String</span></span>|<span data-ttu-id="bfe54-135">Метка локализованный текст для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="bfe54-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="bfe54-136">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="bfe54-136">The default value is empty.</span></span> <span data-ttu-id="bfe54-137">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="bfe54-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="bfe54-138">id</span><span class="sxs-lookup"><span data-stu-id="bfe54-138">id</span></span>|<span data-ttu-id="bfe54-139">String</span><span class="sxs-lookup"><span data-stu-id="bfe54-139">String</span></span>|<span data-ttu-id="bfe54-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bfe54-140">Key of the entity.</span></span> <span data-ttu-id="bfe54-141">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="bfe54-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="bfe54-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfe54-142">lastModifiedDateTime</span></span>|<span data-ttu-id="bfe54-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfe54-143">DateTimeOffset</span></span>|<span data-ttu-id="bfe54-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bfe54-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="bfe54-145">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="bfe54-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="bfe54-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="bfe54-146">defaultValue</span></span>|<span data-ttu-id="bfe54-147">Int64</span><span class="sxs-lookup"><span data-stu-id="bfe54-147">Int64</span></span>|<span data-ttu-id="bfe54-148">Целое число без знака, задающее начальное значение для целой и дробной текстовое поле.</span><span class="sxs-lookup"><span data-stu-id="bfe54-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="bfe54-149">Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="bfe54-149">The default value is 1.</span></span>|
|<span data-ttu-id="bfe54-150">Счетчик</span><span class="sxs-lookup"><span data-stu-id="bfe54-150">spin</span></span>|<span data-ttu-id="bfe54-151">Логический</span><span class="sxs-lookup"><span data-stu-id="bfe54-151">Boolean</span></span>|<span data-ttu-id="bfe54-152">Если значение true, создание элемента управления "Счетчик"; в противном случае следует создайте текстовое поле для числовых записей.</span><span class="sxs-lookup"><span data-stu-id="bfe54-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="bfe54-153">Значение по умолчанию — true.</span><span class="sxs-lookup"><span data-stu-id="bfe54-153">The default value is true.</span></span>|
|<span data-ttu-id="bfe54-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="bfe54-154">spinStep</span></span>|<span data-ttu-id="bfe54-155">Int64</span><span class="sxs-lookup"><span data-stu-id="bfe54-155">Int64</span></span>|<span data-ttu-id="bfe54-156">Целое число без знака, задающее шаг изменений элементов.</span><span class="sxs-lookup"><span data-stu-id="bfe54-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="bfe54-157">Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="bfe54-157">The default value is 1.</span></span>|
|<span data-ttu-id="bfe54-158">Обязательный</span><span class="sxs-lookup"><span data-stu-id="bfe54-158">required</span></span>|<span data-ttu-id="bfe54-159">Логический</span><span class="sxs-lookup"><span data-stu-id="bfe54-159">Boolean</span></span>|<span data-ttu-id="bfe54-160">Требование ввести значение в поле параметра.</span><span class="sxs-lookup"><span data-stu-id="bfe54-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="bfe54-161">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="bfe54-161">The default value is false.</span></span>|
|<span data-ttu-id="bfe54-162">minValue</span><span class="sxs-lookup"><span data-stu-id="bfe54-162">minValue</span></span>|<span data-ttu-id="bfe54-163">Int64</span><span class="sxs-lookup"><span data-stu-id="bfe54-163">Int64</span></span>|<span data-ttu-id="bfe54-164">Неподписанный long, задающее минимальное значение.</span><span class="sxs-lookup"><span data-stu-id="bfe54-164">An unsigned long that specifies the minimum allowed value.</span></span> <span data-ttu-id="bfe54-165">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="bfe54-165">The default value is 0.</span></span>|
|<span data-ttu-id="bfe54-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="bfe54-166">maxValue</span></span>|<span data-ttu-id="bfe54-167">Int64</span><span class="sxs-lookup"><span data-stu-id="bfe54-167">Int64</span></span>|<span data-ttu-id="bfe54-168">Неподписанный long, указывающее максимальное значение.</span><span class="sxs-lookup"><span data-stu-id="bfe54-168">An unsigned long that specifies the maximum allowed value.</span></span> <span data-ttu-id="bfe54-169">Значение по умолчанию — 9999.</span><span class="sxs-lookup"><span data-stu-id="bfe54-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="bfe54-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfe54-170">Response</span></span>
<span data-ttu-id="bfe54-171">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bfe54-171">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfe54-172">Пример</span><span class="sxs-lookup"><span data-stu-id="bfe54-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="bfe54-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfe54-173">Request</span></span>
<span data-ttu-id="bfe54-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfe54-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bfe54-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfe54-175">Response</span></span>
<span data-ttu-id="bfe54-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bfe54-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




