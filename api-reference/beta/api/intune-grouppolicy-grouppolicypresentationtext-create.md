---
title: Создание Граупполиципресентатионтекст
description: Создание нового объекта Граупполиципресентатионтекст.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eaf460bd850958a1804a78d8b580f3c364953993
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43408722"
---
# <a name="create-grouppolicypresentationtext"></a><span data-ttu-id="42255-103">Создание Граупполиципресентатионтекст</span><span class="sxs-lookup"><span data-stu-id="42255-103">Create groupPolicyPresentationText</span></span>

<span data-ttu-id="42255-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42255-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42255-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42255-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42255-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42255-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42255-107">Создание нового объекта [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .</span><span class="sxs-lookup"><span data-stu-id="42255-107">Create a new [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42255-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="42255-108">Prerequisites</span></span>
<span data-ttu-id="42255-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42255-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42255-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42255-111">Permission type</span></span>|<span data-ttu-id="42255-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42255-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42255-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42255-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42255-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42255-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42255-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42255-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42255-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42255-116">Not supported.</span></span>|
|<span data-ttu-id="42255-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="42255-117">Application</span></span>|<span data-ttu-id="42255-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42255-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42255-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42255-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="42255-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="42255-120">Request headers</span></span>
|<span data-ttu-id="42255-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42255-121">Header</span></span>|<span data-ttu-id="42255-122">Значение</span><span class="sxs-lookup"><span data-stu-id="42255-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42255-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42255-123">Authorization</span></span>|<span data-ttu-id="42255-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42255-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42255-125">Accept</span><span class="sxs-lookup"><span data-stu-id="42255-125">Accept</span></span>|<span data-ttu-id="42255-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42255-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42255-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42255-127">Request body</span></span>
<span data-ttu-id="42255-128">В тексте запроса добавьте представление объекта Граупполиципресентатионтекст в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42255-128">In the request body, supply a JSON representation for the groupPolicyPresentationText object.</span></span>

<span data-ttu-id="42255-129">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионтекст.</span><span class="sxs-lookup"><span data-stu-id="42255-129">The following table shows the properties that are required when you create the groupPolicyPresentationText.</span></span>

|<span data-ttu-id="42255-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="42255-130">Property</span></span>|<span data-ttu-id="42255-131">Тип</span><span class="sxs-lookup"><span data-stu-id="42255-131">Type</span></span>|<span data-ttu-id="42255-132">Описание</span><span class="sxs-lookup"><span data-stu-id="42255-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42255-133">label</span><span class="sxs-lookup"><span data-stu-id="42255-133">label</span></span>|<span data-ttu-id="42255-134">String</span><span class="sxs-lookup"><span data-stu-id="42255-134">String</span></span>|<span data-ttu-id="42255-135">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="42255-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="42255-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="42255-136">The default value is empty.</span></span> <span data-ttu-id="42255-137">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="42255-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="42255-138">id</span><span class="sxs-lookup"><span data-stu-id="42255-138">id</span></span>|<span data-ttu-id="42255-139">String</span><span class="sxs-lookup"><span data-stu-id="42255-139">String</span></span>|<span data-ttu-id="42255-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="42255-140">Key of the entity.</span></span> <span data-ttu-id="42255-141">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="42255-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="42255-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42255-142">lastModifiedDateTime</span></span>|<span data-ttu-id="42255-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42255-143">DateTimeOffset</span></span>|<span data-ttu-id="42255-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="42255-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="42255-145">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="42255-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="42255-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="42255-146">Response</span></span>
<span data-ttu-id="42255-147">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионтекст](../resources/intune-grouppolicy-grouppolicypresentationtext.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42255-147">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42255-148">Пример</span><span class="sxs-lookup"><span data-stu-id="42255-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="42255-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="42255-149">Request</span></span>
<span data-ttu-id="42255-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42255-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="42255-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="42255-151">Response</span></span>
<span data-ttu-id="42255-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42255-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



