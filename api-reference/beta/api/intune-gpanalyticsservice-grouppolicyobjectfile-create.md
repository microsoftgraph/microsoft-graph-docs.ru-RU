---
title: Создание groupPolicyObjectFile
description: Создайте новый объект groupPolicyObjectFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a321b735313373b0d412d722edd849eb1370a2ca
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158999"
---
# <a name="create-grouppolicyobjectfile"></a><span data-ttu-id="43df4-103">Создание groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="43df4-103">Create groupPolicyObjectFile</span></span>

<span data-ttu-id="43df4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43df4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43df4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43df4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43df4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43df4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43df4-107">Создайте новый [объект groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)</span><span class="sxs-lookup"><span data-stu-id="43df4-107">Create a new [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43df4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="43df4-108">Prerequisites</span></span>
<span data-ttu-id="43df4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43df4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43df4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43df4-111">Permission type</span></span>|<span data-ttu-id="43df4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43df4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43df4-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43df4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43df4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43df4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43df4-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43df4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43df4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43df4-116">Not supported.</span></span>|
|<span data-ttu-id="43df4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="43df4-117">Application</span></span>|<span data-ttu-id="43df4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43df4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43df4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43df4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyObjectFiles
```

## <a name="request-headers"></a><span data-ttu-id="43df4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="43df4-120">Request headers</span></span>
|<span data-ttu-id="43df4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43df4-121">Header</span></span>|<span data-ttu-id="43df4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="43df4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43df4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43df4-123">Authorization</span></span>|<span data-ttu-id="43df4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43df4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43df4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="43df4-125">Accept</span></span>|<span data-ttu-id="43df4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43df4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43df4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43df4-127">Request body</span></span>
<span data-ttu-id="43df4-128">В теле запроса поставляем представление JSON для объекта groupPolicyObjectFile.</span><span class="sxs-lookup"><span data-stu-id="43df4-128">In the request body, supply a JSON representation for the groupPolicyObjectFile object.</span></span>

<span data-ttu-id="43df4-129">В следующей таблице показаны свойства, необходимые при создании groupPolicyObjectFile.</span><span class="sxs-lookup"><span data-stu-id="43df4-129">The following table shows the properties that are required when you create the groupPolicyObjectFile.</span></span>

|<span data-ttu-id="43df4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="43df4-130">Property</span></span>|<span data-ttu-id="43df4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="43df4-131">Type</span></span>|<span data-ttu-id="43df4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="43df4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43df4-133">id</span><span class="sxs-lookup"><span data-stu-id="43df4-133">id</span></span>|<span data-ttu-id="43df4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="43df4-134">String</span></span>|<span data-ttu-id="43df4-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="43df4-135">Not yet documented</span></span>|
|<span data-ttu-id="43df4-136">groupPolicyObjectId</span><span class="sxs-lookup"><span data-stu-id="43df4-136">groupPolicyObjectId</span></span>|<span data-ttu-id="43df4-137">Guid</span><span class="sxs-lookup"><span data-stu-id="43df4-137">Guid</span></span>|<span data-ttu-id="43df4-138">GUID объекта групповой политики из контента GPO Xml</span><span class="sxs-lookup"><span data-stu-id="43df4-138">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="43df4-139">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="43df4-139">ouDistinguishedName</span></span>|<span data-ttu-id="43df4-140">Строка</span><span class="sxs-lookup"><span data-stu-id="43df4-140">String</span></span>|<span data-ttu-id="43df4-141">Отличительное имя OU.</span><span class="sxs-lookup"><span data-stu-id="43df4-141">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="43df4-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43df4-142">createdDateTime</span></span>|<span data-ttu-id="43df4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43df4-143">DateTimeOffset</span></span>|<span data-ttu-id="43df4-144">Дата и время, в которые была впервые загружена GroupPolicy.</span><span class="sxs-lookup"><span data-stu-id="43df4-144">The date and time at which the GroupPolicy was first uploaded.</span></span>|
|<span data-ttu-id="43df4-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43df4-145">lastModifiedDateTime</span></span>|<span data-ttu-id="43df4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43df4-146">DateTimeOffset</span></span>|<span data-ttu-id="43df4-147">Дата и время последнего изменения GroupPolicyObjectFile.</span><span class="sxs-lookup"><span data-stu-id="43df4-147">The date and time at which the GroupPolicyObjectFile was last modified.</span></span>|
|<span data-ttu-id="43df4-148">content</span><span class="sxs-lookup"><span data-stu-id="43df4-148">content</span></span>|<span data-ttu-id="43df4-149">String</span><span class="sxs-lookup"><span data-stu-id="43df4-149">String</span></span>|<span data-ttu-id="43df4-150">Контент объекта групповой политики.</span><span class="sxs-lookup"><span data-stu-id="43df4-150">The Group Policy Object file content.</span></span>|



## <a name="response"></a><span data-ttu-id="43df4-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="43df4-151">Response</span></span>
<span data-ttu-id="43df4-152">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="43df4-152">If successful, this method returns a `201 Created` response code and a [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43df4-153">Пример</span><span class="sxs-lookup"><span data-stu-id="43df4-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="43df4-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="43df4-154">Request</span></span>
<span data-ttu-id="43df4-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43df4-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="43df4-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="43df4-156">Response</span></span>
<span data-ttu-id="43df4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43df4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




