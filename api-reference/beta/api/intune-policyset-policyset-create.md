---
title: Создание политики
description: Создайте новый объект Policy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 289701c0f1db1d479d80a5d205a0101456cd1f38
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940982"
---
# <a name="create-policyset"></a><span data-ttu-id="958b3-103">Создание политики</span><span class="sxs-lookup"><span data-stu-id="958b3-103">Create policySet</span></span>

> <span data-ttu-id="958b3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="958b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="958b3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="958b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="958b3-106">Создайте новый объект [Policy](../resources/intune-policyset-policyset.md) .</span><span class="sxs-lookup"><span data-stu-id="958b3-106">Create a new [policySet](../resources/intune-policyset-policyset.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="958b3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="958b3-107">Prerequisites</span></span>
<span data-ttu-id="958b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="958b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="958b3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="958b3-110">Permission type</span></span>|<span data-ttu-id="958b3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="958b3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="958b3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="958b3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="958b3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="958b3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="958b3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="958b3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="958b3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="958b3-115">Not supported.</span></span>|
|<span data-ttu-id="958b3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="958b3-116">Application</span></span>|<span data-ttu-id="958b3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="958b3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="958b3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="958b3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets
```

## <a name="request-headers"></a><span data-ttu-id="958b3-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="958b3-119">Request headers</span></span>
|<span data-ttu-id="958b3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="958b3-120">Header</span></span>|<span data-ttu-id="958b3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="958b3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="958b3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="958b3-122">Authorization</span></span>|<span data-ttu-id="958b3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="958b3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="958b3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="958b3-124">Accept</span></span>|<span data-ttu-id="958b3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="958b3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="958b3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="958b3-126">Request body</span></span>
<span data-ttu-id="958b3-127">В тексте запроса добавьте представление объекта Policy в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="958b3-127">In the request body, supply a JSON representation for the policySet object.</span></span>

<span data-ttu-id="958b3-128">В следующей таблице приведены свойства, необходимые при создании этого параметра.</span><span class="sxs-lookup"><span data-stu-id="958b3-128">The following table shows the properties that are required when you create the policySet.</span></span>

|<span data-ttu-id="958b3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="958b3-129">Property</span></span>|<span data-ttu-id="958b3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="958b3-130">Type</span></span>|<span data-ttu-id="958b3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="958b3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="958b3-132">id</span><span class="sxs-lookup"><span data-stu-id="958b3-132">id</span></span>|<span data-ttu-id="958b3-133">String</span><span class="sxs-lookup"><span data-stu-id="958b3-133">String</span></span>|<span data-ttu-id="958b3-134">Ключ набора политик.</span><span class="sxs-lookup"><span data-stu-id="958b3-134">Key of the PolicySet.</span></span>|
|<span data-ttu-id="958b3-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="958b3-135">createdDateTime</span></span>|<span data-ttu-id="958b3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="958b3-136">DateTimeOffset</span></span>|<span data-ttu-id="958b3-137">Время создания набора политик.</span><span class="sxs-lookup"><span data-stu-id="958b3-137">Creation time of the PolicySet.</span></span>|
|<span data-ttu-id="958b3-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="958b3-138">lastModifiedDateTime</span></span>|<span data-ttu-id="958b3-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="958b3-139">DateTimeOffset</span></span>|<span data-ttu-id="958b3-140">Время последнего изменения набора политик.</span><span class="sxs-lookup"><span data-stu-id="958b3-140">Last modified time of the PolicySet.</span></span>|
|<span data-ttu-id="958b3-141">displayName</span><span class="sxs-lookup"><span data-stu-id="958b3-141">displayName</span></span>|<span data-ttu-id="958b3-142">Строка</span><span class="sxs-lookup"><span data-stu-id="958b3-142">String</span></span>|<span data-ttu-id="958b3-143">DisplayName набора политик.</span><span class="sxs-lookup"><span data-stu-id="958b3-143">DisplayName of the PolicySet.</span></span>|
|<span data-ttu-id="958b3-144">description</span><span class="sxs-lookup"><span data-stu-id="958b3-144">description</span></span>|<span data-ttu-id="958b3-145">String</span><span class="sxs-lookup"><span data-stu-id="958b3-145">String</span></span>|<span data-ttu-id="958b3-146">Описание набора политик.</span><span class="sxs-lookup"><span data-stu-id="958b3-146">Description of the PolicySet.</span></span>|
|<span data-ttu-id="958b3-147">status</span><span class="sxs-lookup"><span data-stu-id="958b3-147">status</span></span>|[<span data-ttu-id="958b3-148">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="958b3-148">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="958b3-149">Состояние проверки или назначения набора политик.</span><span class="sxs-lookup"><span data-stu-id="958b3-149">Validation/assignment status of the PolicySet.</span></span> <span data-ttu-id="958b3-150">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="958b3-150">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="958b3-151">errorCode</span><span class="sxs-lookup"><span data-stu-id="958b3-151">errorCode</span></span>|[<span data-ttu-id="958b3-152">errorCode</span><span class="sxs-lookup"><span data-stu-id="958b3-152">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="958b3-153">Код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="958b3-153">Error code if any occured.</span></span> <span data-ttu-id="958b3-154">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="958b3-154">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="958b3-155">гуидеддеплойменттагс</span><span class="sxs-lookup"><span data-stu-id="958b3-155">guidedDeploymentTags</span></span>|<span data-ttu-id="958b3-156">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="958b3-156">String collection</span></span>|<span data-ttu-id="958b3-157">Теги в руководстве по развертыванию</span><span class="sxs-lookup"><span data-stu-id="958b3-157">Tags of the guided deployment</span></span>|
|<span data-ttu-id="958b3-158">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="958b3-158">roleScopeTags</span></span>|<span data-ttu-id="958b3-159">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="958b3-159">String collection</span></span>|<span data-ttu-id="958b3-160">RoleScopeTags набора политик</span><span class="sxs-lookup"><span data-stu-id="958b3-160">RoleScopeTags of the PolicySet</span></span>|



## <a name="response"></a><span data-ttu-id="958b3-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="958b3-161">Response</span></span>
<span data-ttu-id="958b3-162">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Policy](../resources/intune-policyset-policyset.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="958b3-162">If successful, this method returns a `201 Created` response code and a [policySet](../resources/intune-policyset-policyset.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="958b3-163">Пример</span><span class="sxs-lookup"><span data-stu-id="958b3-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="958b3-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="958b3-164">Request</span></span>
<span data-ttu-id="958b3-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="958b3-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="958b3-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="958b3-166">Response</span></span>
<span data-ttu-id="958b3-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="958b3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





