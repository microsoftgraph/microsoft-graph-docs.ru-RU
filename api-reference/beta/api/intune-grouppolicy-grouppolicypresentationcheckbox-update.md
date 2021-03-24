---
title: Обновление groupPolicyPresentationCheckBox
description: Обновление свойств объекта groupPolicyPresentationCheckBox.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 65a8250a05237bab453aadc8a130b791c0758bcd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149781"
---
# <a name="update-grouppolicypresentationcheckbox"></a><span data-ttu-id="d80c5-103">Обновление groupPolicyPresentationCheckBox</span><span class="sxs-lookup"><span data-stu-id="d80c5-103">Update groupPolicyPresentationCheckBox</span></span>

<span data-ttu-id="d80c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d80c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d80c5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d80c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d80c5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d80c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d80c5-107">Обновление свойств объекта [groupPolicyPresentationCheckBox.](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)</span><span class="sxs-lookup"><span data-stu-id="d80c5-107">Update the properties of a [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d80c5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d80c5-108">Prerequisites</span></span>
<span data-ttu-id="d80c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d80c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d80c5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d80c5-111">Permission type</span></span>|<span data-ttu-id="d80c5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d80c5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d80c5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d80c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d80c5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d80c5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d80c5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d80c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d80c5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d80c5-116">Not supported.</span></span>|
|<span data-ttu-id="d80c5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d80c5-117">Application</span></span>|<span data-ttu-id="d80c5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d80c5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d80c5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d80c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="d80c5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d80c5-120">Request headers</span></span>
|<span data-ttu-id="d80c5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d80c5-121">Header</span></span>|<span data-ttu-id="d80c5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d80c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d80c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d80c5-123">Authorization</span></span>|<span data-ttu-id="d80c5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d80c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d80c5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d80c5-125">Accept</span></span>|<span data-ttu-id="d80c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d80c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d80c5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d80c5-127">Request body</span></span>
<span data-ttu-id="d80c5-128">В теле запроса поставляем представление JSON для [объекта groupPolicyPresentationCheckBox.](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)</span><span class="sxs-lookup"><span data-stu-id="d80c5-128">In the request body, supply a JSON representation for the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object.</span></span>

<span data-ttu-id="d80c5-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyPresentationCheckBox.](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)</span><span class="sxs-lookup"><span data-stu-id="d80c5-129">The following table shows the properties that are required when you create the [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).</span></span>

|<span data-ttu-id="d80c5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d80c5-130">Property</span></span>|<span data-ttu-id="d80c5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d80c5-131">Type</span></span>|<span data-ttu-id="d80c5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d80c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d80c5-133">label</span><span class="sxs-lookup"><span data-stu-id="d80c5-133">label</span></span>|<span data-ttu-id="d80c5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d80c5-134">String</span></span>|<span data-ttu-id="d80c5-135">Локализованная текстовая метка для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="d80c5-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="d80c5-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="d80c5-136">The default value is empty.</span></span> <span data-ttu-id="d80c5-137">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d80c5-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d80c5-138">id</span><span class="sxs-lookup"><span data-stu-id="d80c5-138">id</span></span>|<span data-ttu-id="d80c5-139">Строка</span><span class="sxs-lookup"><span data-stu-id="d80c5-139">String</span></span>|<span data-ttu-id="d80c5-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d80c5-140">Key of the entity.</span></span> <span data-ttu-id="d80c5-141">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d80c5-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d80c5-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d80c5-142">lastModifiedDateTime</span></span>|<span data-ttu-id="d80c5-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d80c5-143">DateTimeOffset</span></span>|<span data-ttu-id="d80c5-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d80c5-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="d80c5-145">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="d80c5-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="d80c5-146">defaultChecked</span><span class="sxs-lookup"><span data-stu-id="d80c5-146">defaultChecked</span></span>|<span data-ttu-id="d80c5-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="d80c5-147">Boolean</span></span>|<span data-ttu-id="d80c5-148">Значение по умолчанию для контрольного окна.</span><span class="sxs-lookup"><span data-stu-id="d80c5-148">Default value for the check box.</span></span> <span data-ttu-id="d80c5-149">Значение по умолчанию  false.</span><span class="sxs-lookup"><span data-stu-id="d80c5-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="d80c5-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d80c5-150">Response</span></span>
<span data-ttu-id="d80c5-151">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [GroupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d80c5-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d80c5-152">Пример</span><span class="sxs-lookup"><span data-stu-id="d80c5-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="d80c5-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="d80c5-153">Request</span></span>
<span data-ttu-id="d80c5-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d80c5-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "Label value",
  "defaultChecked": true
}
```

### <a name="response"></a><span data-ttu-id="d80c5-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="d80c5-155">Response</span></span>
<span data-ttu-id="d80c5-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d80c5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




