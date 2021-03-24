---
title: Создание policySet
description: Создание нового объекта policySet.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 864df7c89a6dbbcc80932e87f6616c79d52eca99
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134643"
---
# <a name="create-policyset"></a><span data-ttu-id="310f6-103">Создание policySet</span><span class="sxs-lookup"><span data-stu-id="310f6-103">Create policySet</span></span>

<span data-ttu-id="310f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="310f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="310f6-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="310f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="310f6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="310f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="310f6-107">Создание нового [объекта policySet.](../resources/intune-policyset-policyset.md)</span><span class="sxs-lookup"><span data-stu-id="310f6-107">Create a new [policySet](../resources/intune-policyset-policyset.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="310f6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="310f6-108">Prerequisites</span></span>
<span data-ttu-id="310f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="310f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="310f6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="310f6-111">Permission type</span></span>|<span data-ttu-id="310f6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="310f6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="310f6-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="310f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="310f6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="310f6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="310f6-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="310f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="310f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="310f6-116">Not supported.</span></span>|
|<span data-ttu-id="310f6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="310f6-117">Application</span></span>|<span data-ttu-id="310f6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="310f6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="310f6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="310f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets
```

## <a name="request-headers"></a><span data-ttu-id="310f6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="310f6-120">Request headers</span></span>
|<span data-ttu-id="310f6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="310f6-121">Header</span></span>|<span data-ttu-id="310f6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="310f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="310f6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="310f6-123">Authorization</span></span>|<span data-ttu-id="310f6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="310f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="310f6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="310f6-125">Accept</span></span>|<span data-ttu-id="310f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="310f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="310f6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="310f6-127">Request body</span></span>
<span data-ttu-id="310f6-128">В теле запроса поставляем представление JSON для объекта policySet.</span><span class="sxs-lookup"><span data-stu-id="310f6-128">In the request body, supply a JSON representation for the policySet object.</span></span>

<span data-ttu-id="310f6-129">В следующей таблице показаны свойства, необходимые при создании политикиSet.</span><span class="sxs-lookup"><span data-stu-id="310f6-129">The following table shows the properties that are required when you create the policySet.</span></span>

|<span data-ttu-id="310f6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="310f6-130">Property</span></span>|<span data-ttu-id="310f6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="310f6-131">Type</span></span>|<span data-ttu-id="310f6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="310f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="310f6-133">id</span><span class="sxs-lookup"><span data-stu-id="310f6-133">id</span></span>|<span data-ttu-id="310f6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="310f6-134">String</span></span>|<span data-ttu-id="310f6-135">Клавиша PolicySet.</span><span class="sxs-lookup"><span data-stu-id="310f6-135">Key of the PolicySet.</span></span>|
|<span data-ttu-id="310f6-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="310f6-136">createdDateTime</span></span>|<span data-ttu-id="310f6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="310f6-137">DateTimeOffset</span></span>|<span data-ttu-id="310f6-138">Время создания PolicySet.</span><span class="sxs-lookup"><span data-stu-id="310f6-138">Creation time of the PolicySet.</span></span>|
|<span data-ttu-id="310f6-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="310f6-139">lastModifiedDateTime</span></span>|<span data-ttu-id="310f6-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="310f6-140">DateTimeOffset</span></span>|<span data-ttu-id="310f6-141">Последнее измененное время в PolicySet.</span><span class="sxs-lookup"><span data-stu-id="310f6-141">Last modified time of the PolicySet.</span></span>|
|<span data-ttu-id="310f6-142">displayName</span><span class="sxs-lookup"><span data-stu-id="310f6-142">displayName</span></span>|<span data-ttu-id="310f6-143">Строка</span><span class="sxs-lookup"><span data-stu-id="310f6-143">String</span></span>|<span data-ttu-id="310f6-144">DisplayName of the PolicySet.</span><span class="sxs-lookup"><span data-stu-id="310f6-144">DisplayName of the PolicySet.</span></span>|
|<span data-ttu-id="310f6-145">description</span><span class="sxs-lookup"><span data-stu-id="310f6-145">description</span></span>|<span data-ttu-id="310f6-146">Строка</span><span class="sxs-lookup"><span data-stu-id="310f6-146">String</span></span>|<span data-ttu-id="310f6-147">Описание PolicySet.</span><span class="sxs-lookup"><span data-stu-id="310f6-147">Description of the PolicySet.</span></span>|
|<span data-ttu-id="310f6-148">status</span><span class="sxs-lookup"><span data-stu-id="310f6-148">status</span></span>|[<span data-ttu-id="310f6-149">policySetStatus</span><span class="sxs-lookup"><span data-stu-id="310f6-149">policySetStatus</span></span>](../resources/intune-policyset-policysetstatus.md)|<span data-ttu-id="310f6-150">Проверка/присвоение состояния PolicySet.</span><span class="sxs-lookup"><span data-stu-id="310f6-150">Validation/assignment status of the PolicySet.</span></span> <span data-ttu-id="310f6-151">Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="310f6-151">Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.</span></span>|
|<span data-ttu-id="310f6-152">errorCode</span><span class="sxs-lookup"><span data-stu-id="310f6-152">errorCode</span></span>|[<span data-ttu-id="310f6-153">errorCode</span><span class="sxs-lookup"><span data-stu-id="310f6-153">errorCode</span></span>](../resources/intune-policyset-errorcode.md)|<span data-ttu-id="310f6-154">Код ошибки, если таковое произошло.</span><span class="sxs-lookup"><span data-stu-id="310f6-154">Error code if any occured.</span></span> <span data-ttu-id="310f6-155">Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="310f6-155">Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.</span></span>|
|<span data-ttu-id="310f6-156">guidedDeploymentTags</span><span class="sxs-lookup"><span data-stu-id="310f6-156">guidedDeploymentTags</span></span>|<span data-ttu-id="310f6-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="310f6-157">String collection</span></span>|<span data-ttu-id="310f6-158">Теги управляемого развертывания</span><span class="sxs-lookup"><span data-stu-id="310f6-158">Tags of the guided deployment</span></span>|
|<span data-ttu-id="310f6-159">roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="310f6-159">roleScopeTags</span></span>|<span data-ttu-id="310f6-160">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="310f6-160">String collection</span></span>|<span data-ttu-id="310f6-161">RoleScopeTags of the PolicySet</span><span class="sxs-lookup"><span data-stu-id="310f6-161">RoleScopeTags of the PolicySet</span></span>|



## <a name="response"></a><span data-ttu-id="310f6-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="310f6-162">Response</span></span>
<span data-ttu-id="310f6-163">В случае успешной работы этот метод возвращает код ответа и `201 Created` объект [policySet](../resources/intune-policyset-policyset.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="310f6-163">If successful, this method returns a `201 Created` response code and a [policySet](../resources/intune-policyset-policyset.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="310f6-164">Пример</span><span class="sxs-lookup"><span data-stu-id="310f6-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="310f6-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="310f6-165">Request</span></span>
<span data-ttu-id="310f6-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="310f6-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="310f6-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="310f6-167">Response</span></span>
<span data-ttu-id="310f6-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="310f6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




