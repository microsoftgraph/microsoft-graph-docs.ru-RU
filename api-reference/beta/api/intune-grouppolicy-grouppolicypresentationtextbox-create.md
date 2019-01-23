---
title: Создание groupPolicyPresentationTextBox
description: Создание нового объекта groupPolicyPresentationTextBox.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 20a34e2288541fe948464b1410398138316943a4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430813"
---
# <a name="create-grouppolicypresentationtextbox"></a><span data-ttu-id="fb58d-103">Создание groupPolicyPresentationTextBox</span><span class="sxs-lookup"><span data-stu-id="fb58d-103">Create groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="fb58d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fb58d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fb58d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb58d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb58d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb58d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb58d-107">Создание нового объекта [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="fb58d-107">Create a new [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb58d-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="fb58d-108">Prerequisites</span></span>
<span data-ttu-id="fb58d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fb58d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fb58d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb58d-111">Permission type</span></span>|<span data-ttu-id="fb58d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb58d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb58d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb58d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb58d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb58d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fb58d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb58d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb58d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb58d-116">Not supported.</span></span>|
|<span data-ttu-id="fb58d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb58d-117">Application</span></span>|<span data-ttu-id="fb58d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb58d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb58d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb58d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="fb58d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb58d-120">Request headers</span></span>
|<span data-ttu-id="fb58d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb58d-121">Header</span></span>|<span data-ttu-id="fb58d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fb58d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb58d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb58d-123">Authorization</span></span>|<span data-ttu-id="fb58d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fb58d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb58d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb58d-125">Accept</span></span>|<span data-ttu-id="fb58d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb58d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb58d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb58d-127">Request body</span></span>
<span data-ttu-id="fb58d-128">В тексте запроса укажите представление JSON для объекта groupPolicyPresentationTextBox.</span><span class="sxs-lookup"><span data-stu-id="fb58d-128">In the request body, supply a JSON representation for the groupPolicyPresentationTextBox object.</span></span>

<span data-ttu-id="fb58d-129">В следующей таблице показаны свойства, которые необходимы для создания groupPolicyPresentationTextBox.</span><span class="sxs-lookup"><span data-stu-id="fb58d-129">The following table shows the properties that are required when you create the groupPolicyPresentationTextBox.</span></span>

|<span data-ttu-id="fb58d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb58d-130">Property</span></span>|<span data-ttu-id="fb58d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fb58d-131">Type</span></span>|<span data-ttu-id="fb58d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fb58d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb58d-133">label</span><span class="sxs-lookup"><span data-stu-id="fb58d-133">label</span></span>|<span data-ttu-id="fb58d-134">String</span><span class="sxs-lookup"><span data-stu-id="fb58d-134">String</span></span>|<span data-ttu-id="fb58d-135">Метка локализованный текст для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="fb58d-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="fb58d-136">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="fb58d-136">The default value is empty.</span></span> <span data-ttu-id="fb58d-137">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="fb58d-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="fb58d-138">id</span><span class="sxs-lookup"><span data-stu-id="fb58d-138">id</span></span>|<span data-ttu-id="fb58d-139">String</span><span class="sxs-lookup"><span data-stu-id="fb58d-139">String</span></span>|<span data-ttu-id="fb58d-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fb58d-140">Key of the entity.</span></span> <span data-ttu-id="fb58d-141">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="fb58d-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="fb58d-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb58d-142">lastModifiedDateTime</span></span>|<span data-ttu-id="fb58d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb58d-143">DateTimeOffset</span></span>|<span data-ttu-id="fb58d-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fb58d-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="fb58d-145">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="fb58d-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="fb58d-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="fb58d-146">defaultValue</span></span>|<span data-ttu-id="fb58d-147">String</span><span class="sxs-lookup"><span data-stu-id="fb58d-147">String</span></span>|<span data-ttu-id="fb58d-148">Локализованные строки по умолчанию, отображаемой в текстовом поле.</span><span class="sxs-lookup"><span data-stu-id="fb58d-148">Localized default string displayed in the text box.</span></span> <span data-ttu-id="fb58d-149">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="fb58d-149">The default value is empty.</span></span>|
|<span data-ttu-id="fb58d-150">Обязательный</span><span class="sxs-lookup"><span data-stu-id="fb58d-150">required</span></span>|<span data-ttu-id="fb58d-151">Логический</span><span class="sxs-lookup"><span data-stu-id="fb58d-151">Boolean</span></span>|<span data-ttu-id="fb58d-152">Требование ввести значение в текстовом поле.</span><span class="sxs-lookup"><span data-stu-id="fb58d-152">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="fb58d-153">Значение по умолчанию — False.</span><span class="sxs-lookup"><span data-stu-id="fb58d-153">Default value is false.</span></span>|
|<span data-ttu-id="fb58d-154">maxLength</span><span class="sxs-lookup"><span data-stu-id="fb58d-154">maxLength</span></span>|<span data-ttu-id="fb58d-155">Int64</span><span class="sxs-lookup"><span data-stu-id="fb58d-155">Int64</span></span>|<span data-ttu-id="fb58d-156">Целое число без знака, задающее максимальное количество текстовых символов.</span><span class="sxs-lookup"><span data-stu-id="fb58d-156">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="fb58d-157">Значение по умолчанию — 1023.</span><span class="sxs-lookup"><span data-stu-id="fb58d-157">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="fb58d-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb58d-158">Response</span></span>
<span data-ttu-id="fb58d-159">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fb58d-159">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb58d-160">Пример</span><span class="sxs-lookup"><span data-stu-id="fb58d-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb58d-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb58d-161">Request</span></span>
<span data-ttu-id="fb58d-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb58d-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
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

### <a name="response"></a><span data-ttu-id="fb58d-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb58d-163">Response</span></span>
<span data-ttu-id="fb58d-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fb58d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




