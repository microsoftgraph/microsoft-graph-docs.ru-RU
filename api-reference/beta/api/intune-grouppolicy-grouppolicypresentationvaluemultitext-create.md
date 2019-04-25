---
title: Создание Граупполиципресентатионвалуемултитекст
description: Создание нового объекта Граупполиципресентатионвалуемултитекст.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6ea3a2e745049292979c45bd1a2af2137bd30b6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32530580"
---
# <a name="create-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="9ae0c-103">Создание Граупполиципресентатионвалуемултитекст</span><span class="sxs-lookup"><span data-stu-id="9ae0c-103">Create groupPolicyPresentationValueMultiText</span></span>

> <span data-ttu-id="9ae0c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ae0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ae0c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ae0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ae0c-106">Создание нового объекта [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .</span><span class="sxs-lookup"><span data-stu-id="9ae0c-106">Create a new [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ae0c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9ae0c-107">Prerequisites</span></span>
<span data-ttu-id="9ae0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ae0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ae0c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ae0c-110">Permission type</span></span>|<span data-ttu-id="9ae0c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ae0c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ae0c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ae0c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ae0c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ae0c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9ae0c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ae0c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ae0c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ae0c-115">Not supported.</span></span>|
|<span data-ttu-id="9ae0c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ae0c-116">Application</span></span>|<span data-ttu-id="9ae0c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ae0c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ae0c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ae0c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="9ae0c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ae0c-119">Request headers</span></span>
|<span data-ttu-id="9ae0c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ae0c-120">Header</span></span>|<span data-ttu-id="9ae0c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9ae0c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ae0c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ae0c-122">Authorization</span></span>|<span data-ttu-id="9ae0c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ae0c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ae0c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9ae0c-124">Accept</span></span>|<span data-ttu-id="9ae0c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9ae0c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ae0c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ae0c-126">Request body</span></span>
<span data-ttu-id="9ae0c-127">В тексте запроса добавьте представление объекта Граупполиципресентатионвалуемултитекст в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ae0c-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueMultiText object.</span></span>

<span data-ttu-id="9ae0c-128">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионвалуемултитекст.</span><span class="sxs-lookup"><span data-stu-id="9ae0c-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueMultiText.</span></span>

|<span data-ttu-id="9ae0c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ae0c-129">Property</span></span>|<span data-ttu-id="9ae0c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9ae0c-130">Type</span></span>|<span data-ttu-id="9ae0c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9ae0c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ae0c-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ae0c-132">lastModifiedDateTime</span></span>|<span data-ttu-id="9ae0c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ae0c-133">DateTimeOffset</span></span>|<span data-ttu-id="9ae0c-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9ae0c-134">The date and time the object was last modified.</span></span> <span data-ttu-id="9ae0c-135">НаСледуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9ae0c-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="9ae0c-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ae0c-136">createdDateTime</span></span>|<span data-ttu-id="9ae0c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ae0c-137">DateTimeOffset</span></span>|<span data-ttu-id="9ae0c-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9ae0c-138">The date and time the object was created.</span></span> <span data-ttu-id="9ae0c-139">НаСледуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9ae0c-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="9ae0c-140">id</span><span class="sxs-lookup"><span data-stu-id="9ae0c-140">id</span></span>|<span data-ttu-id="9ae0c-141">String</span><span class="sxs-lookup"><span data-stu-id="9ae0c-141">String</span></span>|<span data-ttu-id="9ae0c-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9ae0c-142">Key of the entity.</span></span> <span data-ttu-id="9ae0c-143">НаСледуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9ae0c-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="9ae0c-144">values</span><span class="sxs-lookup"><span data-stu-id="9ae0c-144">values</span></span>|<span data-ttu-id="9ae0c-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9ae0c-145">String collection</span></span>|<span data-ttu-id="9ae0c-146">Коллекция непустых строк для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="9ae0c-146">A collection of non-empty strings for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="9ae0c-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ae0c-147">Response</span></span>
<span data-ttu-id="9ae0c-148">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ae0c-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ae0c-149">Пример</span><span class="sxs-lookup"><span data-stu-id="9ae0c-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ae0c-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ae0c-150">Request</span></span>
<span data-ttu-id="9ae0c-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ae0c-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "values": [
    "Values value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="9ae0c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ae0c-152">Response</span></span>
<span data-ttu-id="9ae0c-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ae0c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





