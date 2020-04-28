---
title: Обновление Граупполициоператион
description: Обновление свойств объекта Граупполициоператион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 365d94e1c7710bf8c1b84878a1b0feff123f3faf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457295"
---
# <a name="update-grouppolicyoperation"></a><span data-ttu-id="6aa72-103">Обновление Граупполициоператион</span><span class="sxs-lookup"><span data-stu-id="6aa72-103">Update groupPolicyOperation</span></span>

<span data-ttu-id="6aa72-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6aa72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6aa72-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6aa72-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6aa72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aa72-107">Обновление свойств объекта [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="6aa72-107">Update the properties of a [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6aa72-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6aa72-108">Prerequisites</span></span>
<span data-ttu-id="6aa72-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6aa72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aa72-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6aa72-111">Permission type</span></span>|<span data-ttu-id="6aa72-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6aa72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6aa72-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6aa72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6aa72-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aa72-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6aa72-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6aa72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6aa72-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa72-116">Not supported.</span></span>|
|<span data-ttu-id="6aa72-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6aa72-117">Application</span></span>|<span data-ttu-id="6aa72-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aa72-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6aa72-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6aa72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations/{groupPolicyOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="6aa72-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6aa72-120">Request headers</span></span>
|<span data-ttu-id="6aa72-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6aa72-121">Header</span></span>|<span data-ttu-id="6aa72-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6aa72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6aa72-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6aa72-123">Authorization</span></span>|<span data-ttu-id="6aa72-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6aa72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6aa72-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6aa72-125">Accept</span></span>|<span data-ttu-id="6aa72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6aa72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aa72-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6aa72-127">Request body</span></span>
<span data-ttu-id="6aa72-128">В тексте запроса добавьте представление объекта [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6aa72-128">In the request body, supply a JSON representation for the [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>

<span data-ttu-id="6aa72-129">В следующей таблице приведены свойства, необходимые при создании [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md).</span><span class="sxs-lookup"><span data-stu-id="6aa72-129">The following table shows the properties that are required when you create the [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md).</span></span>

|<span data-ttu-id="6aa72-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6aa72-130">Property</span></span>|<span data-ttu-id="6aa72-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6aa72-131">Type</span></span>|<span data-ttu-id="6aa72-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6aa72-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6aa72-133">оператионтипе</span><span class="sxs-lookup"><span data-stu-id="6aa72-133">operationType</span></span>|[<span data-ttu-id="6aa72-134">groupPolicyOperationType</span><span class="sxs-lookup"><span data-stu-id="6aa72-134">groupPolicyOperationType</span></span>](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|<span data-ttu-id="6aa72-135">Тип операции с групповой политикой.</span><span class="sxs-lookup"><span data-stu-id="6aa72-135">The type of group policy operation.</span></span> <span data-ttu-id="6aa72-136">Возможные значения: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span><span class="sxs-lookup"><span data-stu-id="6aa72-136">Possible values are: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span></span>|
|<span data-ttu-id="6aa72-137">оператионстатус</span><span class="sxs-lookup"><span data-stu-id="6aa72-137">operationStatus</span></span>|[<span data-ttu-id="6aa72-138">groupPolicyOperationStatus</span><span class="sxs-lookup"><span data-stu-id="6aa72-138">groupPolicyOperationStatus</span></span>](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|<span data-ttu-id="6aa72-139">Состояние операции групповой политики.</span><span class="sxs-lookup"><span data-stu-id="6aa72-139">The group policy operation status.</span></span> <span data-ttu-id="6aa72-140">Возможные значения: `unknown`, `inProgress`, `success`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="6aa72-140">Possible values are: `unknown`, `inProgress`, `success`, `failed`.</span></span>|
|<span data-ttu-id="6aa72-141">статусдетаилс</span><span class="sxs-lookup"><span data-stu-id="6aa72-141">statusDetails</span></span>|<span data-ttu-id="6aa72-142">String</span><span class="sxs-lookup"><span data-stu-id="6aa72-142">String</span></span>|<span data-ttu-id="6aa72-143">Сведения о состоянии операции групповой политики.</span><span class="sxs-lookup"><span data-stu-id="6aa72-143">The group policy operation status detail.</span></span>|
|<span data-ttu-id="6aa72-144">id</span><span class="sxs-lookup"><span data-stu-id="6aa72-144">id</span></span>|<span data-ttu-id="6aa72-145">String</span><span class="sxs-lookup"><span data-stu-id="6aa72-145">String</span></span>|<span data-ttu-id="6aa72-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6aa72-146">Key of the entity.</span></span>|
|<span data-ttu-id="6aa72-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6aa72-147">lastModifiedDateTime</span></span>|<span data-ttu-id="6aa72-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6aa72-148">DateTimeOffset</span></span>|<span data-ttu-id="6aa72-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6aa72-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="6aa72-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="6aa72-150">Response</span></span>
<span data-ttu-id="6aa72-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6aa72-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aa72-152">Пример</span><span class="sxs-lookup"><span data-stu-id="6aa72-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="6aa72-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="6aa72-153">Request</span></span>
<span data-ttu-id="6aa72-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6aa72-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6aa72-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="6aa72-155">Response</span></span>
<span data-ttu-id="6aa72-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6aa72-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



