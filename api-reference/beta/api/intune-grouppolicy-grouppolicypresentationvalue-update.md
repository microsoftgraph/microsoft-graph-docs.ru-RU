---
title: Обновление groupPolicyPresentationValue
description: Обновление свойств объекта groupPolicyPresentationValue.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4c91d98fc16a338d2aeadd75aae45e9535a38c82
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51157323"
---
# <a name="update-grouppolicypresentationvalue"></a><span data-ttu-id="a9517-103">Обновление groupPolicyPresentationValue</span><span class="sxs-lookup"><span data-stu-id="a9517-103">Update groupPolicyPresentationValue</span></span>

<span data-ttu-id="a9517-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9517-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9517-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9517-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9517-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9517-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9517-107">Обновление свойств объекта [groupPolicyPresentationValue.](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="a9517-107">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9517-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a9517-108">Prerequisites</span></span>
<span data-ttu-id="a9517-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9517-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9517-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9517-111">Permission type</span></span>|<span data-ttu-id="a9517-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9517-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9517-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9517-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9517-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9517-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9517-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9517-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9517-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9517-116">Not supported.</span></span>|
|<span data-ttu-id="a9517-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a9517-117">Application</span></span>|<span data-ttu-id="a9517-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9517-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9517-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9517-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="a9517-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a9517-120">Request headers</span></span>
|<span data-ttu-id="a9517-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9517-121">Header</span></span>|<span data-ttu-id="a9517-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a9517-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9517-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9517-123">Authorization</span></span>|<span data-ttu-id="a9517-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9517-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9517-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a9517-125">Accept</span></span>|<span data-ttu-id="a9517-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9517-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9517-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9517-127">Request body</span></span>
<span data-ttu-id="a9517-128">В теле запроса поставляем представление JSON для [объекта GroupPolicyPresentationValue.](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="a9517-128">In the request body, supply a JSON representation for the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

<span data-ttu-id="a9517-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyPresentationValue.](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)</span><span class="sxs-lookup"><span data-stu-id="a9517-129">The following table shows the properties that are required when you create the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>

|<span data-ttu-id="a9517-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9517-130">Property</span></span>|<span data-ttu-id="a9517-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a9517-131">Type</span></span>|<span data-ttu-id="a9517-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a9517-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9517-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9517-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a9517-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9517-134">DateTimeOffset</span></span>|<span data-ttu-id="a9517-135">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a9517-135">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="a9517-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9517-136">createdDateTime</span></span>|<span data-ttu-id="a9517-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9517-137">DateTimeOffset</span></span>|<span data-ttu-id="a9517-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a9517-138">The date and time the object was created.</span></span>|
|<span data-ttu-id="a9517-139">id</span><span class="sxs-lookup"><span data-stu-id="a9517-139">id</span></span>|<span data-ttu-id="a9517-140">Строка</span><span class="sxs-lookup"><span data-stu-id="a9517-140">String</span></span>|<span data-ttu-id="a9517-141">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a9517-141">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="a9517-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9517-142">Response</span></span>
<span data-ttu-id="a9517-143">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a9517-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9517-144">Пример</span><span class="sxs-lookup"><span data-stu-id="a9517-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9517-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9517-145">Request</span></span>
<span data-ttu-id="a9517-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9517-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="a9517-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9517-147">Response</span></span>
<span data-ttu-id="a9517-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9517-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




