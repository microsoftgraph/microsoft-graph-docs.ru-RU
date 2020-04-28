---
title: Создание политики
description: Создайте новый объект Policy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 22a1d700b0f82cb98876e4fadb439ee5010fed12
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456294"
---
# <a name="create-policyset"></a><span data-ttu-id="e8bf5-103">Создание политики</span><span class="sxs-lookup"><span data-stu-id="e8bf5-103">Create policySet</span></span>

<span data-ttu-id="e8bf5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8bf5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8bf5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8bf5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8bf5-107">Создайте новый объект [Policy](../resources/intune-policyset-policyset.md) .</span><span class="sxs-lookup"><span data-stu-id="e8bf5-107">Create a new [policySet](../resources/intune-policyset-policyset.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8bf5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e8bf5-108">Prerequisites</span></span>
<span data-ttu-id="e8bf5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8bf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8bf5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8bf5-111">Permission type</span></span>|<span data-ttu-id="e8bf5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8bf5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8bf5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8bf5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8bf5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8bf5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8bf5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8bf5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8bf5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-116">Not supported.</span></span>|
|<span data-ttu-id="e8bf5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8bf5-117">Application</span></span>|<span data-ttu-id="e8bf5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8bf5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8bf5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8bf5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets
```

## <a name="request-headers"></a><span data-ttu-id="e8bf5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e8bf5-120">Request headers</span></span>
|<span data-ttu-id="e8bf5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8bf5-121">Header</span></span>|<span data-ttu-id="e8bf5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e8bf5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8bf5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8bf5-123">Authorization</span></span>|<span data-ttu-id="e8bf5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8bf5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e8bf5-125">Accept</span></span>|<span data-ttu-id="e8bf5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8bf5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8bf5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e8bf5-127">Request body</span></span>
<span data-ttu-id="e8bf5-128">В тексте запроса добавьте представление объекта Policy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-128">In the request body, supply a JSON representation for the policySet object.</span></span>

<span data-ttu-id="e8bf5-129">В следующей таблице приведены свойства, необходимые при создании этого параметра.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-129">The following table shows the properties that are required when you create the policySet.</span></span>

|<span data-ttu-id="e8bf5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8bf5-130">Property</span></span>|<span data-ttu-id="e8bf5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e8bf5-131">Type</span></span>|<span data-ttu-id="e8bf5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e8bf5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8bf5-133">id</span><span class="sxs-lookup"><span data-stu-id="e8bf5-133">id</span></span>|<span data-ttu-id="e8bf5-134">String</span><span class="sxs-lookup"><span data-stu-id="e8bf5-134">String</span></span>|<span data-ttu-id="e8bf5-135">Ключ набора политик.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-135">Key of the PolicySet.</span></span>|
|<span data-ttu-id="e8bf5-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8bf5-136">createdDateTime</span></span>|<span data-ttu-id="e8bf5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8bf5-137">DateTimeOffset</span></span>|<span data-ttu-id="e8bf5-138">Время создания набора политик.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-138">Creation time of the PolicySet.</span></span>|
|<span data-ttu-id="e8bf5-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8bf5-139">lastModifiedDateTime</span></span>|<span data-ttu-id="e8bf5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8bf5-140">DateTimeOffset</span></span>|<span data-ttu-id="e8bf5-141">Время последнего изменения набора политик.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-141">Last modified time of the PolicySet.</span></span>|
|<span data-ttu-id="e8bf5-142">displayName</span><span class="sxs-lookup"><span data-stu-id="e8bf5-142">displayName</span></span>|<span data-ttu-id="e8bf5-143">Строка</span><span class="sxs-lookup"><span data-stu-id="e8bf5-143">String</span></span>|<span data-ttu-id="e8bf5-144">DisplayName набора политик.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-144">DisplayName of the PolicySet.</span></span>|
|<span data-ttu-id="e8bf5-145">description</span><span class="sxs-lookup"><span data-stu-id="e8bf5-145">description</span></span>|<span data-ttu-id="e8bf5-146">String</span><span class="sxs-lookup"><span data-stu-id="e8bf5-146">String</span></span>|<span data-ttu-id="e8bf5-147">Описание набора политик.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-147">Description of the PolicySet.</span></span>|
|<span data-ttu-id="e8bf5-148">status</span><span class="sxs-lookup"><span data-stu-id="e8bf5-148">status</span></span>|[<span data-ttu-id="e8bf5-149">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="e8bf5-149">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="e8bf5-150">Состояние проверки или назначения набора политик.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-150">Validation/assignment status of the PolicySet.</span></span> <span data-ttu-id="e8bf5-151">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-151">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="e8bf5-152">errorCode</span><span class="sxs-lookup"><span data-stu-id="e8bf5-152">errorCode</span></span>|[<span data-ttu-id="e8bf5-153">errorCode</span><span class="sxs-lookup"><span data-stu-id="e8bf5-153">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="e8bf5-154">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="e8bf5-154">Error code if any occured.</span></span> <span data-ttu-id="e8bf5-155">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-155">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="e8bf5-156">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="e8bf5-156">guidedDeploymentTags</span></span>|<span data-ttu-id="e8bf5-157">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e8bf5-157">String collection</span></span>|<span data-ttu-id="e8bf5-158">Теги в руководстве по развертыванию</span><span class="sxs-lookup"><span data-stu-id="e8bf5-158">Tags of the guided deployment</span></span>|
|<span data-ttu-id="e8bf5-159">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="e8bf5-159">roleScopeTags</span></span>|<span data-ttu-id="e8bf5-160">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e8bf5-160">String collection</span></span>|<span data-ttu-id="e8bf5-161">RoleScopeTags набора политик</span><span class="sxs-lookup"><span data-stu-id="e8bf5-161">RoleScopeTags of the PolicySet</span></span>|



## <a name="response"></a><span data-ttu-id="e8bf5-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="e8bf5-162">Response</span></span>
<span data-ttu-id="e8bf5-163">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Policy](../resources/intune-policyset-policyset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-163">If successful, this method returns a `201 Created` response code and a [policySet](../resources/intune-policyset-policyset.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8bf5-164">Пример</span><span class="sxs-lookup"><span data-stu-id="e8bf5-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8bf5-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8bf5-165">Request</span></span>
<span data-ttu-id="e8bf5-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e8bf5-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8bf5-167">Response</span></span>
<span data-ttu-id="e8bf5-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8bf5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



