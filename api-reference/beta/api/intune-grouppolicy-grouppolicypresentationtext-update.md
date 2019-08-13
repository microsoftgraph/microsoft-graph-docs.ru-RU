---
title: Обновление Граупполиципресентатионтекст
description: Обновление свойств объекта Граупполиципресентатионтекст.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 84b1d305802eb1b7071952005aa61b7047a827d8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36354711"
---
# <a name="update-grouppolicypresentationtext"></a><span data-ttu-id="ab362-103">Обновление Граупполиципресентатионтекст</span><span class="sxs-lookup"><span data-stu-id="ab362-103">Update groupPolicyPresentationText</span></span>

> <span data-ttu-id="ab362-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab362-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab362-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab362-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab362-106">Обновление свойств объекта [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .</span><span class="sxs-lookup"><span data-stu-id="ab362-106">Update the properties of a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab362-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ab362-107">Prerequisites</span></span>
<span data-ttu-id="ab362-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab362-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab362-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab362-110">Permission type</span></span>|<span data-ttu-id="ab362-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab362-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab362-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab362-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ab362-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab362-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ab362-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab362-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab362-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab362-115">Not supported.</span></span>|
|<span data-ttu-id="ab362-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab362-116">Application</span></span>|<span data-ttu-id="ab362-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab362-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab362-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab362-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="ab362-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab362-119">Request headers</span></span>
|<span data-ttu-id="ab362-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab362-120">Header</span></span>|<span data-ttu-id="ab362-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ab362-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab362-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab362-122">Authorization</span></span>|<span data-ttu-id="ab362-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab362-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab362-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ab362-124">Accept</span></span>|<span data-ttu-id="ab362-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ab362-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab362-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ab362-126">Request body</span></span>
<span data-ttu-id="ab362-127">В тексте запроса добавьте представление объекта [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab362-127">In the request body, supply a JSON representation for the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

<span data-ttu-id="ab362-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md).</span><span class="sxs-lookup"><span data-stu-id="ab362-128">The following table shows the properties that are required when you create the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md).</span></span>

|<span data-ttu-id="ab362-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab362-129">Property</span></span>|<span data-ttu-id="ab362-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ab362-130">Type</span></span>|<span data-ttu-id="ab362-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ab362-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab362-132">label</span><span class="sxs-lookup"><span data-stu-id="ab362-132">label</span></span>|<span data-ttu-id="ab362-133">String</span><span class="sxs-lookup"><span data-stu-id="ab362-133">String</span></span>|<span data-ttu-id="ab362-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="ab362-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="ab362-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="ab362-135">The default value is empty.</span></span> <span data-ttu-id="ab362-136">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ab362-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ab362-137">id</span><span class="sxs-lookup"><span data-stu-id="ab362-137">id</span></span>|<span data-ttu-id="ab362-138">String</span><span class="sxs-lookup"><span data-stu-id="ab362-138">String</span></span>|<span data-ttu-id="ab362-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ab362-139">Key of the entity.</span></span> <span data-ttu-id="ab362-140">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ab362-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ab362-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab362-141">lastModifiedDateTime</span></span>|<span data-ttu-id="ab362-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab362-142">DateTimeOffset</span></span>|<span data-ttu-id="ab362-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ab362-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="ab362-144">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ab362-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ab362-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab362-145">Response</span></span>
<span data-ttu-id="ab362-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab362-146">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab362-147">Пример</span><span class="sxs-lookup"><span data-stu-id="ab362-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab362-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab362-148">Request</span></span>
<span data-ttu-id="ab362-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab362-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="ab362-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab362-150">Response</span></span>
<span data-ttu-id="ab362-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab362-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






