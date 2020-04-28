---
title: Обновление Граупполиципресентатионвалуе
description: Обновление свойств объекта Граупполиципресентатионвалуе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b6598092ab48a357cd98dd90b29f4dd147d1bdfd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462797"
---
# <a name="update-grouppolicypresentationvalue"></a><span data-ttu-id="8df13-103">Обновление Граупполиципресентатионвалуе</span><span class="sxs-lookup"><span data-stu-id="8df13-103">Update groupPolicyPresentationValue</span></span>

<span data-ttu-id="8df13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8df13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8df13-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8df13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8df13-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8df13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8df13-107">Обновление свойств объекта [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="8df13-107">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8df13-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8df13-108">Prerequisites</span></span>
<span data-ttu-id="8df13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8df13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8df13-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8df13-111">Permission type</span></span>|<span data-ttu-id="8df13-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8df13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8df13-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8df13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8df13-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8df13-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8df13-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8df13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8df13-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8df13-116">Not supported.</span></span>|
|<span data-ttu-id="8df13-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8df13-117">Application</span></span>|<span data-ttu-id="8df13-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8df13-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8df13-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8df13-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="8df13-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8df13-120">Request headers</span></span>
|<span data-ttu-id="8df13-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8df13-121">Header</span></span>|<span data-ttu-id="8df13-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8df13-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8df13-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8df13-123">Authorization</span></span>|<span data-ttu-id="8df13-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8df13-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8df13-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8df13-125">Accept</span></span>|<span data-ttu-id="8df13-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8df13-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8df13-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8df13-127">Request body</span></span>
<span data-ttu-id="8df13-128">В тексте запроса добавьте представление объекта [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8df13-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

<span data-ttu-id="8df13-129">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span><span class="sxs-lookup"><span data-stu-id="8df13-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>

|<span data-ttu-id="8df13-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8df13-130">Property</span></span>|<span data-ttu-id="8df13-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8df13-131">Type</span></span>|<span data-ttu-id="8df13-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8df13-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8df13-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8df13-133">lastModifiedDateTime</span></span>|<span data-ttu-id="8df13-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8df13-134">DateTimeOffset</span></span>|<span data-ttu-id="8df13-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8df13-135">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="8df13-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8df13-136">createdDateTime</span></span>|<span data-ttu-id="8df13-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8df13-137">DateTimeOffset</span></span>|<span data-ttu-id="8df13-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8df13-138">The date and time the object was created.</span></span>|
|<span data-ttu-id="8df13-139">id</span><span class="sxs-lookup"><span data-stu-id="8df13-139">id</span></span>|<span data-ttu-id="8df13-140">String</span><span class="sxs-lookup"><span data-stu-id="8df13-140">String</span></span>|<span data-ttu-id="8df13-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8df13-141">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="8df13-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8df13-142">Response</span></span>
<span data-ttu-id="8df13-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8df13-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8df13-144">Пример</span><span class="sxs-lookup"><span data-stu-id="8df13-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="8df13-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="8df13-145">Request</span></span>
<span data-ttu-id="8df13-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8df13-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="8df13-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="8df13-147">Response</span></span>
<span data-ttu-id="8df13-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8df13-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



