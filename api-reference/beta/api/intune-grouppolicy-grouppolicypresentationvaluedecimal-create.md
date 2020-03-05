---
title: Создание ГраупполиципресентатионвалуедеЦимал
description: Создание нового объекта ГраупполиципресентатионвалуедеЦимал.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e4ef33a1f72444fc951b4161bb46225d5d9750c1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42464213"
---
# <a name="create-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="24b40-103">Создание ГраупполиципресентатионвалуедеЦимал</span><span class="sxs-lookup"><span data-stu-id="24b40-103">Create groupPolicyPresentationValueDecimal</span></span>

<span data-ttu-id="24b40-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="24b40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24b40-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24b40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24b40-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24b40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24b40-107">Создание нового объекта [граупполиципресентатионвалуедеЦимал](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="24b40-107">Create a new [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24b40-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="24b40-108">Prerequisites</span></span>
<span data-ttu-id="24b40-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24b40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24b40-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24b40-111">Permission type</span></span>|<span data-ttu-id="24b40-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24b40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24b40-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24b40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24b40-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24b40-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="24b40-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24b40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24b40-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24b40-116">Not supported.</span></span>|
|<span data-ttu-id="24b40-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24b40-117">Application</span></span>|<span data-ttu-id="24b40-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24b40-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24b40-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24b40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="24b40-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="24b40-120">Request headers</span></span>
|<span data-ttu-id="24b40-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24b40-121">Header</span></span>|<span data-ttu-id="24b40-122">Значение</span><span class="sxs-lookup"><span data-stu-id="24b40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24b40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="24b40-123">Authorization</span></span>|<span data-ttu-id="24b40-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24b40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24b40-125">Accept</span><span class="sxs-lookup"><span data-stu-id="24b40-125">Accept</span></span>|<span data-ttu-id="24b40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24b40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24b40-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24b40-127">Request body</span></span>
<span data-ttu-id="24b40-128">В тексте запроса добавьте представление объекта ГраупполиципресентатионвалуедеЦимал в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24b40-128">In the request body, supply a JSON representation for the groupPolicyPresentationValueDecimal object.</span></span>

<span data-ttu-id="24b40-129">В следующей таблице приведены свойства, необходимые при создании ГраупполиципресентатионвалуедеЦимал.</span><span class="sxs-lookup"><span data-stu-id="24b40-129">The following table shows the properties that are required when you create the groupPolicyPresentationValueDecimal.</span></span>

|<span data-ttu-id="24b40-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="24b40-130">Property</span></span>|<span data-ttu-id="24b40-131">Тип</span><span class="sxs-lookup"><span data-stu-id="24b40-131">Type</span></span>|<span data-ttu-id="24b40-132">Описание</span><span class="sxs-lookup"><span data-stu-id="24b40-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24b40-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24b40-133">lastModifiedDateTime</span></span>|<span data-ttu-id="24b40-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24b40-134">DateTimeOffset</span></span>|<span data-ttu-id="24b40-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="24b40-135">The date and time the object was last modified.</span></span> <span data-ttu-id="24b40-136">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="24b40-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="24b40-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24b40-137">createdDateTime</span></span>|<span data-ttu-id="24b40-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24b40-138">DateTimeOffset</span></span>|<span data-ttu-id="24b40-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="24b40-139">The date and time the object was created.</span></span> <span data-ttu-id="24b40-140">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="24b40-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="24b40-141">id</span><span class="sxs-lookup"><span data-stu-id="24b40-141">id</span></span>|<span data-ttu-id="24b40-142">String</span><span class="sxs-lookup"><span data-stu-id="24b40-142">String</span></span>|<span data-ttu-id="24b40-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="24b40-143">Key of the entity.</span></span> <span data-ttu-id="24b40-144">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="24b40-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="24b40-145">значение</span><span class="sxs-lookup"><span data-stu-id="24b40-145">value</span></span>|<span data-ttu-id="24b40-146">Int64</span><span class="sxs-lookup"><span data-stu-id="24b40-146">Int64</span></span>|<span data-ttu-id="24b40-147">Целое значение без знака для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="24b40-147">An unsigned integer value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="24b40-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="24b40-148">Response</span></span>
<span data-ttu-id="24b40-149">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионвалуедеЦимал](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24b40-149">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24b40-150">Пример</span><span class="sxs-lookup"><span data-stu-id="24b40-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="24b40-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="24b40-151">Request</span></span>
<span data-ttu-id="24b40-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24b40-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="24b40-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="24b40-153">Response</span></span>
<span data-ttu-id="24b40-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24b40-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 264

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8821bede-bede-8821-debe-2188debe2188",
  "value": 5
}
```





