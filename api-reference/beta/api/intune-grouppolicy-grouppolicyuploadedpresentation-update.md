---
title: Обновление Граупполициуплоадедпресентатион
description: Обновление свойств объекта Граупполициуплоадедпресентатион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e62c1afd314059d5ea05f8d6fe61a384d2984a8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49224489"
---
# <a name="update-grouppolicyuploadedpresentation"></a><span data-ttu-id="ce763-103">Обновление Граупполициуплоадедпресентатион</span><span class="sxs-lookup"><span data-stu-id="ce763-103">Update groupPolicyUploadedPresentation</span></span>

<span data-ttu-id="ce763-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce763-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce763-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce763-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce763-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce763-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce763-107">Обновление свойств объекта [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="ce763-107">Update the properties of a [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce763-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ce763-108">Prerequisites</span></span>
<span data-ttu-id="ce763-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce763-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce763-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce763-111">Permission type</span></span>|<span data-ttu-id="ce763-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce763-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce763-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce763-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce763-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce763-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce763-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce763-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce763-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce763-116">Not supported.</span></span>|
|<span data-ttu-id="ce763-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ce763-117">Application</span></span>|<span data-ttu-id="ce763-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce763-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce763-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce763-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="ce763-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ce763-120">Request headers</span></span>
|<span data-ttu-id="ce763-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce763-121">Header</span></span>|<span data-ttu-id="ce763-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ce763-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce763-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce763-123">Authorization</span></span>|<span data-ttu-id="ce763-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce763-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce763-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ce763-125">Accept</span></span>|<span data-ttu-id="ce763-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce763-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce763-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce763-127">Request body</span></span>
<span data-ttu-id="ce763-128">В тексте запроса добавьте представление объекта [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce763-128">In the request body, supply a JSON representation for the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object.</span></span>

<span data-ttu-id="ce763-129">В следующей таблице приведены свойства, необходимые при создании [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md).</span><span class="sxs-lookup"><span data-stu-id="ce763-129">The following table shows the properties that are required when you create the [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md).</span></span>

|<span data-ttu-id="ce763-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce763-130">Property</span></span>|<span data-ttu-id="ce763-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ce763-131">Type</span></span>|<span data-ttu-id="ce763-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ce763-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce763-133">label</span><span class="sxs-lookup"><span data-stu-id="ce763-133">label</span></span>|<span data-ttu-id="ce763-134">String</span><span class="sxs-lookup"><span data-stu-id="ce763-134">String</span></span>|<span data-ttu-id="ce763-135">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="ce763-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="ce763-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="ce763-136">The default value is empty.</span></span> <span data-ttu-id="ce763-137">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ce763-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ce763-138">id</span><span class="sxs-lookup"><span data-stu-id="ce763-138">id</span></span>|<span data-ttu-id="ce763-139">String</span><span class="sxs-lookup"><span data-stu-id="ce763-139">String</span></span>|<span data-ttu-id="ce763-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ce763-140">Key of the entity.</span></span> <span data-ttu-id="ce763-141">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ce763-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="ce763-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce763-142">lastModifiedDateTime</span></span>|<span data-ttu-id="ce763-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce763-143">DateTimeOffset</span></span>|<span data-ttu-id="ce763-144">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ce763-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="ce763-145">Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="ce763-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ce763-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce763-146">Response</span></span>
<span data-ttu-id="ce763-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ce763-147">If successful, this method returns a `200 OK` response code and an updated [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce763-148">Пример</span><span class="sxs-lookup"><span data-stu-id="ce763-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce763-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce763-149">Request</span></span>
<span data-ttu-id="ce763-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce763-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="ce763-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce763-151">Response</span></span>
<span data-ttu-id="ce763-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce763-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 213

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
  "label": "Label value",
  "id": "b9f611e8-11e8-b9f6-e811-f6b9e811f6b9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




