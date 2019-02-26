---
title: Создание Граупполиципресентатионвалуемултитекст
description: Создание нового объекта Граупполиципресентатионвалуемултитекст.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 81e6a4068f9daba403053ee2185c4474acee8b01
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144508"
---
# <a name="create-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="c5fde-103">Создание Граупполиципресентатионвалуемултитекст</span><span class="sxs-lookup"><span data-stu-id="c5fde-103">Create groupPolicyPresentationValueMultiText</span></span>

> <span data-ttu-id="c5fde-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5fde-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5fde-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5fde-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5fde-106">Создание нового объекта [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .</span><span class="sxs-lookup"><span data-stu-id="c5fde-106">Create a new [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5fde-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c5fde-107">Prerequisites</span></span>
<span data-ttu-id="c5fde-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5fde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c5fde-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5fde-110">Permission type</span></span>|<span data-ttu-id="c5fde-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5fde-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5fde-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5fde-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c5fde-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5fde-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c5fde-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5fde-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5fde-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5fde-115">Not supported.</span></span>|
|<span data-ttu-id="c5fde-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5fde-116">Application</span></span>|<span data-ttu-id="c5fde-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5fde-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5fde-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5fde-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="c5fde-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5fde-119">Request headers</span></span>
|<span data-ttu-id="c5fde-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5fde-120">Header</span></span>|<span data-ttu-id="c5fde-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c5fde-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5fde-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5fde-122">Authorization</span></span>|<span data-ttu-id="c5fde-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c5fde-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5fde-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c5fde-124">Accept</span></span>|<span data-ttu-id="c5fde-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c5fde-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5fde-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5fde-126">Request body</span></span>
<span data-ttu-id="c5fde-127">В тексте запроса добавьте представление объекта Граупполиципресентатионвалуемултитекст в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5fde-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueMultiText object.</span></span>

<span data-ttu-id="c5fde-128">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионвалуемултитекст.</span><span class="sxs-lookup"><span data-stu-id="c5fde-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueMultiText.</span></span>

|<span data-ttu-id="c5fde-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5fde-129">Property</span></span>|<span data-ttu-id="c5fde-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c5fde-130">Type</span></span>|<span data-ttu-id="c5fde-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c5fde-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5fde-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5fde-132">lastModifiedDateTime</span></span>|<span data-ttu-id="c5fde-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5fde-133">DateTimeOffset</span></span>|<span data-ttu-id="c5fde-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c5fde-134">The date and time the object was last modified.</span></span> <span data-ttu-id="c5fde-135">НаСледуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="c5fde-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="c5fde-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5fde-136">createdDateTime</span></span>|<span data-ttu-id="c5fde-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5fde-137">DateTimeOffset</span></span>|<span data-ttu-id="c5fde-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c5fde-138">The date and time the object was created.</span></span> <span data-ttu-id="c5fde-139">НаСледуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="c5fde-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="c5fde-140">id</span><span class="sxs-lookup"><span data-stu-id="c5fde-140">id</span></span>|<span data-ttu-id="c5fde-141">String</span><span class="sxs-lookup"><span data-stu-id="c5fde-141">String</span></span>|<span data-ttu-id="c5fde-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c5fde-142">Key of the entity.</span></span> <span data-ttu-id="c5fde-143">НаСледуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="c5fde-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="c5fde-144">values</span><span class="sxs-lookup"><span data-stu-id="c5fde-144">values</span></span>|<span data-ttu-id="c5fde-145">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c5fde-145">String collection</span></span>|<span data-ttu-id="c5fde-146">Коллекция непустых строк для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="c5fde-146">A collection of non-empty strings for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="c5fde-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5fde-147">Response</span></span>
<span data-ttu-id="c5fde-148">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионвалуемултитекст](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5fde-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5fde-149">Пример</span><span class="sxs-lookup"><span data-stu-id="c5fde-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5fde-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5fde-150">Request</span></span>
<span data-ttu-id="c5fde-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5fde-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c5fde-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5fde-152">Response</span></span>
<span data-ttu-id="c5fde-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c5fde-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




