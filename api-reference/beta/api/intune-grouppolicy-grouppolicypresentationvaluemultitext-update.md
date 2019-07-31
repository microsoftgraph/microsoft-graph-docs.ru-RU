---
title: Обновление Граупполиципресентатионвалуемултитекст
description: Обновление свойств объекта Граупполиципресентатионвалуемултитекст.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8adb65cdcc06d6c8924e787c56e29bddd0d71ff1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995127"
---
# <a name="update-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="97ad3-103">Обновление Граупполиципресентатионвалуемултитекст</span><span class="sxs-lookup"><span data-stu-id="97ad3-103">Update groupPolicyPresentationValueMultiText</span></span>

> <span data-ttu-id="97ad3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97ad3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97ad3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97ad3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97ad3-106">Обновление свойств объекта [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .</span><span class="sxs-lookup"><span data-stu-id="97ad3-106">Update the properties of a [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97ad3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="97ad3-107">Prerequisites</span></span>
<span data-ttu-id="97ad3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97ad3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97ad3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97ad3-110">Permission type</span></span>|<span data-ttu-id="97ad3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="97ad3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97ad3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97ad3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97ad3-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97ad3-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="97ad3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97ad3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97ad3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97ad3-115">Not supported.</span></span>|
|<span data-ttu-id="97ad3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97ad3-116">Application</span></span>|<span data-ttu-id="97ad3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97ad3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97ad3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97ad3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="97ad3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97ad3-119">Request headers</span></span>
|<span data-ttu-id="97ad3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97ad3-120">Header</span></span>|<span data-ttu-id="97ad3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="97ad3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97ad3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97ad3-122">Authorization</span></span>|<span data-ttu-id="97ad3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97ad3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97ad3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="97ad3-124">Accept</span></span>|<span data-ttu-id="97ad3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97ad3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97ad3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="97ad3-126">Request body</span></span>
<span data-ttu-id="97ad3-127">В тексте запроса добавьте представление объекта [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97ad3-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

<span data-ttu-id="97ad3-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span><span class="sxs-lookup"><span data-stu-id="97ad3-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span></span>

|<span data-ttu-id="97ad3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="97ad3-129">Property</span></span>|<span data-ttu-id="97ad3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="97ad3-130">Type</span></span>|<span data-ttu-id="97ad3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="97ad3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97ad3-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97ad3-132">lastModifiedDateTime</span></span>|<span data-ttu-id="97ad3-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97ad3-133">DateTimeOffset</span></span>|<span data-ttu-id="97ad3-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="97ad3-134">The date and time the object was last modified.</span></span> <span data-ttu-id="97ad3-135">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="97ad3-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="97ad3-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97ad3-136">createdDateTime</span></span>|<span data-ttu-id="97ad3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97ad3-137">DateTimeOffset</span></span>|<span data-ttu-id="97ad3-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="97ad3-138">The date and time the object was created.</span></span> <span data-ttu-id="97ad3-139">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="97ad3-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="97ad3-140">id</span><span class="sxs-lookup"><span data-stu-id="97ad3-140">id</span></span>|<span data-ttu-id="97ad3-141">String</span><span class="sxs-lookup"><span data-stu-id="97ad3-141">String</span></span>|<span data-ttu-id="97ad3-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="97ad3-142">Key of the entity.</span></span> <span data-ttu-id="97ad3-143">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="97ad3-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="97ad3-144">values</span><span class="sxs-lookup"><span data-stu-id="97ad3-144">values</span></span>|<span data-ttu-id="97ad3-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="97ad3-145">String collection</span></span>|<span data-ttu-id="97ad3-146">Коллекция непустых строк для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="97ad3-146">A collection of non-empty strings for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="97ad3-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="97ad3-147">Response</span></span>
<span data-ttu-id="97ad3-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="97ad3-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97ad3-149">Пример</span><span class="sxs-lookup"><span data-stu-id="97ad3-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="97ad3-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="97ad3-150">Request</span></span>
<span data-ttu-id="97ad3-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97ad3-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "values": [
    "Values value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="97ad3-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="97ad3-152">Response</span></span>
<span data-ttu-id="97ad3-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97ad3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 292

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "5156903b-903b-5156-3b90-56513b905651",
  "values": [
    "Values value"
  ]
}
```





