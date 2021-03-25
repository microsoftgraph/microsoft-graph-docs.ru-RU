---
title: Update groupPolicyObjectFile
description: Обновление свойств объекта groupPolicyObjectFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efe599f7b894629ca4b1b1d5c2d3492b76bc9b9e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158964"
---
# <a name="update-grouppolicyobjectfile"></a><span data-ttu-id="2601e-103">Update groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="2601e-103">Update groupPolicyObjectFile</span></span>

<span data-ttu-id="2601e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2601e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2601e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2601e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2601e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2601e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2601e-107">Обновление свойств объекта [groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)</span><span class="sxs-lookup"><span data-stu-id="2601e-107">Update the properties of a [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2601e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2601e-108">Prerequisites</span></span>
<span data-ttu-id="2601e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2601e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2601e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2601e-111">Permission type</span></span>|<span data-ttu-id="2601e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2601e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2601e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2601e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2601e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2601e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2601e-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2601e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2601e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2601e-116">Not supported.</span></span>|
|<span data-ttu-id="2601e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2601e-117">Application</span></span>|<span data-ttu-id="2601e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2601e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2601e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2601e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyObjectFiles/{groupPolicyObjectFileId}
```

## <a name="request-headers"></a><span data-ttu-id="2601e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2601e-120">Request headers</span></span>
|<span data-ttu-id="2601e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2601e-121">Header</span></span>|<span data-ttu-id="2601e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2601e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2601e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2601e-123">Authorization</span></span>|<span data-ttu-id="2601e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2601e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2601e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2601e-125">Accept</span></span>|<span data-ttu-id="2601e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2601e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2601e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2601e-127">Request body</span></span>
<span data-ttu-id="2601e-128">В теле запроса поставляем представление JSON для [объекта groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)</span><span class="sxs-lookup"><span data-stu-id="2601e-128">In the request body, supply a JSON representation for the [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object.</span></span>

<span data-ttu-id="2601e-129">В следующей таблице показаны свойства, необходимые при создании [groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)</span><span class="sxs-lookup"><span data-stu-id="2601e-129">The following table shows the properties that are required when you create the [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md).</span></span>

|<span data-ttu-id="2601e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2601e-130">Property</span></span>|<span data-ttu-id="2601e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2601e-131">Type</span></span>|<span data-ttu-id="2601e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2601e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2601e-133">id</span><span class="sxs-lookup"><span data-stu-id="2601e-133">id</span></span>|<span data-ttu-id="2601e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2601e-134">String</span></span>|<span data-ttu-id="2601e-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="2601e-135">Not yet documented</span></span>|
|<span data-ttu-id="2601e-136">groupPolicyObjectId</span><span class="sxs-lookup"><span data-stu-id="2601e-136">groupPolicyObjectId</span></span>|<span data-ttu-id="2601e-137">Guid</span><span class="sxs-lookup"><span data-stu-id="2601e-137">Guid</span></span>|<span data-ttu-id="2601e-138">GUID объекта групповой политики из контента GPO Xml</span><span class="sxs-lookup"><span data-stu-id="2601e-138">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="2601e-139">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="2601e-139">ouDistinguishedName</span></span>|<span data-ttu-id="2601e-140">Строка</span><span class="sxs-lookup"><span data-stu-id="2601e-140">String</span></span>|<span data-ttu-id="2601e-141">Отличительное имя OU.</span><span class="sxs-lookup"><span data-stu-id="2601e-141">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="2601e-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2601e-142">createdDateTime</span></span>|<span data-ttu-id="2601e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2601e-143">DateTimeOffset</span></span>|<span data-ttu-id="2601e-144">Дата и время, в которые была впервые загружена GroupPolicy.</span><span class="sxs-lookup"><span data-stu-id="2601e-144">The date and time at which the GroupPolicy was first uploaded.</span></span>|
|<span data-ttu-id="2601e-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2601e-145">lastModifiedDateTime</span></span>|<span data-ttu-id="2601e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2601e-146">DateTimeOffset</span></span>|<span data-ttu-id="2601e-147">Дата и время последнего изменения GroupPolicyObjectFile.</span><span class="sxs-lookup"><span data-stu-id="2601e-147">The date and time at which the GroupPolicyObjectFile was last modified.</span></span>|
|<span data-ttu-id="2601e-148">content</span><span class="sxs-lookup"><span data-stu-id="2601e-148">content</span></span>|<span data-ttu-id="2601e-149">String</span><span class="sxs-lookup"><span data-stu-id="2601e-149">String</span></span>|<span data-ttu-id="2601e-150">Контент объекта групповой политики.</span><span class="sxs-lookup"><span data-stu-id="2601e-150">The Group Policy Object file content.</span></span>|



## <a name="response"></a><span data-ttu-id="2601e-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="2601e-151">Response</span></span>
<span data-ttu-id="2601e-152">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2601e-152">If successful, this method returns a `200 OK` response code and an updated [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2601e-153">Пример</span><span class="sxs-lookup"><span data-stu-id="2601e-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="2601e-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="2601e-154">Request</span></span>
<span data-ttu-id="2601e-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2601e-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2601e-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="2601e-156">Response</span></span>
<span data-ttu-id="2601e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2601e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




