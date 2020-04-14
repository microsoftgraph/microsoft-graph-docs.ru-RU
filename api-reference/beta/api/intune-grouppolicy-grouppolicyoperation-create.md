---
title: Создание Граупполициоператион
description: Создание нового объекта Граупполициоператион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7461bfb2e993eeeffcdc6a333638c3c0c2b9d856
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456329"
---
# <a name="create-grouppolicyoperation"></a><span data-ttu-id="47d53-103">Создание Граупполициоператион</span><span class="sxs-lookup"><span data-stu-id="47d53-103">Create groupPolicyOperation</span></span>

<span data-ttu-id="47d53-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47d53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47d53-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47d53-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47d53-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47d53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47d53-107">Создание нового объекта [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="47d53-107">Create a new [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47d53-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="47d53-108">Prerequisites</span></span>
<span data-ttu-id="47d53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47d53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47d53-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47d53-111">Permission type</span></span>|<span data-ttu-id="47d53-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47d53-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47d53-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47d53-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47d53-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d53-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47d53-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47d53-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47d53-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47d53-116">Not supported.</span></span>|
|<span data-ttu-id="47d53-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47d53-117">Application</span></span>|<span data-ttu-id="47d53-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d53-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47d53-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47d53-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations
```

## <a name="request-headers"></a><span data-ttu-id="47d53-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="47d53-120">Request headers</span></span>
|<span data-ttu-id="47d53-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47d53-121">Header</span></span>|<span data-ttu-id="47d53-122">Значение</span><span class="sxs-lookup"><span data-stu-id="47d53-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47d53-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47d53-123">Authorization</span></span>|<span data-ttu-id="47d53-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47d53-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47d53-125">Accept</span><span class="sxs-lookup"><span data-stu-id="47d53-125">Accept</span></span>|<span data-ttu-id="47d53-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47d53-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47d53-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="47d53-127">Request body</span></span>
<span data-ttu-id="47d53-128">В тексте запроса добавьте представление объекта Граупполициоператион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47d53-128">In the request body, supply a JSON representation for the groupPolicyOperation object.</span></span>

<span data-ttu-id="47d53-129">В следующей таблице приведены свойства, необходимые при создании Граупполициоператион.</span><span class="sxs-lookup"><span data-stu-id="47d53-129">The following table shows the properties that are required when you create the groupPolicyOperation.</span></span>

|<span data-ttu-id="47d53-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="47d53-130">Property</span></span>|<span data-ttu-id="47d53-131">Тип</span><span class="sxs-lookup"><span data-stu-id="47d53-131">Type</span></span>|<span data-ttu-id="47d53-132">Описание</span><span class="sxs-lookup"><span data-stu-id="47d53-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47d53-133">оператионтипе</span><span class="sxs-lookup"><span data-stu-id="47d53-133">operationType</span></span>|[<span data-ttu-id="47d53-134">граупполициоператионтипе</span><span class="sxs-lookup"><span data-stu-id="47d53-134">groupPolicyOperationType</span></span>](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|<span data-ttu-id="47d53-135">Тип операции с групповой политикой.</span><span class="sxs-lookup"><span data-stu-id="47d53-135">The type of group policy operation.</span></span> <span data-ttu-id="47d53-136">Возможные значения: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span><span class="sxs-lookup"><span data-stu-id="47d53-136">Possible values are: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span></span>|
|<span data-ttu-id="47d53-137">оператионстатус</span><span class="sxs-lookup"><span data-stu-id="47d53-137">operationStatus</span></span>|[<span data-ttu-id="47d53-138">граупполициоператионстатус</span><span class="sxs-lookup"><span data-stu-id="47d53-138">groupPolicyOperationStatus</span></span>](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|<span data-ttu-id="47d53-139">Состояние операции групповой политики.</span><span class="sxs-lookup"><span data-stu-id="47d53-139">The group policy operation status.</span></span> <span data-ttu-id="47d53-140">Возможные значения: `unknown`, `inProgress`, `success`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="47d53-140">Possible values are: `unknown`, `inProgress`, `success`, `failed`.</span></span>|
|<span data-ttu-id="47d53-141">статусдетаилс</span><span class="sxs-lookup"><span data-stu-id="47d53-141">statusDetails</span></span>|<span data-ttu-id="47d53-142">String</span><span class="sxs-lookup"><span data-stu-id="47d53-142">String</span></span>|<span data-ttu-id="47d53-143">Сведения о состоянии операции групповой политики.</span><span class="sxs-lookup"><span data-stu-id="47d53-143">The group policy operation status detail.</span></span>|
|<span data-ttu-id="47d53-144">id</span><span class="sxs-lookup"><span data-stu-id="47d53-144">id</span></span>|<span data-ttu-id="47d53-145">String</span><span class="sxs-lookup"><span data-stu-id="47d53-145">String</span></span>|<span data-ttu-id="47d53-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="47d53-146">Key of the entity.</span></span>|
|<span data-ttu-id="47d53-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47d53-147">lastModifiedDateTime</span></span>|<span data-ttu-id="47d53-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47d53-148">DateTimeOffset</span></span>|<span data-ttu-id="47d53-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="47d53-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="47d53-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="47d53-150">Response</span></span>
<span data-ttu-id="47d53-151">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47d53-151">If successful, this method returns a `201 Created` response code and a [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47d53-152">Пример</span><span class="sxs-lookup"><span data-stu-id="47d53-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="47d53-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="47d53-153">Request</span></span>
<span data-ttu-id="47d53-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47d53-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47d53-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="47d53-155">Response</span></span>
<span data-ttu-id="47d53-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47d53-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



