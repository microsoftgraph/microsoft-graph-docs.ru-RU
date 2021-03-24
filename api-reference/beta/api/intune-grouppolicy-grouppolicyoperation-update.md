---
title: Обновление groupPolicyOperation
description: Обновление свойств объекта groupPolicyOperation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a2aac24a6cc4d5a121b364b25c3ee5d18c76faf0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145742"
---
# <a name="update-grouppolicyoperation"></a><span data-ttu-id="2d3b7-103">Обновление groupPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="2d3b7-103">Update groupPolicyOperation</span></span>

<span data-ttu-id="2d3b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d3b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d3b7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d3b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d3b7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d3b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d3b7-107">Обновление свойств объекта [groupPolicyOperation.](../resources/intune-grouppolicy-grouppolicyoperation.md)</span><span class="sxs-lookup"><span data-stu-id="2d3b7-107">Update the properties of a [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d3b7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2d3b7-108">Prerequisites</span></span>
<span data-ttu-id="2d3b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d3b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d3b7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d3b7-111">Permission type</span></span>|<span data-ttu-id="2d3b7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d3b7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d3b7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d3b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2d3b7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d3b7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d3b7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d3b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d3b7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d3b7-116">Not supported.</span></span>|
|<span data-ttu-id="2d3b7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2d3b7-117">Application</span></span>|<span data-ttu-id="2d3b7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d3b7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d3b7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d3b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations/{groupPolicyOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="2d3b7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2d3b7-120">Request headers</span></span>
|<span data-ttu-id="2d3b7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d3b7-121">Header</span></span>|<span data-ttu-id="2d3b7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2d3b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d3b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d3b7-123">Authorization</span></span>|<span data-ttu-id="2d3b7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d3b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d3b7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2d3b7-125">Accept</span></span>|<span data-ttu-id="2d3b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2d3b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d3b7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d3b7-127">Request body</span></span>
<span data-ttu-id="2d3b7-128">В теле запроса поставляем представление JSON для [объекта groupPolicyOperation.](../resources/intune-grouppolicy-grouppolicyoperation.md)</span><span class="sxs-lookup"><span data-stu-id="2d3b7-128">In the request body, supply a JSON representation for the [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>

<span data-ttu-id="2d3b7-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyOperation.](../resources/intune-grouppolicy-grouppolicyoperation.md)</span><span class="sxs-lookup"><span data-stu-id="2d3b7-129">The following table shows the properties that are required when you create the [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md).</span></span>

|<span data-ttu-id="2d3b7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d3b7-130">Property</span></span>|<span data-ttu-id="2d3b7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2d3b7-131">Type</span></span>|<span data-ttu-id="2d3b7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2d3b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d3b7-133">operationType</span><span class="sxs-lookup"><span data-stu-id="2d3b7-133">operationType</span></span>|[<span data-ttu-id="2d3b7-134">groupPolicyOperationType</span><span class="sxs-lookup"><span data-stu-id="2d3b7-134">groupPolicyOperationType</span></span>](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|<span data-ttu-id="2d3b7-135">Тип операции групповой политики.</span><span class="sxs-lookup"><span data-stu-id="2d3b7-135">The type of group policy operation.</span></span> <span data-ttu-id="2d3b7-136">Возможные значения: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span><span class="sxs-lookup"><span data-stu-id="2d3b7-136">Possible values are: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span></span>|
|<span data-ttu-id="2d3b7-137">operationStatus</span><span class="sxs-lookup"><span data-stu-id="2d3b7-137">operationStatus</span></span>|[<span data-ttu-id="2d3b7-138">groupPolicyOperationStatus</span><span class="sxs-lookup"><span data-stu-id="2d3b7-138">groupPolicyOperationStatus</span></span>](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|<span data-ttu-id="2d3b7-139">Состояние операции групповой политики.</span><span class="sxs-lookup"><span data-stu-id="2d3b7-139">The group policy operation status.</span></span> <span data-ttu-id="2d3b7-140">Возможные значения: `unknown`, `inProgress`, `success`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="2d3b7-140">Possible values are: `unknown`, `inProgress`, `success`, `failed`.</span></span>|
|<span data-ttu-id="2d3b7-141">statusDetails</span><span class="sxs-lookup"><span data-stu-id="2d3b7-141">statusDetails</span></span>|<span data-ttu-id="2d3b7-142">Строка</span><span class="sxs-lookup"><span data-stu-id="2d3b7-142">String</span></span>|<span data-ttu-id="2d3b7-143">Подробное состояние состояния операции групповой политики.</span><span class="sxs-lookup"><span data-stu-id="2d3b7-143">The group policy operation status detail.</span></span>|
|<span data-ttu-id="2d3b7-144">id</span><span class="sxs-lookup"><span data-stu-id="2d3b7-144">id</span></span>|<span data-ttu-id="2d3b7-145">Строка</span><span class="sxs-lookup"><span data-stu-id="2d3b7-145">String</span></span>|<span data-ttu-id="2d3b7-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2d3b7-146">Key of the entity.</span></span>|
|<span data-ttu-id="2d3b7-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d3b7-147">lastModifiedDateTime</span></span>|<span data-ttu-id="2d3b7-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d3b7-148">DateTimeOffset</span></span>|<span data-ttu-id="2d3b7-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2d3b7-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="2d3b7-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d3b7-150">Response</span></span>
<span data-ttu-id="2d3b7-151">В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2d3b7-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d3b7-152">Пример</span><span class="sxs-lookup"><span data-stu-id="2d3b7-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d3b7-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d3b7-153">Request</span></span>
<span data-ttu-id="2d3b7-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d3b7-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations/{groupPolicyOperationId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "upload",
  "operationStatus": "inProgress",
  "statusDetails": "Status Details value"
}
```

### <a name="response"></a><span data-ttu-id="2d3b7-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d3b7-155">Response</span></span>
<span data-ttu-id="2d3b7-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d3b7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "upload",
  "operationStatus": "inProgress",
  "statusDetails": "Status Details value",
  "id": "4d18865b-865b-4d18-5b86-184d5b86184d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




