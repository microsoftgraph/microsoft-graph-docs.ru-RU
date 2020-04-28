---
title: Обновление Граупполиципресентатионвалуетекст
description: Обновление свойств объекта Граупполиципресентатионвалуетекст.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7df0a93222ae83211ef3ec370e94796b2a6ab34e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43423060"
---
# <a name="update-grouppolicypresentationvaluetext"></a><span data-ttu-id="49c04-103">Обновление Граупполиципресентатионвалуетекст</span><span class="sxs-lookup"><span data-stu-id="49c04-103">Update groupPolicyPresentationValueText</span></span>

<span data-ttu-id="49c04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49c04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49c04-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49c04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49c04-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49c04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49c04-107">Обновление свойств объекта [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) .</span><span class="sxs-lookup"><span data-stu-id="49c04-107">Update the properties of a [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49c04-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="49c04-108">Prerequisites</span></span>
<span data-ttu-id="49c04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49c04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49c04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49c04-111">Permission type</span></span>|<span data-ttu-id="49c04-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49c04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49c04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49c04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49c04-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49c04-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49c04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49c04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49c04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49c04-116">Not supported.</span></span>|
|<span data-ttu-id="49c04-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49c04-117">Application</span></span>|<span data-ttu-id="49c04-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49c04-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49c04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49c04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="49c04-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="49c04-120">Request headers</span></span>
|<span data-ttu-id="49c04-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49c04-121">Header</span></span>|<span data-ttu-id="49c04-122">Значение</span><span class="sxs-lookup"><span data-stu-id="49c04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49c04-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49c04-123">Authorization</span></span>|<span data-ttu-id="49c04-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49c04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49c04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="49c04-125">Accept</span></span>|<span data-ttu-id="49c04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49c04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49c04-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="49c04-127">Request body</span></span>
<span data-ttu-id="49c04-128">В тексте запроса добавьте представление объекта [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49c04-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object.</span></span>

<span data-ttu-id="49c04-129">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).</span><span class="sxs-lookup"><span data-stu-id="49c04-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).</span></span>

|<span data-ttu-id="49c04-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="49c04-130">Property</span></span>|<span data-ttu-id="49c04-131">Тип</span><span class="sxs-lookup"><span data-stu-id="49c04-131">Type</span></span>|<span data-ttu-id="49c04-132">Описание</span><span class="sxs-lookup"><span data-stu-id="49c04-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49c04-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49c04-133">lastModifiedDateTime</span></span>|<span data-ttu-id="49c04-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49c04-134">DateTimeOffset</span></span>|<span data-ttu-id="49c04-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="49c04-135">The date and time the object was last modified.</span></span> <span data-ttu-id="49c04-136">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="49c04-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="49c04-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49c04-137">createdDateTime</span></span>|<span data-ttu-id="49c04-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49c04-138">DateTimeOffset</span></span>|<span data-ttu-id="49c04-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="49c04-139">The date and time the object was created.</span></span> <span data-ttu-id="49c04-140">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="49c04-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="49c04-141">id</span><span class="sxs-lookup"><span data-stu-id="49c04-141">id</span></span>|<span data-ttu-id="49c04-142">String</span><span class="sxs-lookup"><span data-stu-id="49c04-142">String</span></span>|<span data-ttu-id="49c04-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="49c04-143">Key of the entity.</span></span> <span data-ttu-id="49c04-144">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="49c04-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="49c04-145">value</span><span class="sxs-lookup"><span data-stu-id="49c04-145">value</span></span>|<span data-ttu-id="49c04-146">String</span><span class="sxs-lookup"><span data-stu-id="49c04-146">String</span></span>|<span data-ttu-id="49c04-147">Строковое значение для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="49c04-147">A string value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="49c04-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="49c04-148">Response</span></span>
<span data-ttu-id="49c04-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионвалуетекст](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49c04-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49c04-150">Пример</span><span class="sxs-lookup"><span data-stu-id="49c04-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="49c04-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="49c04-151">Request</span></span>
<span data-ttu-id="49c04-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49c04-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 101

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="49c04-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="49c04-153">Response</span></span>
<span data-ttu-id="49c04-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49c04-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "a3883444-3444-a388-4434-88a3443488a3",
  "value": "Value value"
}
```



