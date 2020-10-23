---
title: Обновление Граупполициобжектфиле
description: Обновление свойств объекта Граупполициобжектфиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b266b110a0512539018815c0bf4f3cd33700fb3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692998"
---
# <a name="update-grouppolicyobjectfile"></a><span data-ttu-id="dcb68-103">Обновление Граупполициобжектфиле</span><span class="sxs-lookup"><span data-stu-id="dcb68-103">Update groupPolicyObjectFile</span></span>

<span data-ttu-id="dcb68-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcb68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dcb68-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcb68-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcb68-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dcb68-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcb68-107">Обновление свойств объекта [граупполициобжектфиле](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) .</span><span class="sxs-lookup"><span data-stu-id="dcb68-107">Update the properties of a [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcb68-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dcb68-108">Prerequisites</span></span>
<span data-ttu-id="dcb68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcb68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcb68-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dcb68-111">Permission type</span></span>|<span data-ttu-id="dcb68-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dcb68-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcb68-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dcb68-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dcb68-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcb68-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dcb68-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dcb68-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcb68-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcb68-116">Not supported.</span></span>|
|<span data-ttu-id="dcb68-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dcb68-117">Application</span></span>|<span data-ttu-id="dcb68-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcb68-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcb68-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dcb68-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyObjectFiles/{groupPolicyObjectFileId}
```

## <a name="request-headers"></a><span data-ttu-id="dcb68-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dcb68-120">Request headers</span></span>
|<span data-ttu-id="dcb68-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dcb68-121">Header</span></span>|<span data-ttu-id="dcb68-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dcb68-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcb68-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dcb68-123">Authorization</span></span>|<span data-ttu-id="dcb68-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dcb68-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcb68-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dcb68-125">Accept</span></span>|<span data-ttu-id="dcb68-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dcb68-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcb68-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dcb68-127">Request body</span></span>
<span data-ttu-id="dcb68-128">В тексте запроса добавьте представление объекта [граупполициобжектфиле](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dcb68-128">In the request body, supply a JSON representation for the [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object.</span></span>

<span data-ttu-id="dcb68-129">В следующей таблице приведены свойства, необходимые при создании [граупполициобжектфиле](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md).</span><span class="sxs-lookup"><span data-stu-id="dcb68-129">The following table shows the properties that are required when you create the [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md).</span></span>

|<span data-ttu-id="dcb68-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dcb68-130">Property</span></span>|<span data-ttu-id="dcb68-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dcb68-131">Type</span></span>|<span data-ttu-id="dcb68-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dcb68-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcb68-133">id</span><span class="sxs-lookup"><span data-stu-id="dcb68-133">id</span></span>|<span data-ttu-id="dcb68-134">Строка</span><span class="sxs-lookup"><span data-stu-id="dcb68-134">String</span></span>|<span data-ttu-id="dcb68-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dcb68-135">Not yet documented</span></span>|
|<span data-ttu-id="dcb68-136">граупполициобжектид</span><span class="sxs-lookup"><span data-stu-id="dcb68-136">groupPolicyObjectId</span></span>|<span data-ttu-id="dcb68-137">Guid</span><span class="sxs-lookup"><span data-stu-id="dcb68-137">Guid</span></span>|<span data-ttu-id="dcb68-138">GUID объекта групповой политики из XML-содержимого объекта групповой политики</span><span class="sxs-lookup"><span data-stu-id="dcb68-138">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="dcb68-139">аудистингуишеднаме</span><span class="sxs-lookup"><span data-stu-id="dcb68-139">ouDistinguishedName</span></span>|<span data-ttu-id="dcb68-140">Строка</span><span class="sxs-lookup"><span data-stu-id="dcb68-140">String</span></span>|<span data-ttu-id="dcb68-141">Различающееся имя подразделения.</span><span class="sxs-lookup"><span data-stu-id="dcb68-141">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="dcb68-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dcb68-142">createdDateTime</span></span>|<span data-ttu-id="dcb68-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcb68-143">DateTimeOffset</span></span>|<span data-ttu-id="dcb68-144">Дата и время первой загрузки Граупполици.</span><span class="sxs-lookup"><span data-stu-id="dcb68-144">The date and time at which the GroupPolicy was first uploaded.</span></span>|
|<span data-ttu-id="dcb68-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dcb68-145">lastModifiedDateTime</span></span>|<span data-ttu-id="dcb68-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcb68-146">DateTimeOffset</span></span>|<span data-ttu-id="dcb68-147">Дата и время последнего изменения Граупполициобжектфиле.</span><span class="sxs-lookup"><span data-stu-id="dcb68-147">The date and time at which the GroupPolicyObjectFile was last modified.</span></span>|
|<span data-ttu-id="dcb68-148">content</span><span class="sxs-lookup"><span data-stu-id="dcb68-148">content</span></span>|<span data-ttu-id="dcb68-149">String</span><span class="sxs-lookup"><span data-stu-id="dcb68-149">String</span></span>|<span data-ttu-id="dcb68-150">Содержимое файла объекта групповой политики.</span><span class="sxs-lookup"><span data-stu-id="dcb68-150">The Group Policy Object file content.</span></span>|



## <a name="response"></a><span data-ttu-id="dcb68-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="dcb68-151">Response</span></span>
<span data-ttu-id="dcb68-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициобжектфиле](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dcb68-152">If successful, this method returns a `200 OK` response code and an updated [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcb68-153">Пример</span><span class="sxs-lookup"><span data-stu-id="dcb68-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcb68-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="dcb68-154">Request</span></span>
<span data-ttu-id="dcb68-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dcb68-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyObjectFiles/{groupPolicyObjectFileId}
Content-type: application/json
Content-length: 217

{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "content": "Content value"
}
```

### <a name="response"></a><span data-ttu-id="dcb68-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcb68-156">Response</span></span>
<span data-ttu-id="dcb68-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dcb68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





