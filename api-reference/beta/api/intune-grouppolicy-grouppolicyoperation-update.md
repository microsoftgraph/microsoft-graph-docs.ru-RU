---
title: Обновление Граупполициоператион
description: Обновление свойств объекта Граупполициоператион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3e47b04e84cf6c713036e4f519fb8b71819cf05f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48043264"
---
# <a name="update-grouppolicyoperation"></a><span data-ttu-id="5180b-103">Обновление Граупполициоператион</span><span class="sxs-lookup"><span data-stu-id="5180b-103">Update groupPolicyOperation</span></span>

<span data-ttu-id="5180b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5180b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5180b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5180b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5180b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5180b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5180b-107">Обновление свойств объекта [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="5180b-107">Update the properties of a [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5180b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5180b-108">Prerequisites</span></span>
<span data-ttu-id="5180b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5180b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5180b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5180b-111">Permission type</span></span>|<span data-ttu-id="5180b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5180b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5180b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5180b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5180b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5180b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5180b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5180b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5180b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5180b-116">Not supported.</span></span>|
|<span data-ttu-id="5180b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5180b-117">Application</span></span>|<span data-ttu-id="5180b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5180b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5180b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5180b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations/{groupPolicyOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="5180b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5180b-120">Request headers</span></span>
|<span data-ttu-id="5180b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5180b-121">Header</span></span>|<span data-ttu-id="5180b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5180b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5180b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5180b-123">Authorization</span></span>|<span data-ttu-id="5180b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5180b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5180b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5180b-125">Accept</span></span>|<span data-ttu-id="5180b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5180b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5180b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5180b-127">Request body</span></span>
<span data-ttu-id="5180b-128">В тексте запроса добавьте представление объекта [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5180b-128">In the request body, supply a JSON representation for the [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object.</span></span>

<span data-ttu-id="5180b-129">В следующей таблице приведены свойства, необходимые при создании [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md).</span><span class="sxs-lookup"><span data-stu-id="5180b-129">The following table shows the properties that are required when you create the [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md).</span></span>

|<span data-ttu-id="5180b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5180b-130">Property</span></span>|<span data-ttu-id="5180b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5180b-131">Type</span></span>|<span data-ttu-id="5180b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5180b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5180b-133">оператионтипе</span><span class="sxs-lookup"><span data-stu-id="5180b-133">operationType</span></span>|[<span data-ttu-id="5180b-134">groupPolicyOperationType</span><span class="sxs-lookup"><span data-stu-id="5180b-134">groupPolicyOperationType</span></span>](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|<span data-ttu-id="5180b-135">Тип операции с групповой политикой.</span><span class="sxs-lookup"><span data-stu-id="5180b-135">The type of group policy operation.</span></span> <span data-ttu-id="5180b-136">Возможные значения: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span><span class="sxs-lookup"><span data-stu-id="5180b-136">Possible values are: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.</span></span>|
|<span data-ttu-id="5180b-137">оператионстатус</span><span class="sxs-lookup"><span data-stu-id="5180b-137">operationStatus</span></span>|[<span data-ttu-id="5180b-138">groupPolicyOperationStatus</span><span class="sxs-lookup"><span data-stu-id="5180b-138">groupPolicyOperationStatus</span></span>](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|<span data-ttu-id="5180b-139">Состояние операции групповой политики.</span><span class="sxs-lookup"><span data-stu-id="5180b-139">The group policy operation status.</span></span> <span data-ttu-id="5180b-140">Возможные значения: `unknown`, `inProgress`, `success`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="5180b-140">Possible values are: `unknown`, `inProgress`, `success`, `failed`.</span></span>|
|<span data-ttu-id="5180b-141">статусдетаилс</span><span class="sxs-lookup"><span data-stu-id="5180b-141">statusDetails</span></span>|<span data-ttu-id="5180b-142">Строка</span><span class="sxs-lookup"><span data-stu-id="5180b-142">String</span></span>|<span data-ttu-id="5180b-143">Сведения о состоянии операции групповой политики.</span><span class="sxs-lookup"><span data-stu-id="5180b-143">The group policy operation status detail.</span></span>|
|<span data-ttu-id="5180b-144">id</span><span class="sxs-lookup"><span data-stu-id="5180b-144">id</span></span>|<span data-ttu-id="5180b-145">Строка</span><span class="sxs-lookup"><span data-stu-id="5180b-145">String</span></span>|<span data-ttu-id="5180b-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5180b-146">Key of the entity.</span></span>|
|<span data-ttu-id="5180b-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5180b-147">lastModifiedDateTime</span></span>|<span data-ttu-id="5180b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5180b-148">DateTimeOffset</span></span>|<span data-ttu-id="5180b-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5180b-149">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="5180b-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="5180b-150">Response</span></span>
<span data-ttu-id="5180b-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5180b-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5180b-152">Пример</span><span class="sxs-lookup"><span data-stu-id="5180b-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="5180b-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="5180b-153">Request</span></span>
<span data-ttu-id="5180b-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5180b-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5180b-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="5180b-155">Response</span></span>
<span data-ttu-id="5180b-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5180b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






