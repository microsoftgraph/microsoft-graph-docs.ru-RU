---
title: Создание Граупполиципресентатионтекст
description: Создание нового объекта Граупполиципресентатионтекст.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5fd3ca365eb92185e575850d3ca044478f4ead40
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33904729"
---
# <a name="create-grouppolicypresentationtext"></a><span data-ttu-id="9803c-103">Создание Граупполиципресентатионтекст</span><span class="sxs-lookup"><span data-stu-id="9803c-103">Create groupPolicyPresentationText</span></span>

> <span data-ttu-id="9803c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9803c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9803c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9803c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9803c-106">Создание нового объекта [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .</span><span class="sxs-lookup"><span data-stu-id="9803c-106">Create a new [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9803c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9803c-107">Prerequisites</span></span>
<span data-ttu-id="9803c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9803c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9803c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9803c-110">Permission type</span></span>|<span data-ttu-id="9803c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9803c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9803c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9803c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9803c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9803c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9803c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9803c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9803c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9803c-115">Not supported.</span></span>|
|<span data-ttu-id="9803c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9803c-116">Application</span></span>|<span data-ttu-id="9803c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9803c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9803c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9803c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="9803c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9803c-119">Request headers</span></span>
|<span data-ttu-id="9803c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9803c-120">Header</span></span>|<span data-ttu-id="9803c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9803c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9803c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9803c-122">Authorization</span></span>|<span data-ttu-id="9803c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9803c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9803c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9803c-124">Accept</span></span>|<span data-ttu-id="9803c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9803c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9803c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9803c-126">Request body</span></span>
<span data-ttu-id="9803c-127">В тексте запроса добавьте представление объекта Граупполиципресентатионтекст в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9803c-127">In the request body, supply a JSON representation for the groupPolicyPresentationText object.</span></span>

<span data-ttu-id="9803c-128">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионтекст.</span><span class="sxs-lookup"><span data-stu-id="9803c-128">The following table shows the properties that are required when you create the groupPolicyPresentationText.</span></span>

|<span data-ttu-id="9803c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9803c-129">Property</span></span>|<span data-ttu-id="9803c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9803c-130">Type</span></span>|<span data-ttu-id="9803c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9803c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9803c-132">label</span><span class="sxs-lookup"><span data-stu-id="9803c-132">label</span></span>|<span data-ttu-id="9803c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9803c-133">String</span></span>|<span data-ttu-id="9803c-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="9803c-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="9803c-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="9803c-135">The default value is empty.</span></span> <span data-ttu-id="9803c-136">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9803c-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9803c-137">id</span><span class="sxs-lookup"><span data-stu-id="9803c-137">id</span></span>|<span data-ttu-id="9803c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="9803c-138">String</span></span>|<span data-ttu-id="9803c-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9803c-139">Key of the entity.</span></span> <span data-ttu-id="9803c-140">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9803c-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="9803c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9803c-141">lastModifiedDateTime</span></span>|<span data-ttu-id="9803c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9803c-142">DateTimeOffset</span></span>|<span data-ttu-id="9803c-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9803c-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="9803c-144">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="9803c-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9803c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9803c-145">Response</span></span>
<span data-ttu-id="9803c-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9803c-146">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9803c-147">Пример</span><span class="sxs-lookup"><span data-stu-id="9803c-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="9803c-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="9803c-148">Request</span></span>
<span data-ttu-id="9803c-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9803c-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="9803c-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="9803c-150">Response</span></span>
<span data-ttu-id="9803c-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9803c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 209

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value",
  "id": "bc77d545-d545-bc77-45d5-77bc45d577bc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




