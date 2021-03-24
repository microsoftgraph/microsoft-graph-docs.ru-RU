---
title: Создание groupPolicyPresentationCheckBox
description: Создайте новый объект GroupPolicyPresentationCheckBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 01aa0db90883a469685edacd839188dcea5235b7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142004"
---
# <a name="create-grouppolicypresentationcheckbox"></a><span data-ttu-id="3a9c2-103">Создание groupPolicyPresentationCheckBox</span><span class="sxs-lookup"><span data-stu-id="3a9c2-103">Create groupPolicyPresentationCheckBox</span></span>

<span data-ttu-id="3a9c2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a9c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a9c2-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a9c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a9c2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a9c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a9c2-107">Создайте новый [объект GroupPolicyPresentationCheckBox.](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)</span><span class="sxs-lookup"><span data-stu-id="3a9c2-107">Create a new [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a9c2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3a9c2-108">Prerequisites</span></span>
<span data-ttu-id="3a9c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a9c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a9c2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a9c2-111">Permission type</span></span>|<span data-ttu-id="3a9c2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a9c2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a9c2-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a9c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a9c2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9c2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a9c2-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a9c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a9c2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a9c2-116">Not supported.</span></span>|
|<span data-ttu-id="3a9c2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3a9c2-117">Application</span></span>|<span data-ttu-id="3a9c2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9c2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a9c2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a9c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="3a9c2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3a9c2-120">Request headers</span></span>
|<span data-ttu-id="3a9c2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a9c2-121">Header</span></span>|<span data-ttu-id="3a9c2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3a9c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a9c2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a9c2-123">Authorization</span></span>|<span data-ttu-id="3a9c2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a9c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a9c2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a9c2-125">Accept</span></span>|<span data-ttu-id="3a9c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a9c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a9c2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a9c2-127">Request body</span></span>
<span data-ttu-id="3a9c2-128">В теле запроса поставляем представление JSON для объекта groupPolicyPresentationCheckBox.</span><span class="sxs-lookup"><span data-stu-id="3a9c2-128">In the request body, supply a JSON representation for the groupPolicyPresentationCheckBox object.</span></span>

<span data-ttu-id="3a9c2-129">В следующей таблице показаны свойства, необходимые при создании groupPolicyPresentationCheckBox.</span><span class="sxs-lookup"><span data-stu-id="3a9c2-129">The following table shows the properties that are required when you create the groupPolicyPresentationCheckBox.</span></span>

|<span data-ttu-id="3a9c2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a9c2-130">Property</span></span>|<span data-ttu-id="3a9c2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3a9c2-131">Type</span></span>|<span data-ttu-id="3a9c2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3a9c2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a9c2-133">label</span><span class="sxs-lookup"><span data-stu-id="3a9c2-133">label</span></span>|<span data-ttu-id="3a9c2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3a9c2-134">String</span></span>|<span data-ttu-id="3a9c2-135">Локализованная текстовая метка для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="3a9c2-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="3a9c2-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="3a9c2-136">The default value is empty.</span></span> <span data-ttu-id="3a9c2-137">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3a9c2-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="3a9c2-138">id</span><span class="sxs-lookup"><span data-stu-id="3a9c2-138">id</span></span>|<span data-ttu-id="3a9c2-139">Строка</span><span class="sxs-lookup"><span data-stu-id="3a9c2-139">String</span></span>|<span data-ttu-id="3a9c2-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3a9c2-140">Key of the entity.</span></span> <span data-ttu-id="3a9c2-141">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3a9c2-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="3a9c2-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a9c2-142">lastModifiedDateTime</span></span>|<span data-ttu-id="3a9c2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a9c2-143">DateTimeOffset</span></span>|<span data-ttu-id="3a9c2-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3a9c2-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="3a9c2-145">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="3a9c2-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="3a9c2-146">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="3a9c2-146">defaultChecked</span></span>|<span data-ttu-id="3a9c2-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a9c2-147">Boolean</span></span>|<span data-ttu-id="3a9c2-148">Значение по умолчанию для контрольного окна.</span><span class="sxs-lookup"><span data-stu-id="3a9c2-148">Default value for the check box.</span></span> <span data-ttu-id="3a9c2-149">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="3a9c2-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="3a9c2-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a9c2-150">Response</span></span>
<span data-ttu-id="3a9c2-151">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект GroupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3a9c2-151">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a9c2-152">Пример</span><span class="sxs-lookup"><span data-stu-id="3a9c2-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a9c2-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a9c2-153">Request</span></span>
<span data-ttu-id="3a9c2-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a9c2-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3a9c2-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a9c2-155">Response</span></span>
<span data-ttu-id="3a9c2-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a9c2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




