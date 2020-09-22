---
title: Создание Граупполициоператион
description: Создание нового объекта Граупполициоператион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e131361edf0d563eb67fb7e12865d312f938c9f0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078852"
---
# <a name="create-grouppolicyoperation"></a><span data-ttu-id="578d5-103">Создание Граупполициоператион</span><span class="sxs-lookup"><span data-stu-id="578d5-103">Create groupPolicyOperation</span></span>

<span data-ttu-id="578d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="578d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="578d5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="578d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="578d5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="578d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="578d5-107">Создание нового объекта [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="578d5-107">Create a new [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="578d5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="578d5-108">Prerequisites</span></span>
<span data-ttu-id="578d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="578d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="578d5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="578d5-111">Permission type</span></span>|<span data-ttu-id="578d5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="578d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="578d5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="578d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="578d5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="578d5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="578d5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="578d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="578d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="578d5-116">Not supported.</span></span>|
|<span data-ttu-id="578d5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="578d5-117">Application</span></span>|<span data-ttu-id="578d5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="578d5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="578d5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="578d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations
```

## <a name="request-headers"></a><span data-ttu-id="578d5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="578d5-120">Request headers</span></span>
|<span data-ttu-id="578d5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="578d5-121">Header</span></span>|<span data-ttu-id="578d5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="578d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="578d5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="578d5-123">Authorization</span></span>|<span data-ttu-id="578d5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="578d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="578d5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="578d5-125">Accept</span></span>|<span data-ttu-id="578d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="578d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="578d5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="578d5-127">Request body</span></span>
<span data-ttu-id="578d5-128">В тексте запроса добавьте представление объекта Граупполициоператион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="578d5-128">In the request body, supply a JSON representation for the groupPolicyOperation object.</span></span>

<span data-ttu-id="578d5-129">В следующей таблице приведены свойства, необходимые при создании Граупполициоператион.</span><span class="sxs-lookup"><span data-stu-id="578d5-129">The following table shows the properties that are required when you create the groupPolicyOperation.</span></span>

|<span data-ttu-id="578d5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="578d5-130">Property</span></span>|<span data-ttu-id="578d5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="578d5-131">Type</span></span>|<span data-ttu-id="578d5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="578d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="578d5-133">оператионтипе</span><span class="sxs-lookup"><span data-stu-id="578d5-133">operationType</span></span>|[<span data-ttu-id="578d5-134">groupPolicyOperationType</span><span class="sxs-lookup"><span data-stu-id="578d5-134">groupPolicyOperationType</span></span>](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|<span data-ttu-id="578d5-135">Тип операции с групповой политикой.</span><span class="sxs-lookup"><span data-stu-id="578d5-135">The type of group policy operation.</span></span> <span data-ttu-id="578d5-136">Возможные значения: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span><span class="sxs-lookup"><span data-stu-id="578d5-136">Possible values are: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span></span>|
|<span data-ttu-id="578d5-137">оператионстатус</span><span class="sxs-lookup"><span data-stu-id="578d5-137">operationStatus</span></span>|[<span data-ttu-id="578d5-138">groupPolicyOperationStatus</span><span class="sxs-lookup"><span data-stu-id="578d5-138">groupPolicyOperationStatus</span></span>](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|<span data-ttu-id="578d5-139">Состояние операции групповой политики.</span><span class="sxs-lookup"><span data-stu-id="578d5-139">The group policy operation status.</span></span> <span data-ttu-id="578d5-140">Возможные значения: `unknown`, `inProgress`, `success`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="578d5-140">Possible values are: `unknown`, `inProgress`, `success`, `failed`.</span></span>|
|<span data-ttu-id="578d5-141">статусдетаилс</span><span class="sxs-lookup"><span data-stu-id="578d5-141">statusDetails</span></span>|<span data-ttu-id="578d5-142">String</span><span class="sxs-lookup"><span data-stu-id="578d5-142">String</span></span>|<span data-ttu-id="578d5-143">Сведения о состоянии операции групповой политики.</span><span class="sxs-lookup"><span data-stu-id="578d5-143">The group policy operation status detail.</span></span>|
|<span data-ttu-id="578d5-144">id</span><span class="sxs-lookup"><span data-stu-id="578d5-144">id</span></span>|<span data-ttu-id="578d5-145">String</span><span class="sxs-lookup"><span data-stu-id="578d5-145">String</span></span>|<span data-ttu-id="578d5-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="578d5-146">Key of the entity.</span></span>|
|<span data-ttu-id="578d5-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="578d5-147">lastModifiedDateTime</span></span>|<span data-ttu-id="578d5-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="578d5-148">DateTimeOffset</span></span>|<span data-ttu-id="578d5-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="578d5-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="578d5-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="578d5-150">Response</span></span>
<span data-ttu-id="578d5-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="578d5-151">If successful, this method returns a `201 Created` response code and a [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="578d5-152">Пример</span><span class="sxs-lookup"><span data-stu-id="578d5-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="578d5-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="578d5-153">Request</span></span>
<span data-ttu-id="578d5-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="578d5-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "upload",
  "operationStatus": "inProgress",
  "statusDetails": "Status Details value"
}
```

### <a name="response"></a><span data-ttu-id="578d5-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="578d5-155">Response</span></span>
<span data-ttu-id="578d5-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="578d5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






