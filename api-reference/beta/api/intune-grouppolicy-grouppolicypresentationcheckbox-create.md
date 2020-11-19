---
title: Создание Граупполиципресентатиончеккбокс
description: Создание нового объекта Граупполиципресентатиончеккбокс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b1f3a517d924f0f7a6690d51440e60f5d6ae12a3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49285879"
---
# <a name="create-grouppolicypresentationcheckbox"></a><span data-ttu-id="c5727-103">Создание Граупполиципресентатиончеккбокс</span><span class="sxs-lookup"><span data-stu-id="c5727-103">Create groupPolicyPresentationCheckBox</span></span>

<span data-ttu-id="c5727-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5727-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5727-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5727-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5727-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5727-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5727-107">Создание нового объекта [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .</span><span class="sxs-lookup"><span data-stu-id="c5727-107">Create a new [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5727-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c5727-108">Prerequisites</span></span>
<span data-ttu-id="c5727-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5727-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5727-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5727-111">Permission type</span></span>|<span data-ttu-id="c5727-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5727-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5727-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5727-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5727-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5727-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5727-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5727-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5727-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5727-116">Not supported.</span></span>|
|<span data-ttu-id="c5727-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5727-117">Application</span></span>|<span data-ttu-id="c5727-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5727-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5727-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5727-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="c5727-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c5727-120">Request headers</span></span>
|<span data-ttu-id="c5727-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5727-121">Header</span></span>|<span data-ttu-id="c5727-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c5727-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5727-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5727-123">Authorization</span></span>|<span data-ttu-id="c5727-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5727-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5727-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5727-125">Accept</span></span>|<span data-ttu-id="c5727-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5727-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5727-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5727-127">Request body</span></span>
<span data-ttu-id="c5727-128">В тексте запроса добавьте представление объекта Граупполиципресентатиончеккбокс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5727-128">In the request body, supply a JSON representation for the groupPolicyPresentationCheckBox object.</span></span>

<span data-ttu-id="c5727-129">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатиончеккбокс.</span><span class="sxs-lookup"><span data-stu-id="c5727-129">The following table shows the properties that are required when you create the groupPolicyPresentationCheckBox.</span></span>

|<span data-ttu-id="c5727-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5727-130">Property</span></span>|<span data-ttu-id="c5727-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c5727-131">Type</span></span>|<span data-ttu-id="c5727-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c5727-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5727-133">label</span><span class="sxs-lookup"><span data-stu-id="c5727-133">label</span></span>|<span data-ttu-id="c5727-134">String</span><span class="sxs-lookup"><span data-stu-id="c5727-134">String</span></span>|<span data-ttu-id="c5727-135">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="c5727-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="c5727-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="c5727-136">The default value is empty.</span></span> <span data-ttu-id="c5727-137">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c5727-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c5727-138">id</span><span class="sxs-lookup"><span data-stu-id="c5727-138">id</span></span>|<span data-ttu-id="c5727-139">String</span><span class="sxs-lookup"><span data-stu-id="c5727-139">String</span></span>|<span data-ttu-id="c5727-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c5727-140">Key of the entity.</span></span> <span data-ttu-id="c5727-141">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c5727-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c5727-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5727-142">lastModifiedDateTime</span></span>|<span data-ttu-id="c5727-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5727-143">DateTimeOffset</span></span>|<span data-ttu-id="c5727-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c5727-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="c5727-145">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c5727-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c5727-146">дефаултчеккед</span><span class="sxs-lookup"><span data-stu-id="c5727-146">defaultChecked</span></span>|<span data-ttu-id="c5727-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5727-147">Boolean</span></span>|<span data-ttu-id="c5727-148">Значение по умолчанию для этого флажка.</span><span class="sxs-lookup"><span data-stu-id="c5727-148">Default value for the check box.</span></span> <span data-ttu-id="c5727-149">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="c5727-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="c5727-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5727-150">Response</span></span>
<span data-ttu-id="c5727-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5727-151">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5727-152">Пример</span><span class="sxs-lookup"><span data-stu-id="c5727-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5727-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5727-153">Request</span></span>
<span data-ttu-id="c5727-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5727-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c5727-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5727-155">Response</span></span>
<span data-ttu-id="c5727-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5727-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




