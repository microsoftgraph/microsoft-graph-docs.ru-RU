---
title: Обновление windowsDefenderApplicationControlSupplementalPolicy
description: Обновление свойств объекта WindowsDefenderApplicationControlSupplementalPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c6740654616d112db2d64910b5dd716111a582c0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134027"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicy"></a><span data-ttu-id="9841a-103">Обновление windowsDefenderApplicationControlSupplementalPolicy</span><span class="sxs-lookup"><span data-stu-id="9841a-103">Update windowsDefenderApplicationControlSupplementalPolicy</span></span>

<span data-ttu-id="9841a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9841a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9841a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9841a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9841a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9841a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9841a-107">Обновление свойств объекта [WindowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9841a-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9841a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9841a-108">Prerequisites</span></span>
<span data-ttu-id="9841a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9841a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9841a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9841a-111">Permission type</span></span>|<span data-ttu-id="9841a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9841a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9841a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9841a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9841a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9841a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9841a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9841a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9841a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9841a-116">Not supported.</span></span>|
|<span data-ttu-id="9841a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9841a-117">Application</span></span>|<span data-ttu-id="9841a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9841a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9841a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9841a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}/policy
```

## <a name="request-headers"></a><span data-ttu-id="9841a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9841a-120">Request headers</span></span>
|<span data-ttu-id="9841a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9841a-121">Header</span></span>|<span data-ttu-id="9841a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9841a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9841a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9841a-123">Authorization</span></span>|<span data-ttu-id="9841a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9841a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9841a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9841a-125">Accept</span></span>|<span data-ttu-id="9841a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9841a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9841a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9841a-127">Request body</span></span>
<span data-ttu-id="9841a-128">В теле запроса поставляем представление JSON для [объекта WindowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9841a-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

<span data-ttu-id="9841a-129">В следующей таблице показаны свойства, необходимые при создании [windowsDefenderApplicationControlSupplementalPolicy.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9841a-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md).</span></span>

|<span data-ttu-id="9841a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9841a-130">Property</span></span>|<span data-ttu-id="9841a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9841a-131">Type</span></span>|<span data-ttu-id="9841a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9841a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9841a-133">id</span><span class="sxs-lookup"><span data-stu-id="9841a-133">id</span></span>|<span data-ttu-id="9841a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9841a-134">String</span></span>|<span data-ttu-id="9841a-135">Ключ для дополнительной политики WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="9841a-135">The key for the WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="9841a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9841a-136">displayName</span></span>|<span data-ttu-id="9841a-137">Строка</span><span class="sxs-lookup"><span data-stu-id="9841a-137">String</span></span>|<span data-ttu-id="9841a-138">Отображение имени дополнительной политики WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="9841a-138">The display name of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="9841a-139">description</span><span class="sxs-lookup"><span data-stu-id="9841a-139">description</span></span>|<span data-ttu-id="9841a-140">Строка</span><span class="sxs-lookup"><span data-stu-id="9841a-140">String</span></span>|<span data-ttu-id="9841a-141">Описание дополнительной политики WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="9841a-141">The description of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="9841a-142">содержимое</span><span class="sxs-lookup"><span data-stu-id="9841a-142">content</span></span>|<span data-ttu-id="9841a-143">Binary</span><span class="sxs-lookup"><span data-stu-id="9841a-143">Binary</span></span>|<span data-ttu-id="9841a-144">Контент дополнительной политики WindowsDefenderApplicationControl в формате byte array.</span><span class="sxs-lookup"><span data-stu-id="9841a-144">The WindowsDefenderApplicationControl supplemental policy content in byte array format.</span></span>|
|<span data-ttu-id="9841a-145">contentFileName</span><span class="sxs-lookup"><span data-stu-id="9841a-145">contentFileName</span></span>|<span data-ttu-id="9841a-146">Строка</span><span class="sxs-lookup"><span data-stu-id="9841a-146">String</span></span>|<span data-ttu-id="9841a-147">Имя файла дополнительного контента политики WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="9841a-147">The WindowsDefenderApplicationControl supplemental policy content's file name.</span></span>|
|<span data-ttu-id="9841a-148">version</span><span class="sxs-lookup"><span data-stu-id="9841a-148">version</span></span>|<span data-ttu-id="9841a-149">String</span><span class="sxs-lookup"><span data-stu-id="9841a-149">String</span></span>|<span data-ttu-id="9841a-150">Версия дополнительной политики WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="9841a-150">The WindowsDefenderApplicationControl supplemental policy's version.</span></span>|
|<span data-ttu-id="9841a-151">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="9841a-151">creationDateTime</span></span>|<span data-ttu-id="9841a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9841a-152">DateTimeOffset</span></span>|<span data-ttu-id="9841a-153">Дата и время отправки дополнительной политики WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="9841a-153">The date and time when the WindowsDefenderApplicationControl supplemental policy was uploaded.</span></span>|
|<span data-ttu-id="9841a-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9841a-154">lastModifiedDateTime</span></span>|<span data-ttu-id="9841a-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9841a-155">DateTimeOffset</span></span>|<span data-ttu-id="9841a-156">Дата и время последнего изменения политики дополнительных приложений WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="9841a-156">The date and time when the WindowsDefenderApplicationControl supplemental policy was last modified.</span></span>|
|<span data-ttu-id="9841a-157">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9841a-157">roleScopeTagIds</span></span>|<span data-ttu-id="9841a-158">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9841a-158">String collection</span></span>|<span data-ttu-id="9841a-159">Список тегов области для этого объекта дополнительной политики WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="9841a-159">List of Scope Tags for this WindowsDefenderApplicationControl supplemental policy entity.</span></span>|



## <a name="response"></a><span data-ttu-id="9841a-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="9841a-160">Response</span></span>
<span data-ttu-id="9841a-161">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9841a-161">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9841a-162">Пример</span><span class="sxs-lookup"><span data-stu-id="9841a-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="9841a-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="9841a-163">Request</span></span>
<span data-ttu-id="9841a-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9841a-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="9841a-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="9841a-165">Response</span></span>
<span data-ttu-id="9841a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9841a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 517

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "id": "83d0c39e-c39e-83d0-9ec3-d0839ec3d083",
  "displayName": "Display Name value",
  "description": "Description value",
  "content": "Y29udGVudA==",
  "contentFileName": "Content File Name value",
  "version": "Version value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




