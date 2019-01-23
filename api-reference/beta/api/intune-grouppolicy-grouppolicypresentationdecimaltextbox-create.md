---
title: Создание groupPolicyPresentationDecimalTextBox
description: Создание нового объекта groupPolicyPresentationDecimalTextBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1cc6e5cb8104cc4d9ff4cffcf2157fe954f991cf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430761"
---
# <a name="create-grouppolicypresentationdecimaltextbox"></a><span data-ttu-id="19c75-103">Создание groupPolicyPresentationDecimalTextBox</span><span class="sxs-lookup"><span data-stu-id="19c75-103">Create groupPolicyPresentationDecimalTextBox</span></span>

> <span data-ttu-id="19c75-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="19c75-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="19c75-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19c75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19c75-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19c75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19c75-107">Создание нового объекта [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="19c75-107">Create a new [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19c75-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="19c75-108">Prerequisites</span></span>
<span data-ttu-id="19c75-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="19c75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="19c75-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19c75-111">Permission type</span></span>|<span data-ttu-id="19c75-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19c75-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19c75-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19c75-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19c75-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19c75-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="19c75-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19c75-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19c75-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19c75-116">Not supported.</span></span>|
|<span data-ttu-id="19c75-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19c75-117">Application</span></span>|<span data-ttu-id="19c75-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19c75-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19c75-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19c75-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="19c75-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19c75-120">Request headers</span></span>
|<span data-ttu-id="19c75-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19c75-121">Header</span></span>|<span data-ttu-id="19c75-122">Значение</span><span class="sxs-lookup"><span data-stu-id="19c75-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19c75-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19c75-123">Authorization</span></span>|<span data-ttu-id="19c75-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="19c75-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19c75-125">Accept</span><span class="sxs-lookup"><span data-stu-id="19c75-125">Accept</span></span>|<span data-ttu-id="19c75-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19c75-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19c75-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="19c75-127">Request body</span></span>
<span data-ttu-id="19c75-128">В тексте запроса укажите представление JSON для объекта groupPolicyPresentationDecimalTextBox.</span><span class="sxs-lookup"><span data-stu-id="19c75-128">In the request body, supply a JSON representation for the groupPolicyPresentationDecimalTextBox object.</span></span>

<span data-ttu-id="19c75-129">В следующей таблице показаны свойства, которые необходимы для создания groupPolicyPresentationDecimalTextBox.</span><span class="sxs-lookup"><span data-stu-id="19c75-129">The following table shows the properties that are required when you create the groupPolicyPresentationDecimalTextBox.</span></span>

|<span data-ttu-id="19c75-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="19c75-130">Property</span></span>|<span data-ttu-id="19c75-131">Тип</span><span class="sxs-lookup"><span data-stu-id="19c75-131">Type</span></span>|<span data-ttu-id="19c75-132">Описание</span><span class="sxs-lookup"><span data-stu-id="19c75-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19c75-133">label</span><span class="sxs-lookup"><span data-stu-id="19c75-133">label</span></span>|<span data-ttu-id="19c75-134">String</span><span class="sxs-lookup"><span data-stu-id="19c75-134">String</span></span>|<span data-ttu-id="19c75-135">Метка локализованный текст для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="19c75-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="19c75-136">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="19c75-136">The default value is empty.</span></span> <span data-ttu-id="19c75-137">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="19c75-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="19c75-138">id</span><span class="sxs-lookup"><span data-stu-id="19c75-138">id</span></span>|<span data-ttu-id="19c75-139">String</span><span class="sxs-lookup"><span data-stu-id="19c75-139">String</span></span>|<span data-ttu-id="19c75-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="19c75-140">Key of the entity.</span></span> <span data-ttu-id="19c75-141">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="19c75-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="19c75-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19c75-142">lastModifiedDateTime</span></span>|<span data-ttu-id="19c75-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19c75-143">DateTimeOffset</span></span>|<span data-ttu-id="19c75-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="19c75-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="19c75-145">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="19c75-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="19c75-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="19c75-146">defaultValue</span></span>|<span data-ttu-id="19c75-147">Int64</span><span class="sxs-lookup"><span data-stu-id="19c75-147">Int64</span></span>|<span data-ttu-id="19c75-148">Целое число без знака, задающее начальное значение для целой и дробной текстовое поле.</span><span class="sxs-lookup"><span data-stu-id="19c75-148">An unsigned integer that specifies the initial value for the decimal text box.</span></span> <span data-ttu-id="19c75-149">Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="19c75-149">The default value is 1.</span></span>|
|<span data-ttu-id="19c75-150">Счетчик</span><span class="sxs-lookup"><span data-stu-id="19c75-150">spin</span></span>|<span data-ttu-id="19c75-151">Логический</span><span class="sxs-lookup"><span data-stu-id="19c75-151">Boolean</span></span>|<span data-ttu-id="19c75-152">Если значение true, создание элемента управления "Счетчик"; в противном случае следует создайте текстовое поле для числовых записей.</span><span class="sxs-lookup"><span data-stu-id="19c75-152">If true, create a spin control; otherwise, create a text box for numeric entry.</span></span> <span data-ttu-id="19c75-153">Значение по умолчанию — true.</span><span class="sxs-lookup"><span data-stu-id="19c75-153">The default value is true.</span></span>|
|<span data-ttu-id="19c75-154">spinStep</span><span class="sxs-lookup"><span data-stu-id="19c75-154">spinStep</span></span>|<span data-ttu-id="19c75-155">Int64</span><span class="sxs-lookup"><span data-stu-id="19c75-155">Int64</span></span>|<span data-ttu-id="19c75-156">Целое число без знака, задающее шаг изменений элементов.</span><span class="sxs-lookup"><span data-stu-id="19c75-156">An unsigned integer that specifies the increment of change for the spin control.</span></span> <span data-ttu-id="19c75-157">Значение по умолчанию — 1.</span><span class="sxs-lookup"><span data-stu-id="19c75-157">The default value is 1.</span></span>|
|<span data-ttu-id="19c75-158">Обязательный</span><span class="sxs-lookup"><span data-stu-id="19c75-158">required</span></span>|<span data-ttu-id="19c75-159">Логический</span><span class="sxs-lookup"><span data-stu-id="19c75-159">Boolean</span></span>|<span data-ttu-id="19c75-160">Требование ввести значение в поле параметра.</span><span class="sxs-lookup"><span data-stu-id="19c75-160">Requirement to enter a value in the parameter box.</span></span> <span data-ttu-id="19c75-161">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="19c75-161">The default value is false.</span></span>|
|<span data-ttu-id="19c75-162">minValue</span><span class="sxs-lookup"><span data-stu-id="19c75-162">minValue</span></span>|<span data-ttu-id="19c75-163">Int64</span><span class="sxs-lookup"><span data-stu-id="19c75-163">Int64</span></span>|<span data-ttu-id="19c75-164">Целое число без знака, задающее минимальное допустимое значение.</span><span class="sxs-lookup"><span data-stu-id="19c75-164">An unsigned integer that specifies the minimum allowed value.</span></span> <span data-ttu-id="19c75-165">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="19c75-165">The default value is 0.</span></span>|
|<span data-ttu-id="19c75-166">maxValue</span><span class="sxs-lookup"><span data-stu-id="19c75-166">maxValue</span></span>|<span data-ttu-id="19c75-167">Int64</span><span class="sxs-lookup"><span data-stu-id="19c75-167">Int64</span></span>|<span data-ttu-id="19c75-168">Целое число без знака, задающее максимальное разрешенное значение.</span><span class="sxs-lookup"><span data-stu-id="19c75-168">An unsigned integer that specifies the maximum allowed value.</span></span> <span data-ttu-id="19c75-169">Значение по умолчанию — 9999.</span><span class="sxs-lookup"><span data-stu-id="19c75-169">The default value is 9999.</span></span>|



## <a name="response"></a><span data-ttu-id="19c75-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="19c75-170">Response</span></span>
<span data-ttu-id="19c75-171">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="19c75-171">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19c75-172">Пример</span><span class="sxs-lookup"><span data-stu-id="19c75-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="19c75-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="19c75-173">Request</span></span>
<span data-ttu-id="19c75-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19c75-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="19c75-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="19c75-175">Response</span></span>
<span data-ttu-id="19c75-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="19c75-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




