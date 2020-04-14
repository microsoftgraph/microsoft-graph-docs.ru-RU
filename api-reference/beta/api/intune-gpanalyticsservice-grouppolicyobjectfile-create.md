---
title: Создание Граупполициобжектфиле
description: Создание нового объекта Граупполициобжектфиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: addb2ac25071618b01866065afac6c4389aa15cb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454941"
---
# <a name="create-grouppolicyobjectfile"></a><span data-ttu-id="2ac32-103">Создание Граупполициобжектфиле</span><span class="sxs-lookup"><span data-stu-id="2ac32-103">Create groupPolicyObjectFile</span></span>

<span data-ttu-id="2ac32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ac32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ac32-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ac32-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ac32-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ac32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ac32-107">Создание нового объекта [граупполициобжектфиле](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) .</span><span class="sxs-lookup"><span data-stu-id="2ac32-107">Create a new [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ac32-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2ac32-108">Prerequisites</span></span>
<span data-ttu-id="2ac32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ac32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ac32-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ac32-111">Permission type</span></span>|<span data-ttu-id="2ac32-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ac32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ac32-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ac32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ac32-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ac32-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2ac32-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ac32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ac32-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ac32-116">Not supported.</span></span>|
|<span data-ttu-id="2ac32-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ac32-117">Application</span></span>|<span data-ttu-id="2ac32-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ac32-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ac32-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ac32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyObjectFiles
```

## <a name="request-headers"></a><span data-ttu-id="2ac32-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2ac32-120">Request headers</span></span>
|<span data-ttu-id="2ac32-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ac32-121">Header</span></span>|<span data-ttu-id="2ac32-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2ac32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ac32-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ac32-123">Authorization</span></span>|<span data-ttu-id="2ac32-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ac32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ac32-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2ac32-125">Accept</span></span>|<span data-ttu-id="2ac32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ac32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ac32-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2ac32-127">Request body</span></span>
<span data-ttu-id="2ac32-128">В тексте запроса добавьте представление объекта Граупполициобжектфиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ac32-128">In the request body, supply a JSON representation for the groupPolicyObjectFile object.</span></span>

<span data-ttu-id="2ac32-129">В следующей таблице приведены свойства, необходимые при создании Граупполициобжектфиле.</span><span class="sxs-lookup"><span data-stu-id="2ac32-129">The following table shows the properties that are required when you create the groupPolicyObjectFile.</span></span>

|<span data-ttu-id="2ac32-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ac32-130">Property</span></span>|<span data-ttu-id="2ac32-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2ac32-131">Type</span></span>|<span data-ttu-id="2ac32-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2ac32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ac32-133">id</span><span class="sxs-lookup"><span data-stu-id="2ac32-133">id</span></span>|<span data-ttu-id="2ac32-134">String</span><span class="sxs-lookup"><span data-stu-id="2ac32-134">String</span></span>|<span data-ttu-id="2ac32-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2ac32-135">Not yet documented</span></span>|
|<span data-ttu-id="2ac32-136">граупполициобжектид</span><span class="sxs-lookup"><span data-stu-id="2ac32-136">groupPolicyObjectId</span></span>|<span data-ttu-id="2ac32-137">GUID</span><span class="sxs-lookup"><span data-stu-id="2ac32-137">Guid</span></span>|<span data-ttu-id="2ac32-138">GUID объекта групповой политики из XML-содержимого объекта групповой политики</span><span class="sxs-lookup"><span data-stu-id="2ac32-138">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="2ac32-139">аудистингуишеднаме</span><span class="sxs-lookup"><span data-stu-id="2ac32-139">ouDistinguishedName</span></span>|<span data-ttu-id="2ac32-140">String</span><span class="sxs-lookup"><span data-stu-id="2ac32-140">String</span></span>|<span data-ttu-id="2ac32-141">Различающееся имя подразделения.</span><span class="sxs-lookup"><span data-stu-id="2ac32-141">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="2ac32-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ac32-142">createdDateTime</span></span>|<span data-ttu-id="2ac32-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ac32-143">DateTimeOffset</span></span>|<span data-ttu-id="2ac32-144">Дата и время первой загрузки Граупполици.</span><span class="sxs-lookup"><span data-stu-id="2ac32-144">The date and time at which the GroupPolicy was first uploaded.</span></span>|
|<span data-ttu-id="2ac32-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ac32-145">lastModifiedDateTime</span></span>|<span data-ttu-id="2ac32-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ac32-146">DateTimeOffset</span></span>|<span data-ttu-id="2ac32-147">Дата и время последнего изменения Граупполициобжектфиле.</span><span class="sxs-lookup"><span data-stu-id="2ac32-147">The date and time at which the GroupPolicyObjectFile was last modified.</span></span>|
|<span data-ttu-id="2ac32-148">content</span><span class="sxs-lookup"><span data-stu-id="2ac32-148">content</span></span>|<span data-ttu-id="2ac32-149">String</span><span class="sxs-lookup"><span data-stu-id="2ac32-149">String</span></span>|<span data-ttu-id="2ac32-150">Содержимое файла объекта групповой политики.</span><span class="sxs-lookup"><span data-stu-id="2ac32-150">The Group Policy Object file content.</span></span>|



## <a name="response"></a><span data-ttu-id="2ac32-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ac32-151">Response</span></span>
<span data-ttu-id="2ac32-152">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполициобжектфиле](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ac32-152">If successful, this method returns a `201 Created` response code and a [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ac32-153">Пример</span><span class="sxs-lookup"><span data-stu-id="2ac32-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ac32-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ac32-154">Request</span></span>
<span data-ttu-id="2ac32-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ac32-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyObjectFiles
Content-type: application/json
Content-length: 217

{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "content": "Content value"
}
```

### <a name="response"></a><span data-ttu-id="2ac32-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ac32-156">Response</span></span>
<span data-ttu-id="2ac32-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ac32-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 389

{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "id": "65c0499d-499d-65c0-9d49-c0659d49c065",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "content": "Content value"
}
```



