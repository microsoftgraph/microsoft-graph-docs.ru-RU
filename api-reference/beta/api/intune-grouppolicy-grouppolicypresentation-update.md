---
title: Обновление groupPolicyPresentation
description: Обновление свойств объекта groupPolicyPresentation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da0b72b6818672c005c76170264f6749e3fab9bb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142018"
---
# <a name="update-grouppolicypresentation"></a><span data-ttu-id="b99f2-103">Обновление groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="b99f2-103">Update groupPolicyPresentation</span></span>

<span data-ttu-id="b99f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b99f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b99f2-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b99f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b99f2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b99f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b99f2-107">Обновление свойств объекта [groupPolicyPresentation.](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b99f2-107">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b99f2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b99f2-108">Prerequisites</span></span>
<span data-ttu-id="b99f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b99f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b99f2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b99f2-111">Permission type</span></span>|<span data-ttu-id="b99f2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b99f2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b99f2-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b99f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b99f2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b99f2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b99f2-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b99f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b99f2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b99f2-116">Not supported.</span></span>|
|<span data-ttu-id="b99f2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b99f2-117">Application</span></span>|<span data-ttu-id="b99f2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b99f2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b99f2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b99f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="b99f2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b99f2-120">Request headers</span></span>
|<span data-ttu-id="b99f2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b99f2-121">Header</span></span>|<span data-ttu-id="b99f2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b99f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b99f2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b99f2-123">Authorization</span></span>|<span data-ttu-id="b99f2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b99f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b99f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b99f2-125">Accept</span></span>|<span data-ttu-id="b99f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b99f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b99f2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b99f2-127">Request body</span></span>
<span data-ttu-id="b99f2-128">В теле запроса поставляем представление JSON для [объекта groupPolicyPresentation.](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b99f2-128">In the request body, supply a JSON representation for the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

<span data-ttu-id="b99f2-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyPresentation.](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="b99f2-129">The following table shows the properties that are required when you create the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span></span>

|<span data-ttu-id="b99f2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b99f2-130">Property</span></span>|<span data-ttu-id="b99f2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b99f2-131">Type</span></span>|<span data-ttu-id="b99f2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b99f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b99f2-133">label</span><span class="sxs-lookup"><span data-stu-id="b99f2-133">label</span></span>|<span data-ttu-id="b99f2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b99f2-134">String</span></span>|<span data-ttu-id="b99f2-135">Локализованная текстовая метка для любого объекта презентации.</span><span class="sxs-lookup"><span data-stu-id="b99f2-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="b99f2-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="b99f2-136">The default value is empty.</span></span>|
|<span data-ttu-id="b99f2-137">id</span><span class="sxs-lookup"><span data-stu-id="b99f2-137">id</span></span>|<span data-ttu-id="b99f2-138">Строка</span><span class="sxs-lookup"><span data-stu-id="b99f2-138">String</span></span>|<span data-ttu-id="b99f2-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b99f2-139">Key of the entity.</span></span>|
|<span data-ttu-id="b99f2-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b99f2-140">lastModifiedDateTime</span></span>|<span data-ttu-id="b99f2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b99f2-141">DateTimeOffset</span></span>|<span data-ttu-id="b99f2-142">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b99f2-142">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="b99f2-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b99f2-143">Response</span></span>
<span data-ttu-id="b99f2-144">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b99f2-144">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b99f2-145">Пример</span><span class="sxs-lookup"><span data-stu-id="b99f2-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="b99f2-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="b99f2-146">Request</span></span>
<span data-ttu-id="b99f2-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b99f2-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="b99f2-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="b99f2-148">Response</span></span>
<span data-ttu-id="b99f2-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b99f2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 205

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value",
  "id": "a33caa6a-aa6a-a33c-6aaa-3ca36aaa3ca3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




