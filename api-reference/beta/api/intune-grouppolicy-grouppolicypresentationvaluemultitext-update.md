---
title: Update groupPolicyPresentationValueMultiText
description: Обновление свойств объекта groupPolicyPresentationValueMultiText.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 91ba45eff86cb03c2ecdd1f84812d7791b3b9c79
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125949"
---
# <a name="update-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="3588d-103">Update groupPolicyPresentationValueMultiText</span><span class="sxs-lookup"><span data-stu-id="3588d-103">Update groupPolicyPresentationValueMultiText</span></span>

<span data-ttu-id="3588d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3588d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3588d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3588d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3588d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3588d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3588d-107">Обновление свойств объекта [groupPolicyPresentationValueMultiText.](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)</span><span class="sxs-lookup"><span data-stu-id="3588d-107">Update the properties of a [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3588d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3588d-108">Prerequisites</span></span>
<span data-ttu-id="3588d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3588d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3588d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3588d-111">Permission type</span></span>|<span data-ttu-id="3588d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3588d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3588d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3588d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3588d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3588d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3588d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3588d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3588d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3588d-116">Not supported.</span></span>|
|<span data-ttu-id="3588d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3588d-117">Application</span></span>|<span data-ttu-id="3588d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3588d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3588d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3588d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="3588d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3588d-120">Request headers</span></span>
|<span data-ttu-id="3588d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3588d-121">Header</span></span>|<span data-ttu-id="3588d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3588d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3588d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3588d-123">Authorization</span></span>|<span data-ttu-id="3588d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3588d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3588d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3588d-125">Accept</span></span>|<span data-ttu-id="3588d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3588d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3588d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3588d-127">Request body</span></span>
<span data-ttu-id="3588d-128">В тексте запроса поставляем представление JSON для [объекта groupPolicyPresentationValueMultiText.](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)</span><span class="sxs-lookup"><span data-stu-id="3588d-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

<span data-ttu-id="3588d-129">В следующей таблице показаны свойства, необходимые при создании [группыPolicyPresentationValueMultiText.](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)</span><span class="sxs-lookup"><span data-stu-id="3588d-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).</span></span>

|<span data-ttu-id="3588d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3588d-130">Property</span></span>|<span data-ttu-id="3588d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3588d-131">Type</span></span>|<span data-ttu-id="3588d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3588d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3588d-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3588d-133">lastModifiedDateTime</span></span>|<span data-ttu-id="3588d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3588d-134">DateTimeOffset</span></span>|<span data-ttu-id="3588d-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3588d-135">The date and time the object was last modified.</span></span> <span data-ttu-id="3588d-136">Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3588d-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="3588d-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3588d-137">createdDateTime</span></span>|<span data-ttu-id="3588d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3588d-138">DateTimeOffset</span></span>|<span data-ttu-id="3588d-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3588d-139">The date and time the object was created.</span></span> <span data-ttu-id="3588d-140">Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3588d-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="3588d-141">id</span><span class="sxs-lookup"><span data-stu-id="3588d-141">id</span></span>|<span data-ttu-id="3588d-142">Строка</span><span class="sxs-lookup"><span data-stu-id="3588d-142">String</span></span>|<span data-ttu-id="3588d-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3588d-143">Key of the entity.</span></span> <span data-ttu-id="3588d-144">Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="3588d-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="3588d-145">values</span><span class="sxs-lookup"><span data-stu-id="3588d-145">values</span></span>|<span data-ttu-id="3588d-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3588d-146">String collection</span></span>|<span data-ttu-id="3588d-147">Коллекция непустых строк для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="3588d-147">A collection of non-empty strings for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="3588d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="3588d-148">Response</span></span>
<span data-ttu-id="3588d-149">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [GroupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3588d-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3588d-150">Пример</span><span class="sxs-lookup"><span data-stu-id="3588d-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="3588d-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="3588d-151">Request</span></span>
<span data-ttu-id="3588d-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3588d-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3588d-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="3588d-153">Response</span></span>
<span data-ttu-id="3588d-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3588d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




