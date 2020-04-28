---
title: Создание Граупполицидефинитионвалуе
description: Создание нового объекта Граупполицидефинитионвалуе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8327d26dc2966f141a5c76e1b419101c130c88be
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454518"
---
# <a name="create-grouppolicydefinitionvalue"></a><span data-ttu-id="33fec-103">Создание Граупполицидефинитионвалуе</span><span class="sxs-lookup"><span data-stu-id="33fec-103">Create groupPolicyDefinitionValue</span></span>

<span data-ttu-id="33fec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33fec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33fec-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33fec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33fec-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33fec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33fec-107">Создание нового объекта [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .</span><span class="sxs-lookup"><span data-stu-id="33fec-107">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33fec-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="33fec-108">Prerequisites</span></span>
<span data-ttu-id="33fec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33fec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33fec-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33fec-111">Permission type</span></span>|<span data-ttu-id="33fec-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="33fec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33fec-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33fec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33fec-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33fec-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="33fec-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33fec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33fec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33fec-116">Not supported.</span></span>|
|<span data-ttu-id="33fec-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33fec-117">Application</span></span>|<span data-ttu-id="33fec-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33fec-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33fec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33fec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

## <a name="request-headers"></a><span data-ttu-id="33fec-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="33fec-120">Request headers</span></span>
|<span data-ttu-id="33fec-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="33fec-121">Header</span></span>|<span data-ttu-id="33fec-122">Значение</span><span class="sxs-lookup"><span data-stu-id="33fec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33fec-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33fec-123">Authorization</span></span>|<span data-ttu-id="33fec-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33fec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33fec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="33fec-125">Accept</span></span>|<span data-ttu-id="33fec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33fec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33fec-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="33fec-127">Request body</span></span>
<span data-ttu-id="33fec-128">В тексте запроса добавьте представление объекта Граупполицидефинитионвалуе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33fec-128">In the request body, supply a JSON representation for the groupPolicyDefinitionValue object.</span></span>

<span data-ttu-id="33fec-129">В следующей таблице приведены свойства, необходимые при создании Граупполицидефинитионвалуе.</span><span class="sxs-lookup"><span data-stu-id="33fec-129">The following table shows the properties that are required when you create the groupPolicyDefinitionValue.</span></span>

|<span data-ttu-id="33fec-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="33fec-130">Property</span></span>|<span data-ttu-id="33fec-131">Тип</span><span class="sxs-lookup"><span data-stu-id="33fec-131">Type</span></span>|<span data-ttu-id="33fec-132">Описание</span><span class="sxs-lookup"><span data-stu-id="33fec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33fec-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33fec-133">createdDateTime</span></span>|<span data-ttu-id="33fec-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33fec-134">DateTimeOffset</span></span>|<span data-ttu-id="33fec-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="33fec-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="33fec-136">enabled</span><span class="sxs-lookup"><span data-stu-id="33fec-136">enabled</span></span>|<span data-ttu-id="33fec-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="33fec-137">Boolean</span></span>|<span data-ttu-id="33fec-138">Включает или отключает соответствующее определение групповой политики.</span><span class="sxs-lookup"><span data-stu-id="33fec-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="33fec-139">конфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="33fec-139">configurationType</span></span>|[<span data-ttu-id="33fec-140">граупполициконфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="33fec-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="33fec-141">Указывает, как должно настраиваться значение.</span><span class="sxs-lookup"><span data-stu-id="33fec-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="33fec-142">Это может быть либо политика, либо предпочтение.</span><span class="sxs-lookup"><span data-stu-id="33fec-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="33fec-143">Возможные значения: `policy`, `preference`.</span><span class="sxs-lookup"><span data-stu-id="33fec-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="33fec-144">id</span><span class="sxs-lookup"><span data-stu-id="33fec-144">id</span></span>|<span data-ttu-id="33fec-145">String</span><span class="sxs-lookup"><span data-stu-id="33fec-145">String</span></span>|<span data-ttu-id="33fec-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="33fec-146">Key of the entity.</span></span>|
|<span data-ttu-id="33fec-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33fec-147">lastModifiedDateTime</span></span>|<span data-ttu-id="33fec-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33fec-148">DateTimeOffset</span></span>|<span data-ttu-id="33fec-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="33fec-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="33fec-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="33fec-150">Response</span></span>
<span data-ttu-id="33fec-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="33fec-151">If successful, this method returns a `201 Created` response code and a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33fec-152">Пример</span><span class="sxs-lookup"><span data-stu-id="33fec-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="33fec-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="33fec-153">Request</span></span>
<span data-ttu-id="33fec-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33fec-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
Content-type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": true,
  "configurationType": "preference"
}
```

### <a name="response"></a><span data-ttu-id="33fec-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="33fec-155">Response</span></span>
<span data-ttu-id="33fec-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="33fec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



