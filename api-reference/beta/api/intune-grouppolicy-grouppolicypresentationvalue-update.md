---
title: Обновление Граупполиципресентатионвалуе
description: Обновление свойств объекта Граупполиципресентатионвалуе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dc93403587282d9f9c449a09dad77b98f9e70181
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33904505"
---
# <a name="update-grouppolicypresentationvalue"></a><span data-ttu-id="f85ec-103">Обновление Граупполиципресентатионвалуе</span><span class="sxs-lookup"><span data-stu-id="f85ec-103">Update groupPolicyPresentationValue</span></span>

> <span data-ttu-id="f85ec-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f85ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f85ec-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f85ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f85ec-106">Обновление свойств объекта [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="f85ec-106">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f85ec-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f85ec-107">Prerequisites</span></span>
<span data-ttu-id="f85ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f85ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f85ec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f85ec-110">Permission type</span></span>|<span data-ttu-id="f85ec-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f85ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f85ec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f85ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f85ec-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f85ec-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f85ec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f85ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f85ec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f85ec-115">Not supported.</span></span>|
|<span data-ttu-id="f85ec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f85ec-116">Application</span></span>|<span data-ttu-id="f85ec-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f85ec-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f85ec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f85ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="f85ec-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f85ec-119">Request headers</span></span>
|<span data-ttu-id="f85ec-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f85ec-120">Header</span></span>|<span data-ttu-id="f85ec-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f85ec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f85ec-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f85ec-122">Authorization</span></span>|<span data-ttu-id="f85ec-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f85ec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f85ec-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f85ec-124">Accept</span></span>|<span data-ttu-id="f85ec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f85ec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f85ec-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f85ec-126">Request body</span></span>
<span data-ttu-id="f85ec-127">В тексте запроса добавьте представление объекта [Граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f85ec-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

<span data-ttu-id="f85ec-128">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span><span class="sxs-lookup"><span data-stu-id="f85ec-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>

|<span data-ttu-id="f85ec-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f85ec-129">Property</span></span>|<span data-ttu-id="f85ec-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f85ec-130">Type</span></span>|<span data-ttu-id="f85ec-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f85ec-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f85ec-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f85ec-132">lastModifiedDateTime</span></span>|<span data-ttu-id="f85ec-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f85ec-133">DateTimeOffset</span></span>|<span data-ttu-id="f85ec-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f85ec-134">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="f85ec-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f85ec-135">createdDateTime</span></span>|<span data-ttu-id="f85ec-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f85ec-136">DateTimeOffset</span></span>|<span data-ttu-id="f85ec-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f85ec-137">The date and time the object was created.</span></span>|
|<span data-ttu-id="f85ec-138">id</span><span class="sxs-lookup"><span data-stu-id="f85ec-138">id</span></span>|<span data-ttu-id="f85ec-139">Строка</span><span class="sxs-lookup"><span data-stu-id="f85ec-139">String</span></span>|<span data-ttu-id="f85ec-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f85ec-140">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="f85ec-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f85ec-141">Response</span></span>
<span data-ttu-id="f85ec-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f85ec-142">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f85ec-143">Пример</span><span class="sxs-lookup"><span data-stu-id="f85ec-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="f85ec-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="f85ec-144">Request</span></span>
<span data-ttu-id="f85ec-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f85ec-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="f85ec-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="f85ec-146">Response</span></span>
<span data-ttu-id="f85ec-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f85ec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8132eaab-eaab-8132-abea-3281abea3281"
}
```




