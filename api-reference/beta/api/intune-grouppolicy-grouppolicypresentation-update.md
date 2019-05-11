---
title: Обновление Граупполиципресентатион
description: Обновление свойств объекта Граупполиципресентатион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ea90fd410a905e57818e6c95253b218e36686dbb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33905072"
---
# <a name="update-grouppolicypresentation"></a><span data-ttu-id="10eb4-103">Обновление Граупполиципресентатион</span><span class="sxs-lookup"><span data-stu-id="10eb4-103">Update groupPolicyPresentation</span></span>

> <span data-ttu-id="10eb4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10eb4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10eb4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10eb4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10eb4-106">Обновление свойств объекта [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) .</span><span class="sxs-lookup"><span data-stu-id="10eb4-106">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10eb4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="10eb4-107">Prerequisites</span></span>
<span data-ttu-id="10eb4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10eb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10eb4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10eb4-110">Permission type</span></span>|<span data-ttu-id="10eb4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10eb4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10eb4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10eb4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10eb4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10eb4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="10eb4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10eb4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10eb4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10eb4-115">Not supported.</span></span>|
|<span data-ttu-id="10eb4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10eb4-116">Application</span></span>|<span data-ttu-id="10eb4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10eb4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10eb4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10eb4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="10eb4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10eb4-119">Request headers</span></span>
|<span data-ttu-id="10eb4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10eb4-120">Header</span></span>|<span data-ttu-id="10eb4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="10eb4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10eb4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10eb4-122">Authorization</span></span>|<span data-ttu-id="10eb4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10eb4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10eb4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="10eb4-124">Accept</span></span>|<span data-ttu-id="10eb4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10eb4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10eb4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10eb4-126">Request body</span></span>
<span data-ttu-id="10eb4-127">В тексте запроса добавьте представление объекта [Граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10eb4-127">In the request body, supply a JSON representation for the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

<span data-ttu-id="10eb4-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md).</span><span class="sxs-lookup"><span data-stu-id="10eb4-128">The following table shows the properties that are required when you create the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span></span>

|<span data-ttu-id="10eb4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="10eb4-129">Property</span></span>|<span data-ttu-id="10eb4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="10eb4-130">Type</span></span>|<span data-ttu-id="10eb4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="10eb4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10eb4-132">label</span><span class="sxs-lookup"><span data-stu-id="10eb4-132">label</span></span>|<span data-ttu-id="10eb4-133">Строка</span><span class="sxs-lookup"><span data-stu-id="10eb4-133">String</span></span>|<span data-ttu-id="10eb4-134">Локализованная текстовая подпись для любой сущности презентации.</span><span class="sxs-lookup"><span data-stu-id="10eb4-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="10eb4-135">По умолчанию это значение пусто.</span><span class="sxs-lookup"><span data-stu-id="10eb4-135">The default value is empty.</span></span>|
|<span data-ttu-id="10eb4-136">id</span><span class="sxs-lookup"><span data-stu-id="10eb4-136">id</span></span>|<span data-ttu-id="10eb4-137">Строка</span><span class="sxs-lookup"><span data-stu-id="10eb4-137">String</span></span>|<span data-ttu-id="10eb4-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="10eb4-138">Key of the entity.</span></span>|
|<span data-ttu-id="10eb4-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10eb4-139">lastModifiedDateTime</span></span>|<span data-ttu-id="10eb4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10eb4-140">DateTimeOffset</span></span>|<span data-ttu-id="10eb4-141">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="10eb4-141">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="10eb4-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="10eb4-142">Response</span></span>
<span data-ttu-id="10eb4-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10eb4-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10eb4-144">Пример</span><span class="sxs-lookup"><span data-stu-id="10eb4-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="10eb4-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="10eb4-145">Request</span></span>
<span data-ttu-id="10eb4-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10eb4-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="10eb4-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="10eb4-147">Response</span></span>
<span data-ttu-id="10eb4-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10eb4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




