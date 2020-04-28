---
title: Обновление Граупполиципресентатион
description: Обновление свойств объекта Граупполиципресентатион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6532615d0e2228d1caec4cf784a7d139b9323e13
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43375499"
---
# <a name="update-grouppolicypresentation"></a><span data-ttu-id="d3e2f-103">Обновление Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="d3e2f-103">Update groupPolicyPresentation</span></span>

<span data-ttu-id="d3e2f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3e2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3e2f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3e2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3e2f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3e2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3e2f-107">Обновление свойств объекта [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="d3e2f-107">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3e2f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d3e2f-108">Prerequisites</span></span>
<span data-ttu-id="d3e2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3e2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3e2f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3e2f-111">Permission type</span></span>|<span data-ttu-id="d3e2f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3e2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3e2f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3e2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3e2f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3e2f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3e2f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3e2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3e2f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3e2f-116">Not supported.</span></span>|
|<span data-ttu-id="d3e2f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3e2f-117">Application</span></span>|<span data-ttu-id="d3e2f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3e2f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3e2f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3e2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="d3e2f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d3e2f-120">Request headers</span></span>
|<span data-ttu-id="d3e2f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3e2f-121">Header</span></span>|<span data-ttu-id="d3e2f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d3e2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3e2f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3e2f-123">Authorization</span></span>|<span data-ttu-id="d3e2f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3e2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3e2f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d3e2f-125">Accept</span></span>|<span data-ttu-id="d3e2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3e2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3e2f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d3e2f-127">Request body</span></span>
<span data-ttu-id="d3e2f-128">В тексте запроса добавьте представление объекта [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3e2f-128">In the request body, supply a JSON representation for the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

<span data-ttu-id="d3e2f-129">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md).</span><span class="sxs-lookup"><span data-stu-id="d3e2f-129">The following table shows the properties that are required when you create the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span></span>

|<span data-ttu-id="d3e2f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3e2f-130">Property</span></span>|<span data-ttu-id="d3e2f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d3e2f-131">Type</span></span>|<span data-ttu-id="d3e2f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d3e2f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3e2f-133">label</span><span class="sxs-lookup"><span data-stu-id="d3e2f-133">label</span></span>|<span data-ttu-id="d3e2f-134">String</span><span class="sxs-lookup"><span data-stu-id="d3e2f-134">String</span></span>|<span data-ttu-id="d3e2f-135">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="d3e2f-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="d3e2f-136">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="d3e2f-136">The default value is empty.</span></span>|
|<span data-ttu-id="d3e2f-137">id</span><span class="sxs-lookup"><span data-stu-id="d3e2f-137">id</span></span>|<span data-ttu-id="d3e2f-138">String</span><span class="sxs-lookup"><span data-stu-id="d3e2f-138">String</span></span>|<span data-ttu-id="d3e2f-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d3e2f-139">Key of the entity.</span></span>|
|<span data-ttu-id="d3e2f-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3e2f-140">lastModifiedDateTime</span></span>|<span data-ttu-id="d3e2f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3e2f-141">DateTimeOffset</span></span>|<span data-ttu-id="d3e2f-142">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d3e2f-142">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="d3e2f-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="d3e2f-143">Response</span></span>
<span data-ttu-id="d3e2f-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3e2f-144">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3e2f-145">Пример</span><span class="sxs-lookup"><span data-stu-id="d3e2f-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3e2f-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3e2f-146">Request</span></span>
<span data-ttu-id="d3e2f-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3e2f-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="d3e2f-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3e2f-148">Response</span></span>
<span data-ttu-id="d3e2f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3e2f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



