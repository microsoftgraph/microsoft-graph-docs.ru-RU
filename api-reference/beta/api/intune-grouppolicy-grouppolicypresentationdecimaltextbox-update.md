---
title: Обновление groupPolicyPresentationDecimalTextBox
description: Обновление свойства объекта groupPolicyPresentationDecimalTextBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c4f91abc80fe37fe3f3677afc7d06b547df9bee4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430642"
---
# <a name="update-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="fb3b8-103">Обновление groupPolicyPresentationDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="fb3b8-103">Update groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="fb3b8-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fb3b8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb3b8-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb3b8-107">Обновление свойства объекта [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="fb3b8-107">Update the properties of a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb3b8-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="fb3b8-108">Prerequisites</span></span>
<span data-ttu-id="fb3b8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fb3b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fb3b8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb3b8-111">Permission type</span></span>|<span data-ttu-id="fb3b8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb3b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb3b8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb3b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb3b8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb3b8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fb3b8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb3b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb3b8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-116">Not supported.</span></span>|
|<span data-ttu-id="fb3b8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb3b8-117">Application</span></span>|<span data-ttu-id="fb3b8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb3b8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb3b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="fb3b8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb3b8-120">Request headers</span></span>
|<span data-ttu-id="fb3b8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb3b8-121">Header</span></span>|<span data-ttu-id="fb3b8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fb3b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb3b8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb3b8-123">Authorization</span></span>|<span data-ttu-id="fb3b8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fb3b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb3b8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb3b8-125">Accept</span></span>|<span data-ttu-id="fb3b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb3b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb3b8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb3b8-127">Request body</span></span>
<span data-ttu-id="fb3b8-128">В тексте запроса укажите представление JSON для объекта [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="fb3b8-128">In the request body, supply a JSON representation for the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

<span data-ttu-id="fb3b8-129">В следующей таблице показаны свойства, которые необходимы для создания [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span><span class="sxs-lookup"><span data-stu-id="fb3b8-129">The following table shows the properties that are required when you create the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md).</span></span>

|<span data-ttu-id="fb3b8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb3b8-130">Property</span></span>|<span data-ttu-id="fb3b8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fb3b8-131">Type</span></span>|<span data-ttu-id="fb3b8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fb3b8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb3b8-133">label</span><span class="sxs-lookup"><span data-stu-id="fb3b8-133">label</span></span>|<span data-ttu-id="fb3b8-134">String</span><span class="sxs-lookup"><span data-stu-id="fb3b8-134">String</span></span>|<span data-ttu-id="fb3b8-135">Метка локализованный текст для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="fb3b8-136">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-136">The default value is empty.</span></span> <span data-ttu-id="fb3b8-137">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="fb3b8-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="fb3b8-138">id</span><span class="sxs-lookup"><span data-stu-id="fb3b8-138">id</span></span>|<span data-ttu-id="fb3b8-139">String</span><span class="sxs-lookup"><span data-stu-id="fb3b8-139">String</span></span>|<span data-ttu-id="fb3b8-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-140">Key of the entity.</span></span> <span data-ttu-id="fb3b8-141">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="fb3b8-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="fb3b8-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb3b8-142">lastModifiedDateTime</span></span>|<span data-ttu-id="fb3b8-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb3b8-143">DateTimeOffset</span></span>|<span data-ttu-id="fb3b8-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="fb3b8-145">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="fb3b8-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="fb3b8-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="fb3b8-146">defaultValue</span></span>|<span data-ttu-id="fb3b8-147">Int64</span><span class="sxs-lookup"><span data-stu-id="fb3b8-147">Int64</span></span>|<span data-ttu-id="fb3b8-148">Целое число без знака, задающее начальное значение для целой и дробной текстовое поле.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="fb3b8-149">Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-149">The default value is 1.</span></span>|
|<span data-ttu-id="fb3b8-150">Счетчик</span><span class="sxs-lookup"><span data-stu-id="fb3b8-150">spin</span></span>|<span data-ttu-id="fb3b8-151">Логический</span><span class="sxs-lookup"><span data-stu-id="fb3b8-151">Boolean</span></span>|<span data-ttu-id="fb3b8-152">Если значение true, создание элемента управления "Счетчик"; в противном случае следует создайте текстовое поле для числовых записей.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="fb3b8-153">Значение по умолчанию — true.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-153">The default value is true.</span></span>|
|<span data-ttu-id="fb3b8-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="fb3b8-154">spinStep</span></span>|<span data-ttu-id="fb3b8-155">Int64</span><span class="sxs-lookup"><span data-stu-id="fb3b8-155">Int64</span></span>|<span data-ttu-id="fb3b8-156">Целое число без знака, задающее шаг изменений элементов.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="fb3b8-157">Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-157">The default value is 1.</span></span>|
|<span data-ttu-id="fb3b8-158">Обязательный</span><span class="sxs-lookup"><span data-stu-id="fb3b8-158">required</span></span>|<span data-ttu-id="fb3b8-159">Логический</span><span class="sxs-lookup"><span data-stu-id="fb3b8-159">Boolean</span></span>|<span data-ttu-id="fb3b8-160">Требование ввести значение в поле параметра.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="fb3b8-161">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-161">The default value is false.</span></span>|
|<span data-ttu-id="fb3b8-162">minValue</span><span class="sxs-lookup"><span data-stu-id="fb3b8-162">minValue</span></span>|<span data-ttu-id="fb3b8-163">Int64</span><span class="sxs-lookup"><span data-stu-id="fb3b8-163">Int64</span></span>|<span data-ttu-id="fb3b8-164">Целое число без знака, задающее минимальное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-164">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="fb3b8-165">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-165">The default value is 0.</span></span>|
|<span data-ttu-id="fb3b8-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="fb3b8-166">maxValue</span></span>|<span data-ttu-id="fb3b8-167">Int64</span><span class="sxs-lookup"><span data-stu-id="fb3b8-167">Int64</span></span>|<span data-ttu-id="fb3b8-168">Целое число без знака, задающее максимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-168">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="fb3b8-169">Значение по умолчанию — 9999.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="fb3b8-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb3b8-170">Response</span></span>
<span data-ttu-id="fb3b8-171">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-171">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb3b8-172">Пример</span><span class="sxs-lookup"><span data-stu-id="fb3b8-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb3b8-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb3b8-173">Request</span></span>
<span data-ttu-id="fb3b8-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
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

### <a name="response"></a><span data-ttu-id="fb3b8-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb3b8-175">Response</span></span>
<span data-ttu-id="fb3b8-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fb3b8-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




