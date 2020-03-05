---
title: Создание политики
description: Создайте новый объект Policy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1bb85838c8a5271a7fced4c2ad27bddfdb1b6ebc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460670"
---
# <a name="create-policyset"></a><span data-ttu-id="820df-103">Создание политики</span><span class="sxs-lookup"><span data-stu-id="820df-103">Create policySet</span></span>

<span data-ttu-id="820df-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="820df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="820df-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="820df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="820df-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="820df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="820df-107">Создайте новый объект [Policy](../resources/intune-policyset-policyset.md) .</span><span class="sxs-lookup"><span data-stu-id="820df-107">Create a new [policySet](../resources/intune-policyset-policyset.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="820df-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="820df-108">Prerequisites</span></span>
<span data-ttu-id="820df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="820df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="820df-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="820df-111">Permission type</span></span>|<span data-ttu-id="820df-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="820df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="820df-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="820df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="820df-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="820df-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="820df-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="820df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="820df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="820df-116">Not supported.</span></span>|
|<span data-ttu-id="820df-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="820df-117">Application</span></span>|<span data-ttu-id="820df-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="820df-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="820df-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="820df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets
```

## <a name="request-headers"></a><span data-ttu-id="820df-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="820df-120">Request headers</span></span>
|<span data-ttu-id="820df-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="820df-121">Header</span></span>|<span data-ttu-id="820df-122">Значение</span><span class="sxs-lookup"><span data-stu-id="820df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="820df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="820df-123">Authorization</span></span>|<span data-ttu-id="820df-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="820df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="820df-125">Accept</span><span class="sxs-lookup"><span data-stu-id="820df-125">Accept</span></span>|<span data-ttu-id="820df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="820df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="820df-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="820df-127">Request body</span></span>
<span data-ttu-id="820df-128">В тексте запроса добавьте представление объекта Policy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="820df-128">In the request body, supply a JSON representation for the policySet object.</span></span>

<span data-ttu-id="820df-129">В следующей таблице приведены свойства, необходимые при создании этого параметра.</span><span class="sxs-lookup"><span data-stu-id="820df-129">The following table shows the properties that are required when you create the policySet.</span></span>

|<span data-ttu-id="820df-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="820df-130">Property</span></span>|<span data-ttu-id="820df-131">Тип</span><span class="sxs-lookup"><span data-stu-id="820df-131">Type</span></span>|<span data-ttu-id="820df-132">Описание</span><span class="sxs-lookup"><span data-stu-id="820df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="820df-133">id</span><span class="sxs-lookup"><span data-stu-id="820df-133">id</span></span>|<span data-ttu-id="820df-134">String</span><span class="sxs-lookup"><span data-stu-id="820df-134">String</span></span>|<span data-ttu-id="820df-135">Ключ набора политик.</span><span class="sxs-lookup"><span data-stu-id="820df-135">Key of the PolicySet.</span></span>|
|<span data-ttu-id="820df-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="820df-136">createdDateTime</span></span>|<span data-ttu-id="820df-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="820df-137">DateTimeOffset</span></span>|<span data-ttu-id="820df-138">Время создания набора политик.</span><span class="sxs-lookup"><span data-stu-id="820df-138">Creation time of the PolicySet.</span></span>|
|<span data-ttu-id="820df-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="820df-139">lastModifiedDateTime</span></span>|<span data-ttu-id="820df-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="820df-140">DateTimeOffset</span></span>|<span data-ttu-id="820df-141">Время последнего изменения набора политик.</span><span class="sxs-lookup"><span data-stu-id="820df-141">Last modified time of the PolicySet.</span></span>|
|<span data-ttu-id="820df-142">displayName</span><span class="sxs-lookup"><span data-stu-id="820df-142">displayName</span></span>|<span data-ttu-id="820df-143">Строка</span><span class="sxs-lookup"><span data-stu-id="820df-143">String</span></span>|<span data-ttu-id="820df-144">DisplayName набора политик.</span><span class="sxs-lookup"><span data-stu-id="820df-144">DisplayName of the PolicySet.</span></span>|
|<span data-ttu-id="820df-145">description</span><span class="sxs-lookup"><span data-stu-id="820df-145">description</span></span>|<span data-ttu-id="820df-146">String</span><span class="sxs-lookup"><span data-stu-id="820df-146">String</span></span>|<span data-ttu-id="820df-147">Описание набора политик.</span><span class="sxs-lookup"><span data-stu-id="820df-147">Description of the PolicySet.</span></span>|
|<span data-ttu-id="820df-148">status</span><span class="sxs-lookup"><span data-stu-id="820df-148">status</span></span>|[<span data-ttu-id="820df-149">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="820df-149">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="820df-150">Состояние проверки или назначения набора политик.</span><span class="sxs-lookup"><span data-stu-id="820df-150">Validation/assignment status of the PolicySet.</span></span> <span data-ttu-id="820df-151">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="820df-151">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="820df-152">errorCode</span><span class="sxs-lookup"><span data-stu-id="820df-152">errorCode</span></span>|[<span data-ttu-id="820df-153">errorCode</span><span class="sxs-lookup"><span data-stu-id="820df-153">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="820df-154">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="820df-154">Error code if any occured.</span></span> <span data-ttu-id="820df-155">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="820df-155">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="820df-156">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="820df-156">guidedDeploymentTags</span></span>|<span data-ttu-id="820df-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="820df-157">String collection</span></span>|<span data-ttu-id="820df-158">Теги в руководстве по развертыванию</span><span class="sxs-lookup"><span data-stu-id="820df-158">Tags of the guided deployment</span></span>|
|<span data-ttu-id="820df-159">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="820df-159">roleScopeTags</span></span>|<span data-ttu-id="820df-160">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="820df-160">String collection</span></span>|<span data-ttu-id="820df-161">RoleScopeTags набора политик</span><span class="sxs-lookup"><span data-stu-id="820df-161">RoleScopeTags of the PolicySet</span></span>|



## <a name="response"></a><span data-ttu-id="820df-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="820df-162">Response</span></span>
<span data-ttu-id="820df-163">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Policy](../resources/intune-policyset-policyset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="820df-163">If successful, this method returns a `201 Created` response code and a [policySet](../resources/intune-policyset-policyset.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="820df-164">Пример</span><span class="sxs-lookup"><span data-stu-id="820df-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="820df-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="820df-165">Request</span></span>
<span data-ttu-id="820df-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="820df-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets
Content-type: application/json
Content-length: 317

{
  "@odata.type": "#microsoft.graph.policySet",
  "displayName": "Display Name value",
  "description": "Description value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="820df-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="820df-167">Response</span></span>
<span data-ttu-id="820df-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="820df-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.policySet",
  "id": "653cb373-b373-653c-73b3-3c6573b33c65",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "roleScopeTags": [
    "Role Scope Tags value"
  ]
}
```





