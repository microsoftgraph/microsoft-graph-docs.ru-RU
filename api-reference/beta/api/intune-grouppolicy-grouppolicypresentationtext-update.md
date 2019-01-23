---
title: Обновление groupPolicyPresentationText
description: Обновление свойства объекта groupPolicyPresentationText.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 750a98c0c0dbeb90e6e8a7987d8988bb1aebe5d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430852"
---
# <a name="update-grouppolicypresentationtext"></a><span data-ttu-id="e825c-103">Обновление groupPolicyPresentationText</span><span class="sxs-lookup"><span data-stu-id="e825c-103">Update groupPolicyPresentationText</span></span>

> <span data-ttu-id="e825c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e825c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e825c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e825c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e825c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e825c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e825c-107">Обновление свойства объекта [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .</span><span class="sxs-lookup"><span data-stu-id="e825c-107">Update the properties of a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e825c-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="e825c-108">Prerequisites</span></span>
<span data-ttu-id="e825c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e825c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e825c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e825c-111">Permission type</span></span>|<span data-ttu-id="e825c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e825c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e825c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e825c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e825c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e825c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e825c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e825c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e825c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e825c-116">Not supported.</span></span>|
|<span data-ttu-id="e825c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e825c-117">Application</span></span>|<span data-ttu-id="e825c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e825c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e825c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e825c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="e825c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e825c-120">Request headers</span></span>
|<span data-ttu-id="e825c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e825c-121">Header</span></span>|<span data-ttu-id="e825c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e825c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e825c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e825c-123">Authorization</span></span>|<span data-ttu-id="e825c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e825c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e825c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e825c-125">Accept</span></span>|<span data-ttu-id="e825c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e825c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e825c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e825c-127">Request body</span></span>
<span data-ttu-id="e825c-128">В тексте запроса укажите представление JSON для объекта [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .</span><span class="sxs-lookup"><span data-stu-id="e825c-128">In the request body, supply a JSON representation for the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

<span data-ttu-id="e825c-129">В следующей таблице показаны свойства, которые необходимы для создания [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md).</span><span class="sxs-lookup"><span data-stu-id="e825c-129">The following table shows the properties that are required when you create the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md).</span></span>

|<span data-ttu-id="e825c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e825c-130">Property</span></span>|<span data-ttu-id="e825c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e825c-131">Type</span></span>|<span data-ttu-id="e825c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e825c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e825c-133">label</span><span class="sxs-lookup"><span data-stu-id="e825c-133">label</span></span>|<span data-ttu-id="e825c-134">String</span><span class="sxs-lookup"><span data-stu-id="e825c-134">String</span></span>|<span data-ttu-id="e825c-135">Метка локализованный текст для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="e825c-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="e825c-136">Значение по умолчанию будет пустым.</span><span class="sxs-lookup"><span data-stu-id="e825c-136">The default value is empty.</span></span> <span data-ttu-id="e825c-137">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="e825c-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="e825c-138">id</span><span class="sxs-lookup"><span data-stu-id="e825c-138">id</span></span>|<span data-ttu-id="e825c-139">String</span><span class="sxs-lookup"><span data-stu-id="e825c-139">String</span></span>|<span data-ttu-id="e825c-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e825c-140">Key of the entity.</span></span> <span data-ttu-id="e825c-141">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="e825c-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="e825c-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e825c-142">lastModifiedDateTime</span></span>|<span data-ttu-id="e825c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e825c-143">DateTimeOffset</span></span>|<span data-ttu-id="e825c-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e825c-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="e825c-145">Наследуется от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="e825c-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e825c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="e825c-146">Response</span></span>
<span data-ttu-id="e825c-147">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e825c-147">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e825c-148">Пример</span><span class="sxs-lookup"><span data-stu-id="e825c-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="e825c-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="e825c-149">Request</span></span>
<span data-ttu-id="e825c-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e825c-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="e825c-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="e825c-151">Response</span></span>
<span data-ttu-id="e825c-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e825c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 209

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value",
  "id": "bc77d545-d545-bc77-45d5-77bc45d577bc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




