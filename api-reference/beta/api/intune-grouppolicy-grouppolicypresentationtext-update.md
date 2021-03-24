---
title: Update groupPolicyPresentationText
description: Обновление свойств объекта groupPolicyPresentationText.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: edab3145c9618c0c298cd1502c6aed5965394713
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149438"
---
# <a name="update-grouppolicypresentationtext"></a><span data-ttu-id="66ca7-103">Update groupPolicyPresentationText</span><span class="sxs-lookup"><span data-stu-id="66ca7-103">Update groupPolicyPresentationText</span></span>

<span data-ttu-id="66ca7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66ca7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66ca7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66ca7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66ca7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66ca7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66ca7-107">Обновление свойств объекта [groupPolicyPresentationText.](../resources/intune-grouppolicy-grouppolicypresentationtext.md)</span><span class="sxs-lookup"><span data-stu-id="66ca7-107">Update the properties of a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66ca7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="66ca7-108">Prerequisites</span></span>
<span data-ttu-id="66ca7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66ca7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66ca7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66ca7-111">Permission type</span></span>|<span data-ttu-id="66ca7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66ca7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66ca7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66ca7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66ca7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66ca7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="66ca7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66ca7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66ca7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66ca7-116">Not supported.</span></span>|
|<span data-ttu-id="66ca7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="66ca7-117">Application</span></span>|<span data-ttu-id="66ca7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66ca7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66ca7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66ca7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="66ca7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="66ca7-120">Request headers</span></span>
|<span data-ttu-id="66ca7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="66ca7-121">Header</span></span>|<span data-ttu-id="66ca7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="66ca7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66ca7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66ca7-123">Authorization</span></span>|<span data-ttu-id="66ca7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66ca7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66ca7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="66ca7-125">Accept</span></span>|<span data-ttu-id="66ca7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="66ca7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66ca7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66ca7-127">Request body</span></span>
<span data-ttu-id="66ca7-128">В тексте запроса поставляем представление JSON для [объекта GroupPolicyPresentationText.](../resources/intune-grouppolicy-grouppolicypresentationtext.md)</span><span class="sxs-lookup"><span data-stu-id="66ca7-128">In the request body, supply a JSON representation for the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

<span data-ttu-id="66ca7-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyPresentationText.](../resources/intune-grouppolicy-grouppolicypresentationtext.md)</span><span class="sxs-lookup"><span data-stu-id="66ca7-129">The following table shows the properties that are required when you create the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md).</span></span>

|<span data-ttu-id="66ca7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="66ca7-130">Property</span></span>|<span data-ttu-id="66ca7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="66ca7-131">Type</span></span>|<span data-ttu-id="66ca7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="66ca7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66ca7-133">label</span><span class="sxs-lookup"><span data-stu-id="66ca7-133">label</span></span>|<span data-ttu-id="66ca7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="66ca7-134">String</span></span>|<span data-ttu-id="66ca7-135">Локализованная текстовая метка для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="66ca7-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="66ca7-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="66ca7-136">The default value is empty.</span></span> <span data-ttu-id="66ca7-137">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="66ca7-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="66ca7-138">id</span><span class="sxs-lookup"><span data-stu-id="66ca7-138">id</span></span>|<span data-ttu-id="66ca7-139">Строка</span><span class="sxs-lookup"><span data-stu-id="66ca7-139">String</span></span>|<span data-ttu-id="66ca7-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="66ca7-140">Key of the entity.</span></span> <span data-ttu-id="66ca7-141">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="66ca7-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="66ca7-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66ca7-142">lastModifiedDateTime</span></span>|<span data-ttu-id="66ca7-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66ca7-143">DateTimeOffset</span></span>|<span data-ttu-id="66ca7-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="66ca7-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="66ca7-145">Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="66ca7-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="66ca7-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="66ca7-146">Response</span></span>
<span data-ttu-id="66ca7-147">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="66ca7-147">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66ca7-148">Пример</span><span class="sxs-lookup"><span data-stu-id="66ca7-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="66ca7-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="66ca7-149">Request</span></span>
<span data-ttu-id="66ca7-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66ca7-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="66ca7-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="66ca7-151">Response</span></span>
<span data-ttu-id="66ca7-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66ca7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




