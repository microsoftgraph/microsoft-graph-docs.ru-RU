---
title: Создание ГраупполиципресентатионвалуедеЦимал
description: Создание нового объекта ГраупполиципресентатионвалуедеЦимал.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e6f25accf5a348daf95a6ee90dafc8826aafbc7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974750"
---
# <a name="create-grouppolicypresentationvaluedecimal"></a><span data-ttu-id="2b9be-103">Создание ГраупполиципресентатионвалуедеЦимал</span><span class="sxs-lookup"><span data-stu-id="2b9be-103">Create groupPolicyPresentationValueDecimal</span></span>

> <span data-ttu-id="2b9be-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b9be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b9be-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b9be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b9be-106">Создание нового объекта [граупполиципресентатионвалуедеЦимал](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="2b9be-106">Create a new [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b9be-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2b9be-107">Prerequisites</span></span>
<span data-ttu-id="2b9be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b9be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b9be-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b9be-110">Permission type</span></span>|<span data-ttu-id="2b9be-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b9be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b9be-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b9be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2b9be-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b9be-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2b9be-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b9be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b9be-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b9be-115">Not supported.</span></span>|
|<span data-ttu-id="2b9be-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b9be-116">Application</span></span>|<span data-ttu-id="2b9be-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b9be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b9be-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b9be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="2b9be-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b9be-119">Request headers</span></span>
|<span data-ttu-id="2b9be-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b9be-120">Header</span></span>|<span data-ttu-id="2b9be-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2b9be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b9be-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b9be-122">Authorization</span></span>|<span data-ttu-id="2b9be-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b9be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b9be-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2b9be-124">Accept</span></span>|<span data-ttu-id="2b9be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2b9be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b9be-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b9be-126">Request body</span></span>
<span data-ttu-id="2b9be-127">В тексте запроса добавьте представление объекта ГраупполиципресентатионвалуедеЦимал в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b9be-127">In the request body, supply a JSON representation for the groupPolicyPresentationValueDecimal object.</span></span>

<span data-ttu-id="2b9be-128">В следующей таблице приведены свойства, необходимые при создании ГраупполиципресентатионвалуедеЦимал.</span><span class="sxs-lookup"><span data-stu-id="2b9be-128">The following table shows the properties that are required when you create the groupPolicyPresentationValueDecimal.</span></span>

|<span data-ttu-id="2b9be-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b9be-129">Property</span></span>|<span data-ttu-id="2b9be-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2b9be-130">Type</span></span>|<span data-ttu-id="2b9be-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2b9be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b9be-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b9be-132">lastModifiedDateTime</span></span>|<span data-ttu-id="2b9be-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b9be-133">DateTimeOffset</span></span>|<span data-ttu-id="2b9be-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2b9be-134">The date and time the object was last modified.</span></span> <span data-ttu-id="2b9be-135">НаСледуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2b9be-135">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2b9be-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b9be-136">createdDateTime</span></span>|<span data-ttu-id="2b9be-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b9be-137">DateTimeOffset</span></span>|<span data-ttu-id="2b9be-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2b9be-138">The date and time the object was created.</span></span> <span data-ttu-id="2b9be-139">НаСледуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2b9be-139">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2b9be-140">id</span><span class="sxs-lookup"><span data-stu-id="2b9be-140">id</span></span>|<span data-ttu-id="2b9be-141">String</span><span class="sxs-lookup"><span data-stu-id="2b9be-141">String</span></span>|<span data-ttu-id="2b9be-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2b9be-142">Key of the entity.</span></span> <span data-ttu-id="2b9be-143">НаСледуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2b9be-143">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2b9be-144">value</span><span class="sxs-lookup"><span data-stu-id="2b9be-144">value</span></span>|<span data-ttu-id="2b9be-145">Int64</span><span class="sxs-lookup"><span data-stu-id="2b9be-145">Int64</span></span>|<span data-ttu-id="2b9be-146">Целое значение без знака для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="2b9be-146">An unsigned integer value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="2b9be-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b9be-147">Response</span></span>
<span data-ttu-id="2b9be-148">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионвалуедеЦимал](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b9be-148">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b9be-149">Пример</span><span class="sxs-lookup"><span data-stu-id="2b9be-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b9be-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b9be-150">Request</span></span>
<span data-ttu-id="2b9be-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b9be-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="2b9be-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b9be-152">Response</span></span>
<span data-ttu-id="2b9be-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b9be-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




