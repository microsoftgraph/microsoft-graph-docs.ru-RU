---
title: Создание Граупполиципресентатионвалуе
description: Создание нового объекта Граупполиципресентатионвалуе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 86da1fc53ffba6f386bfdfffa7d7b96c83a80407
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39942761"
---
# <a name="create-grouppolicypresentationvalue"></a><span data-ttu-id="30b46-103">Создание Граупполиципресентатионвалуе</span><span class="sxs-lookup"><span data-stu-id="30b46-103">Create groupPolicyPresentationValue</span></span>

> <span data-ttu-id="30b46-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30b46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30b46-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30b46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30b46-106">Создание нового объекта [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="30b46-106">Create a new [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30b46-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="30b46-107">Prerequisites</span></span>
<span data-ttu-id="30b46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30b46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30b46-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30b46-110">Permission type</span></span>|<span data-ttu-id="30b46-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30b46-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30b46-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30b46-112">Delegated (work or school account)</span></span>|<span data-ttu-id="30b46-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30b46-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="30b46-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30b46-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30b46-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30b46-115">Not supported.</span></span>|
|<span data-ttu-id="30b46-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30b46-116">Application</span></span>|<span data-ttu-id="30b46-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30b46-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30b46-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30b46-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="30b46-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="30b46-119">Request headers</span></span>
|<span data-ttu-id="30b46-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30b46-120">Header</span></span>|<span data-ttu-id="30b46-121">Значение</span><span class="sxs-lookup"><span data-stu-id="30b46-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30b46-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30b46-122">Authorization</span></span>|<span data-ttu-id="30b46-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30b46-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30b46-124">Accept</span><span class="sxs-lookup"><span data-stu-id="30b46-124">Accept</span></span>|<span data-ttu-id="30b46-125">application/json</span><span class="sxs-lookup"><span data-stu-id="30b46-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30b46-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="30b46-126">Request body</span></span>
<span data-ttu-id="30b46-127">В тексте запроса добавьте представление объекта Граупполиципресентатионвалуе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30b46-127">In the request body, supply a JSON representation for the groupPolicyPresentationValue object.</span></span>

<span data-ttu-id="30b46-128">В следующей таблице приведены свойства, необходимые при создании Граупполиципресентатионвалуе.</span><span class="sxs-lookup"><span data-stu-id="30b46-128">The following table shows the properties that are required when you create the groupPolicyPresentationValue.</span></span>

|<span data-ttu-id="30b46-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="30b46-129">Property</span></span>|<span data-ttu-id="30b46-130">Тип</span><span class="sxs-lookup"><span data-stu-id="30b46-130">Type</span></span>|<span data-ttu-id="30b46-131">Описание</span><span class="sxs-lookup"><span data-stu-id="30b46-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30b46-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30b46-132">lastModifiedDateTime</span></span>|<span data-ttu-id="30b46-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30b46-133">DateTimeOffset</span></span>|<span data-ttu-id="30b46-134">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="30b46-134">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="30b46-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30b46-135">createdDateTime</span></span>|<span data-ttu-id="30b46-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30b46-136">DateTimeOffset</span></span>|<span data-ttu-id="30b46-137">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="30b46-137">The date and time the object was created.</span></span>|
|<span data-ttu-id="30b46-138">id</span><span class="sxs-lookup"><span data-stu-id="30b46-138">id</span></span>|<span data-ttu-id="30b46-139">Строка</span><span class="sxs-lookup"><span data-stu-id="30b46-139">String</span></span>|<span data-ttu-id="30b46-140">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="30b46-140">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="30b46-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="30b46-141">Response</span></span>
<span data-ttu-id="30b46-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30b46-142">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30b46-143">Пример</span><span class="sxs-lookup"><span data-stu-id="30b46-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="30b46-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="30b46-144">Request</span></span>
<span data-ttu-id="30b46-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30b46-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="30b46-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="30b46-146">Response</span></span>
<span data-ttu-id="30b46-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30b46-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





