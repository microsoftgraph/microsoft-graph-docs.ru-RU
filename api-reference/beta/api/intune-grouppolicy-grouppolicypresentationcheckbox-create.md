---
title: Создание Граупполиципресентатиончеккбокс
description: Создание нового объекта Граупполиципресентатиончеккбокс.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4f1346c446699905956a120307463dee43a08e1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965419"
---
# <a name="create-grouppolicypresentationcheckbox"></a><span data-ttu-id="fc176-103">Создание Граупполиципресентатиончеккбокс</span><span class="sxs-lookup"><span data-stu-id="fc176-103">Create groupPolicyPresentationCheckBox</span></span>

> <span data-ttu-id="fc176-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc176-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc176-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc176-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc176-106">Создание нового объекта [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="fc176-106">Create a new [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc176-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fc176-107">Prerequisites</span></span>
<span data-ttu-id="fc176-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc176-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc176-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc176-110">Permission type</span></span>|<span data-ttu-id="fc176-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc176-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc176-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc176-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc176-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc176-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fc176-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc176-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc176-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc176-115">Not supported.</span></span>|
|<span data-ttu-id="fc176-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc176-116">Application</span></span>|<span data-ttu-id="fc176-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc176-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc176-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc176-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="fc176-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc176-119">Request headers</span></span>
|<span data-ttu-id="fc176-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc176-120">Header</span></span>|<span data-ttu-id="fc176-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fc176-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc176-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc176-122">Authorization</span></span>|<span data-ttu-id="fc176-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc176-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc176-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fc176-124">Accept</span></span>|<span data-ttu-id="fc176-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc176-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc176-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc176-126">Request body</span></span>
<span data-ttu-id="fc176-127">В тексте запроса добавьте представление объекта Граупполиципресентатиончеккбокс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc176-127">In the request body, supply a JSON representation for the groupPolicyPresentationCheckBox object.</span></span>

<span data-ttu-id="fc176-128">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатиончеккбокс.</span><span class="sxs-lookup"><span data-stu-id="fc176-128">The following table shows the properties that are required when you create the groupPolicyPresentationCheckBox.</span></span>

|<span data-ttu-id="fc176-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc176-129">Property</span></span>|<span data-ttu-id="fc176-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fc176-130">Type</span></span>|<span data-ttu-id="fc176-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fc176-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc176-132">label</span><span class="sxs-lookup"><span data-stu-id="fc176-132">label</span></span>|<span data-ttu-id="fc176-133">String</span><span class="sxs-lookup"><span data-stu-id="fc176-133">String</span></span>|<span data-ttu-id="fc176-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="fc176-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="fc176-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="fc176-135">The default value is empty.</span></span> <span data-ttu-id="fc176-136">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="fc176-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="fc176-137">id</span><span class="sxs-lookup"><span data-stu-id="fc176-137">id</span></span>|<span data-ttu-id="fc176-138">String</span><span class="sxs-lookup"><span data-stu-id="fc176-138">String</span></span>|<span data-ttu-id="fc176-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fc176-139">Key of the entity.</span></span> <span data-ttu-id="fc176-140">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="fc176-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="fc176-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc176-141">lastModifiedDateTime</span></span>|<span data-ttu-id="fc176-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc176-142">DateTimeOffset</span></span>|<span data-ttu-id="fc176-143">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fc176-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="fc176-144">НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="fc176-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="fc176-145">Дефаултчеккед</span><span class="sxs-lookup"><span data-stu-id="fc176-145">defaultChecked</span></span>|<span data-ttu-id="fc176-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc176-146">Boolean</span></span>|<span data-ttu-id="fc176-147">Значение по умолчанию для этого флажка.</span><span class="sxs-lookup"><span data-stu-id="fc176-147">Default value for the check box.</span></span> <span data-ttu-id="fc176-148">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="fc176-148">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="fc176-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc176-149">Response</span></span>
<span data-ttu-id="fc176-150">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc176-150">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc176-151">Пример</span><span class="sxs-lookup"><span data-stu-id="fc176-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc176-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc176-152">Request</span></span>
<span data-ttu-id="fc176-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc176-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "defaultChecked": true
}
```

### <a name="response"></a><span data-ttu-id="fc176-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc176-154">Response</span></span>
<span data-ttu-id="fc176-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc176-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "id": "7748190f-190f-7748-0f19-48770f194877",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultChecked": true
}
```




