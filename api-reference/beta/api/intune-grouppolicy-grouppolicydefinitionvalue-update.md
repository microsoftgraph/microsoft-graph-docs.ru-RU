---
title: Обновление Граупполицидефинитионвалуе
description: Обновление свойств объекта Граупполицидефинитионвалуе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 224d57b2cd327e3e61e59dc77d2e1cbcb93d56de
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723191"
---
# <a name="update-grouppolicydefinitionvalue"></a><span data-ttu-id="59a66-103">Обновление Граупполицидефинитионвалуе</span><span class="sxs-lookup"><span data-stu-id="59a66-103">Update groupPolicyDefinitionValue</span></span>

<span data-ttu-id="59a66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59a66-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59a66-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59a66-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59a66-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="59a66-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59a66-107">Обновление свойств объекта [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="59a66-107">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59a66-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="59a66-108">Prerequisites</span></span>
<span data-ttu-id="59a66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59a66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59a66-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59a66-111">Permission type</span></span>|<span data-ttu-id="59a66-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="59a66-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59a66-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59a66-113">Delegated (work or school account)</span></span>|<span data-ttu-id="59a66-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59a66-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="59a66-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59a66-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59a66-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59a66-116">Not supported.</span></span>|
|<span data-ttu-id="59a66-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59a66-117">Application</span></span>|<span data-ttu-id="59a66-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59a66-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59a66-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59a66-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a><span data-ttu-id="59a66-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="59a66-120">Request headers</span></span>
|<span data-ttu-id="59a66-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59a66-121">Header</span></span>|<span data-ttu-id="59a66-122">Значение</span><span class="sxs-lookup"><span data-stu-id="59a66-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59a66-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59a66-123">Authorization</span></span>|<span data-ttu-id="59a66-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59a66-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59a66-125">Accept</span><span class="sxs-lookup"><span data-stu-id="59a66-125">Accept</span></span>|<span data-ttu-id="59a66-126">application/json</span><span class="sxs-lookup"><span data-stu-id="59a66-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59a66-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="59a66-127">Request body</span></span>
<span data-ttu-id="59a66-128">В тексте запроса добавьте представление объекта [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59a66-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

<span data-ttu-id="59a66-129">В следующей таблице приведены свойства, необходимые при создании [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span><span class="sxs-lookup"><span data-stu-id="59a66-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>

|<span data-ttu-id="59a66-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="59a66-130">Property</span></span>|<span data-ttu-id="59a66-131">Тип</span><span class="sxs-lookup"><span data-stu-id="59a66-131">Type</span></span>|<span data-ttu-id="59a66-132">Описание</span><span class="sxs-lookup"><span data-stu-id="59a66-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59a66-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59a66-133">createdDateTime</span></span>|<span data-ttu-id="59a66-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59a66-134">DateTimeOffset</span></span>|<span data-ttu-id="59a66-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="59a66-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="59a66-136">enabled</span><span class="sxs-lookup"><span data-stu-id="59a66-136">enabled</span></span>|<span data-ttu-id="59a66-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="59a66-137">Boolean</span></span>|<span data-ttu-id="59a66-138">Включает или отключает соответствующее определение групповой политики.</span><span class="sxs-lookup"><span data-stu-id="59a66-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="59a66-139">конфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="59a66-139">configurationType</span></span>|[<span data-ttu-id="59a66-140">граупполициконфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="59a66-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="59a66-141">Указывает, как должно настраиваться значение.</span><span class="sxs-lookup"><span data-stu-id="59a66-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="59a66-142">Это может быть либо политика, либо предпочтение.</span><span class="sxs-lookup"><span data-stu-id="59a66-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="59a66-143">Возможные значения: `policy`, `preference`.</span><span class="sxs-lookup"><span data-stu-id="59a66-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="59a66-144">id</span><span class="sxs-lookup"><span data-stu-id="59a66-144">id</span></span>|<span data-ttu-id="59a66-145">Строка</span><span class="sxs-lookup"><span data-stu-id="59a66-145">String</span></span>|<span data-ttu-id="59a66-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="59a66-146">Key of the entity.</span></span>|
|<span data-ttu-id="59a66-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59a66-147">lastModifiedDateTime</span></span>|<span data-ttu-id="59a66-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59a66-148">DateTimeOffset</span></span>|<span data-ttu-id="59a66-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="59a66-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="59a66-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="59a66-150">Response</span></span>
<span data-ttu-id="59a66-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="59a66-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59a66-152">Пример</span><span class="sxs-lookup"><span data-stu-id="59a66-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="59a66-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="59a66-153">Request</span></span>
<span data-ttu-id="59a66-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59a66-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
Content-type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": true,
  "configurationType": "preference"
}
```

### <a name="response"></a><span data-ttu-id="59a66-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="59a66-155">Response</span></span>
<span data-ttu-id="59a66-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59a66-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "enabled": true,
  "configurationType": "preference",
  "id": "50428918-8918-5042-1889-425018894250",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





