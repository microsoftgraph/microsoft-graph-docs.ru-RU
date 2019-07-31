---
title: Обновление ГраупполиципресентатионвалуедеЦимал
description: Обновление свойств объекта ГраупполиципресентатионвалуедеЦимал.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 075e4f55a919c37882198db541dd4d877ba8df86
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35989184"
---
# <a name="update-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="300f5-103">Обновление ГраупполиципресентатионвалуедеЦимал</span><span class="sxs-lookup"><span data-stu-id="300f5-103">Update groupPolicyPresentationValueDecimal</span></span>

> <span data-ttu-id="300f5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="300f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="300f5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="300f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="300f5-106">Обновление свойств объекта [граупполиципресентатионвалуедеЦимал](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="300f5-106">Update the properties of a [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="300f5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="300f5-107">Prerequisites</span></span>
<span data-ttu-id="300f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="300f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="300f5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="300f5-110">Permission type</span></span>|<span data-ttu-id="300f5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="300f5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="300f5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="300f5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="300f5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="300f5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="300f5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="300f5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="300f5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="300f5-115">Not supported.</span></span>|
|<span data-ttu-id="300f5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="300f5-116">Application</span></span>|<span data-ttu-id="300f5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="300f5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="300f5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="300f5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="300f5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="300f5-119">Request headers</span></span>
|<span data-ttu-id="300f5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="300f5-120">Header</span></span>|<span data-ttu-id="300f5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="300f5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="300f5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="300f5-122">Authorization</span></span>|<span data-ttu-id="300f5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="300f5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="300f5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="300f5-124">Accept</span></span>|<span data-ttu-id="300f5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="300f5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="300f5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="300f5-126">Request body</span></span>
<span data-ttu-id="300f5-127">В тексте запроса добавьте представление объекта [граупполиципресентатионвалуедеЦимал](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="300f5-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

<span data-ttu-id="300f5-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионвалуедеЦимал](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md).</span><span class="sxs-lookup"><span data-stu-id="300f5-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md).</span></span>

|<span data-ttu-id="300f5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="300f5-129">Property</span></span>|<span data-ttu-id="300f5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="300f5-130">Type</span></span>|<span data-ttu-id="300f5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="300f5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="300f5-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="300f5-132">lastModifiedDateTime</span></span>|<span data-ttu-id="300f5-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="300f5-133">DateTimeOffset</span></span>|<span data-ttu-id="300f5-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="300f5-134">The date and time the object was last modified.</span></span> <span data-ttu-id="300f5-135">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="300f5-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="300f5-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="300f5-136">createdDateTime</span></span>|<span data-ttu-id="300f5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="300f5-137">DateTimeOffset</span></span>|<span data-ttu-id="300f5-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="300f5-138">The date and time the object was created.</span></span> <span data-ttu-id="300f5-139">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="300f5-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="300f5-140">id</span><span class="sxs-lookup"><span data-stu-id="300f5-140">id</span></span>|<span data-ttu-id="300f5-141">String</span><span class="sxs-lookup"><span data-stu-id="300f5-141">String</span></span>|<span data-ttu-id="300f5-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="300f5-142">Key of the entity.</span></span> <span data-ttu-id="300f5-143">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="300f5-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="300f5-144">значение</span><span class="sxs-lookup"><span data-stu-id="300f5-144">value</span></span>|<span data-ttu-id="300f5-145">Int64</span><span class="sxs-lookup"><span data-stu-id="300f5-145">Int64</span></span>|<span data-ttu-id="300f5-146">Целое значение без знака для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="300f5-146">An unsigned integer value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="300f5-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="300f5-147">Response</span></span>
<span data-ttu-id="300f5-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионвалуедеЦимал](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="300f5-148">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="300f5-149">Пример</span><span class="sxs-lookup"><span data-stu-id="300f5-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="300f5-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="300f5-150">Request</span></span>
<span data-ttu-id="300f5-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="300f5-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="300f5-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="300f5-152">Response</span></span>
<span data-ttu-id="300f5-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="300f5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





