---
title: Создание groupPolicyDefinitionValue
description: Создайте новый объект GroupPolicyDefinitionValue.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 21268136dde7a2e813a854d779f11f5f0e61217e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142046"
---
# <a name="create-grouppolicydefinitionvalue"></a><span data-ttu-id="fb69d-103">Создание groupPolicyDefinitionValue</span><span class="sxs-lookup"><span data-stu-id="fb69d-103">Create groupPolicyDefinitionValue</span></span>

<span data-ttu-id="fb69d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb69d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb69d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb69d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb69d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb69d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb69d-107">Создайте новый [объект GroupPolicyDefinitionValue.](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="fb69d-107">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb69d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fb69d-108">Prerequisites</span></span>
<span data-ttu-id="fb69d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb69d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb69d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb69d-111">Permission type</span></span>|<span data-ttu-id="fb69d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb69d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb69d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb69d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb69d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb69d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb69d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb69d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb69d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb69d-116">Not supported.</span></span>|
|<span data-ttu-id="fb69d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fb69d-117">Application</span></span>|<span data-ttu-id="fb69d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb69d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb69d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb69d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

## <a name="request-headers"></a><span data-ttu-id="fb69d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fb69d-120">Request headers</span></span>
|<span data-ttu-id="fb69d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb69d-121">Header</span></span>|<span data-ttu-id="fb69d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fb69d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb69d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb69d-123">Authorization</span></span>|<span data-ttu-id="fb69d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb69d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb69d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb69d-125">Accept</span></span>|<span data-ttu-id="fb69d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb69d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb69d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb69d-127">Request body</span></span>
<span data-ttu-id="fb69d-128">В теле запроса поставляем представление JSON для объекта GroupPolicyDefinitionValue.</span><span class="sxs-lookup"><span data-stu-id="fb69d-128">In the request body, supply a JSON representation for the groupPolicyDefinitionValue object.</span></span>

<span data-ttu-id="fb69d-129">В следующей таблице показаны свойства, необходимые при создании группыPolicyDefinitionValue.</span><span class="sxs-lookup"><span data-stu-id="fb69d-129">The following table shows the properties that are required when you create the groupPolicyDefinitionValue.</span></span>

|<span data-ttu-id="fb69d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb69d-130">Property</span></span>|<span data-ttu-id="fb69d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fb69d-131">Type</span></span>|<span data-ttu-id="fb69d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fb69d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb69d-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb69d-133">createdDateTime</span></span>|<span data-ttu-id="fb69d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb69d-134">DateTimeOffset</span></span>|<span data-ttu-id="fb69d-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fb69d-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="fb69d-136">enabled</span><span class="sxs-lookup"><span data-stu-id="fb69d-136">enabled</span></span>|<span data-ttu-id="fb69d-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb69d-137">Boolean</span></span>|<span data-ttu-id="fb69d-138">Включает или отключает связанное определение групповой политики.</span><span class="sxs-lookup"><span data-stu-id="fb69d-138">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="fb69d-139">configurationType</span><span class="sxs-lookup"><span data-stu-id="fb69d-139">configurationType</span></span>|[<span data-ttu-id="fb69d-140">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="fb69d-140">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="fb69d-141">Указывает, как следует настроить значение.</span><span class="sxs-lookup"><span data-stu-id="fb69d-141">Specifies how the value should be configured.</span></span> <span data-ttu-id="fb69d-142">Это может быть как политика, так и как предпочтение.</span><span class="sxs-lookup"><span data-stu-id="fb69d-142">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="fb69d-143">Возможные значения: `policy`, `preference`.</span><span class="sxs-lookup"><span data-stu-id="fb69d-143">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="fb69d-144">id</span><span class="sxs-lookup"><span data-stu-id="fb69d-144">id</span></span>|<span data-ttu-id="fb69d-145">Строка</span><span class="sxs-lookup"><span data-stu-id="fb69d-145">String</span></span>|<span data-ttu-id="fb69d-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fb69d-146">Key of the entity.</span></span>|
|<span data-ttu-id="fb69d-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb69d-147">lastModifiedDateTime</span></span>|<span data-ttu-id="fb69d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb69d-148">DateTimeOffset</span></span>|<span data-ttu-id="fb69d-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fb69d-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="fb69d-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb69d-150">Response</span></span>
<span data-ttu-id="fb69d-151">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект GroupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fb69d-151">If successful, this method returns a `201 Created` response code and a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb69d-152">Пример</span><span class="sxs-lookup"><span data-stu-id="fb69d-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb69d-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb69d-153">Request</span></span>
<span data-ttu-id="fb69d-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb69d-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fb69d-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb69d-155">Response</span></span>
<span data-ttu-id="fb69d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb69d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




