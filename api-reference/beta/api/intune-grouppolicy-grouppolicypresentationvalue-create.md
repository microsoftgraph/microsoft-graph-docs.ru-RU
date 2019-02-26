---
title: Создание Граупполиципресентатионвалуе
description: Создание нового объекта Граупполиципресентатионвалуе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8e657917d0c07173e9a4a4553a7deaecc0f06f1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160902"
---
# <a name="create-grouppolicypresentationvalue"></a><span data-ttu-id="5e107-103">Создание Граупполиципресентатионвалуе</span><span class="sxs-lookup"><span data-stu-id="5e107-103">Create groupPolicyPresentationValue</span></span>

> <span data-ttu-id="5e107-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e107-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e107-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e107-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e107-106">Создание нового объекта [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="5e107-106">Create a new [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e107-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5e107-107">Prerequisites</span></span>
<span data-ttu-id="5e107-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5e107-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5e107-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e107-110">Permission type</span></span>|<span data-ttu-id="5e107-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e107-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e107-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e107-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5e107-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e107-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5e107-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e107-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e107-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e107-115">Not supported.</span></span>|
|<span data-ttu-id="5e107-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e107-116">Application</span></span>|<span data-ttu-id="5e107-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e107-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e107-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e107-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="5e107-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e107-119">Request headers</span></span>
|<span data-ttu-id="5e107-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e107-120">Header</span></span>|<span data-ttu-id="5e107-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5e107-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e107-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e107-122">Authorization</span></span>|<span data-ttu-id="5e107-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5e107-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e107-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5e107-124">Accept</span></span>|<span data-ttu-id="5e107-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5e107-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e107-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e107-126">Request body</span></span>
<span data-ttu-id="5e107-127">В тексте запроса добавьте представление объекта Граупполиципресентатионвалуе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e107-127">In the request body, supply a JSON representation for the groupPolicyPresentationValue object.</span></span>

<span data-ttu-id="5e107-128">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионвалуе.</span><span class="sxs-lookup"><span data-stu-id="5e107-128">The following table shows the properties that are required when you create the groupPolicyPresentationValue.</span></span>

|<span data-ttu-id="5e107-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e107-129">Property</span></span>|<span data-ttu-id="5e107-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5e107-130">Type</span></span>|<span data-ttu-id="5e107-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5e107-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e107-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e107-132">lastModifiedDateTime</span></span>|<span data-ttu-id="5e107-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e107-133">DateTimeOffset</span></span>|<span data-ttu-id="5e107-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5e107-134">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="5e107-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e107-135">createdDateTime</span></span>|<span data-ttu-id="5e107-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e107-136">DateTimeOffset</span></span>|<span data-ttu-id="5e107-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5e107-137">The date and time the object was created.</span></span>|
|<span data-ttu-id="5e107-138">id</span><span class="sxs-lookup"><span data-stu-id="5e107-138">id</span></span>|<span data-ttu-id="5e107-139">String</span><span class="sxs-lookup"><span data-stu-id="5e107-139">String</span></span>|<span data-ttu-id="5e107-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5e107-140">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="5e107-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e107-141">Response</span></span>
<span data-ttu-id="5e107-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e107-142">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e107-143">Пример</span><span class="sxs-lookup"><span data-stu-id="5e107-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e107-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e107-144">Request</span></span>
<span data-ttu-id="5e107-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e107-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="5e107-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e107-146">Response</span></span>
<span data-ttu-id="5e107-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5e107-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8132eaab-eaab-8132-abea-3281abea3281"
}
```




