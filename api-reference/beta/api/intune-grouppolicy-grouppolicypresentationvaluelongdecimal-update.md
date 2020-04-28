---
title: Обновление ГраупполиципресентатионвалуелонгдеЦимал
description: Обновление свойств объекта ГраупполиципресентатионвалуелонгдеЦимал.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd8b7b26a106ca3631ea668147e8783100acddd2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462682"
---
# <a name="update-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="2701f-103">Обновление ГраупполиципресентатионвалуелонгдеЦимал</span><span class="sxs-lookup"><span data-stu-id="2701f-103">Update groupPolicyPresentationValueLongDecimal</span></span>

<span data-ttu-id="2701f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2701f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2701f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2701f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2701f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2701f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2701f-107">Обновление свойств объекта [граупполиципресентатионвалуелонгдеЦимал](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .</span><span class="sxs-lookup"><span data-stu-id="2701f-107">Update the properties of a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2701f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2701f-108">Prerequisites</span></span>
<span data-ttu-id="2701f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2701f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2701f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2701f-111">Permission type</span></span>|<span data-ttu-id="2701f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2701f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2701f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2701f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2701f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2701f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2701f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2701f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2701f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2701f-116">Not supported.</span></span>|
|<span data-ttu-id="2701f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2701f-117">Application</span></span>|<span data-ttu-id="2701f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2701f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2701f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2701f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="2701f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2701f-120">Request headers</span></span>
|<span data-ttu-id="2701f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2701f-121">Header</span></span>|<span data-ttu-id="2701f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2701f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2701f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2701f-123">Authorization</span></span>|<span data-ttu-id="2701f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2701f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2701f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2701f-125">Accept</span></span>|<span data-ttu-id="2701f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2701f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2701f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2701f-127">Request body</span></span>
<span data-ttu-id="2701f-128">В тексте запроса добавьте представление объекта [граупполиципресентатионвалуелонгдеЦимал](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2701f-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

<span data-ttu-id="2701f-129">В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионвалуелонгдеЦимал](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span><span class="sxs-lookup"><span data-stu-id="2701f-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span></span>

|<span data-ttu-id="2701f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2701f-130">Property</span></span>|<span data-ttu-id="2701f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2701f-131">Type</span></span>|<span data-ttu-id="2701f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2701f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2701f-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2701f-133">lastModifiedDateTime</span></span>|<span data-ttu-id="2701f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2701f-134">DateTimeOffset</span></span>|<span data-ttu-id="2701f-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2701f-135">The date and time the object was last modified.</span></span> <span data-ttu-id="2701f-136">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2701f-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2701f-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2701f-137">createdDateTime</span></span>|<span data-ttu-id="2701f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2701f-138">DateTimeOffset</span></span>|<span data-ttu-id="2701f-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2701f-139">The date and time the object was created.</span></span> <span data-ttu-id="2701f-140">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2701f-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2701f-141">id</span><span class="sxs-lookup"><span data-stu-id="2701f-141">id</span></span>|<span data-ttu-id="2701f-142">String</span><span class="sxs-lookup"><span data-stu-id="2701f-142">String</span></span>|<span data-ttu-id="2701f-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2701f-143">Key of the entity.</span></span> <span data-ttu-id="2701f-144">Наследуется от [граупполиципресентатионвалуе](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2701f-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="2701f-145">значение</span><span class="sxs-lookup"><span data-stu-id="2701f-145">value</span></span>|<span data-ttu-id="2701f-146">Int64</span><span class="sxs-lookup"><span data-stu-id="2701f-146">Int64</span></span>|<span data-ttu-id="2701f-147">Длинное значение без знака для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="2701f-147">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="2701f-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="2701f-148">Response</span></span>
<span data-ttu-id="2701f-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионвалуелонгдеЦимал](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2701f-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2701f-150">Пример</span><span class="sxs-lookup"><span data-stu-id="2701f-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="2701f-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="2701f-151">Request</span></span>
<span data-ttu-id="2701f-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2701f-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="2701f-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="2701f-153">Response</span></span>
<span data-ttu-id="2701f-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2701f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "210f7078-7078-210f-7870-0f2178700f21",
  "value": 5
}
```



