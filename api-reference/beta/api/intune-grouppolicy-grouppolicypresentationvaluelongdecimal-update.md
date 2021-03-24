---
title: Update groupPolicyPresentationValueLongDecimal
description: Обновление свойств объекта groupPolicyPresentationValueLongDecimal.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 29db585995728b84f6f4157c5e3c61c0ffa3fe7d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145735"
---
# <a name="update-grouppolicypresentationvaluelongdecimal"></a><span data-ttu-id="e76cd-103">Update groupPolicyPresentationValueLongDecimal</span><span class="sxs-lookup"><span data-stu-id="e76cd-103">Update groupPolicyPresentationValueLongDecimal</span></span>

<span data-ttu-id="e76cd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e76cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e76cd-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e76cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e76cd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e76cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e76cd-107">Обновление свойств объекта [groupPolicyPresentationValueLongDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)</span><span class="sxs-lookup"><span data-stu-id="e76cd-107">Update the properties of a [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e76cd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e76cd-108">Prerequisites</span></span>
<span data-ttu-id="e76cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e76cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e76cd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e76cd-111">Permission type</span></span>|<span data-ttu-id="e76cd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e76cd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e76cd-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e76cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e76cd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e76cd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e76cd-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e76cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e76cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e76cd-116">Not supported.</span></span>|
|<span data-ttu-id="e76cd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e76cd-117">Application</span></span>|<span data-ttu-id="e76cd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e76cd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e76cd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e76cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="e76cd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e76cd-120">Request headers</span></span>
|<span data-ttu-id="e76cd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e76cd-121">Header</span></span>|<span data-ttu-id="e76cd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e76cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e76cd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e76cd-123">Authorization</span></span>|<span data-ttu-id="e76cd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e76cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e76cd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e76cd-125">Accept</span></span>|<span data-ttu-id="e76cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e76cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e76cd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e76cd-127">Request body</span></span>
<span data-ttu-id="e76cd-128">В теле запроса поставляем представление JSON для [объекта groupPolicyPresentationValueLongDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)</span><span class="sxs-lookup"><span data-stu-id="e76cd-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object.</span></span>

<span data-ttu-id="e76cd-129">В следующей таблице показаны свойства, необходимые при создании [группыPolicyPresentationValueLongDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)</span><span class="sxs-lookup"><span data-stu-id="e76cd-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).</span></span>

|<span data-ttu-id="e76cd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e76cd-130">Property</span></span>|<span data-ttu-id="e76cd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e76cd-131">Type</span></span>|<span data-ttu-id="e76cd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e76cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e76cd-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e76cd-133">lastModifiedDateTime</span></span>|<span data-ttu-id="e76cd-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e76cd-134">DateTimeOffset</span></span>|<span data-ttu-id="e76cd-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e76cd-135">The date and time the object was last modified.</span></span> <span data-ttu-id="e76cd-136">Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e76cd-136">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="e76cd-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e76cd-137">createdDateTime</span></span>|<span data-ttu-id="e76cd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e76cd-138">DateTimeOffset</span></span>|<span data-ttu-id="e76cd-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e76cd-139">The date and time the object was created.</span></span> <span data-ttu-id="e76cd-140">Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e76cd-140">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="e76cd-141">id</span><span class="sxs-lookup"><span data-stu-id="e76cd-141">id</span></span>|<span data-ttu-id="e76cd-142">Строка</span><span class="sxs-lookup"><span data-stu-id="e76cd-142">String</span></span>|<span data-ttu-id="e76cd-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e76cd-143">Key of the entity.</span></span> <span data-ttu-id="e76cd-144">Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e76cd-144">Inherited from [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span></span>|
|<span data-ttu-id="e76cd-145">значение</span><span class="sxs-lookup"><span data-stu-id="e76cd-145">value</span></span>|<span data-ttu-id="e76cd-146">Int64</span><span class="sxs-lookup"><span data-stu-id="e76cd-146">Int64</span></span>|<span data-ttu-id="e76cd-147">Неподписаное длинное значение для связанной презентации.</span><span class="sxs-lookup"><span data-stu-id="e76cd-147">An unsigned long value for the associated presentation.</span></span>|



## <a name="response"></a><span data-ttu-id="e76cd-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="e76cd-148">Response</span></span>
<span data-ttu-id="e76cd-149">В случае успеха этот метод возвращает код ответа и обновленный `200 OK` [объект groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e76cd-149">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e76cd-150">Пример</span><span class="sxs-lookup"><span data-stu-id="e76cd-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="e76cd-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="e76cd-151">Request</span></span>
<span data-ttu-id="e76cd-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e76cd-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="e76cd-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="e76cd-153">Response</span></span>
<span data-ttu-id="e76cd-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e76cd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




