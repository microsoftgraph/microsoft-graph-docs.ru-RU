---
title: Создание groupPolicyPresentationMultiTextBox
description: Создание нового объекта groupPolicyPresentationMultiTextBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 41042c5ad62cb56573e924c69b62cef72ee6835c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430575"
---
# <a name="create-grouppolicypresentationmultitextbox"></a><span data-ttu-id="8805c-103">Создание groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="8805c-103">Create groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="8805c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8805c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8805c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8805c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8805c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8805c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8805c-107">Создание нового объекта [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="8805c-107">Create a new [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8805c-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="8805c-108">Prerequisites</span></span>
<span data-ttu-id="8805c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8805c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8805c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8805c-111">Permission type</span></span>|<span data-ttu-id="8805c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8805c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8805c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8805c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8805c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8805c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8805c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8805c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8805c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8805c-116">Not supported.</span></span>|
|<span data-ttu-id="8805c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8805c-117">Application</span></span>|<span data-ttu-id="8805c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8805c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8805c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8805c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="8805c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8805c-120">Request headers</span></span>
|<span data-ttu-id="8805c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8805c-121">Header</span></span>|<span data-ttu-id="8805c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8805c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8805c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8805c-123">Authorization</span></span>|<span data-ttu-id="8805c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8805c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8805c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8805c-125">Accept</span></span>|<span data-ttu-id="8805c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8805c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8805c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8805c-127">Request body</span></span>
<span data-ttu-id="8805c-128">В тексте запроса укажите представление JSON для объекта groupPolicyPresentationMultiTextBox.</span><span class="sxs-lookup"><span data-stu-id="8805c-128">In the request body, supply a JSON representation for the groupPolicyPresentationMultiTextBox object.</span></span>

<span data-ttu-id="8805c-129">В следующей таблице показаны свойства, которые необходимы для создания groupPolicyPresentationMultiTextBox.</span><span class="sxs-lookup"><span data-stu-id="8805c-129">The following table shows the properties that are required when you create the groupPolicyPresentationMultiTextBox.</span></span>

|<span data-ttu-id="8805c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8805c-130">Property</span></span>|<span data-ttu-id="8805c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8805c-131">Type</span></span>|<span data-ttu-id="8805c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8805c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8805c-133">label</span><span class="sxs-lookup"><span data-stu-id="8805c-133">label</span></span>|<span data-ttu-id="8805c-134">String</span><span class="sxs-lookup"><span data-stu-id="8805c-134">String</span></span>|<span data-ttu-id="8805c-135">Метка локализованный текст для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="8805c-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="8805c-136">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="8805c-136">The default value is empty.</span></span> <span data-ttu-id="8805c-137">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8805c-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8805c-138">id</span><span class="sxs-lookup"><span data-stu-id="8805c-138">id</span></span>|<span data-ttu-id="8805c-139">String</span><span class="sxs-lookup"><span data-stu-id="8805c-139">String</span></span>|<span data-ttu-id="8805c-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8805c-140">Key of the entity.</span></span> <span data-ttu-id="8805c-141">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8805c-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8805c-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8805c-142">lastModifiedDateTime</span></span>|<span data-ttu-id="8805c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8805c-143">DateTimeOffset</span></span>|<span data-ttu-id="8805c-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8805c-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="8805c-145">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="8805c-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="8805c-146">Обязательный</span><span class="sxs-lookup"><span data-stu-id="8805c-146">required</span></span>|<span data-ttu-id="8805c-147">Логический</span><span class="sxs-lookup"><span data-stu-id="8805c-147">Boolean</span></span>|<span data-ttu-id="8805c-148">Требование ввести значение в текстовом поле.</span><span class="sxs-lookup"><span data-stu-id="8805c-148">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="8805c-149">Значение по умолчанию — False.</span><span class="sxs-lookup"><span data-stu-id="8805c-149">Default value is false.</span></span>|
|<span data-ttu-id="8805c-150">maxLength</span><span class="sxs-lookup"><span data-stu-id="8805c-150">maxLength</span></span>|<span data-ttu-id="8805c-151">Int64</span><span class="sxs-lookup"><span data-stu-id="8805c-151">Int64</span></span>|<span data-ttu-id="8805c-152">Целое число без знака, задающее максимальное количество текстовых символов.</span><span class="sxs-lookup"><span data-stu-id="8805c-152">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="8805c-153">Значение по умолчанию — 1023.</span><span class="sxs-lookup"><span data-stu-id="8805c-153">Default value is 1023.</span></span>|
|<span data-ttu-id="8805c-154">maxStrings</span><span class="sxs-lookup"><span data-stu-id="8805c-154">maxStrings</span></span>|<span data-ttu-id="8805c-155">Int64</span><span class="sxs-lookup"><span data-stu-id="8805c-155">Int64</span></span>|<span data-ttu-id="8805c-156">Целое число без знака, задающее максимальное число строк.</span><span class="sxs-lookup"><span data-stu-id="8805c-156">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="8805c-157">Значение по умолчанию равно 0.</span><span class="sxs-lookup"><span data-stu-id="8805c-157">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="8805c-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="8805c-158">Response</span></span>
<span data-ttu-id="8805c-159">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8805c-159">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8805c-160">Пример</span><span class="sxs-lookup"><span data-stu-id="8805c-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="8805c-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="8805c-161">Request</span></span>
<span data-ttu-id="8805c-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8805c-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```

### <a name="response"></a><span data-ttu-id="8805c-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="8805c-163">Response</span></span>
<span data-ttu-id="8805c-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8805c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 278

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "id": "381ac035-c035-381a-35c0-1a3835c01a38",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```




