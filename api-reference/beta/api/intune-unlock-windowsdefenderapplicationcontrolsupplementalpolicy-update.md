---
title: Обновление Виндовсдефендераппликатионконтролсупплементалполици
description: Обновление свойств объекта Виндовсдефендераппликатионконтролсупплементалполици.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d44f7e1cfb97068130bc282d40bd222fbc616e6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095865"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicy"></a><span data-ttu-id="10c80-103">Обновление Виндовсдефендераппликатионконтролсупплементалполици</span><span class="sxs-lookup"><span data-stu-id="10c80-103">Update windowsDefenderApplicationControlSupplementalPolicy</span></span>

<span data-ttu-id="10c80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10c80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10c80-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10c80-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10c80-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10c80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10c80-107">Обновление свойств объекта [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="10c80-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10c80-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="10c80-108">Prerequisites</span></span>
<span data-ttu-id="10c80-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10c80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10c80-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10c80-111">Permission type</span></span>|<span data-ttu-id="10c80-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10c80-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10c80-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10c80-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10c80-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10c80-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="10c80-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10c80-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10c80-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10c80-116">Not supported.</span></span>|
|<span data-ttu-id="10c80-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10c80-117">Application</span></span>|<span data-ttu-id="10c80-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10c80-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10c80-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10c80-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}/policy
```

## <a name="request-headers"></a><span data-ttu-id="10c80-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="10c80-120">Request headers</span></span>
|<span data-ttu-id="10c80-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10c80-121">Header</span></span>|<span data-ttu-id="10c80-122">Значение</span><span class="sxs-lookup"><span data-stu-id="10c80-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10c80-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10c80-123">Authorization</span></span>|<span data-ttu-id="10c80-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10c80-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10c80-125">Accept</span><span class="sxs-lookup"><span data-stu-id="10c80-125">Accept</span></span>|<span data-ttu-id="10c80-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10c80-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10c80-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10c80-127">Request body</span></span>
<span data-ttu-id="10c80-128">В тексте запроса добавьте представление объекта [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10c80-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

<span data-ttu-id="10c80-129">В следующей таблице приведены свойства, необходимые при создании [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="10c80-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md).</span></span>

|<span data-ttu-id="10c80-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="10c80-130">Property</span></span>|<span data-ttu-id="10c80-131">Тип</span><span class="sxs-lookup"><span data-stu-id="10c80-131">Type</span></span>|<span data-ttu-id="10c80-132">Описание</span><span class="sxs-lookup"><span data-stu-id="10c80-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10c80-133">id</span><span class="sxs-lookup"><span data-stu-id="10c80-133">id</span></span>|<span data-ttu-id="10c80-134">Строка</span><span class="sxs-lookup"><span data-stu-id="10c80-134">String</span></span>|<span data-ttu-id="10c80-135">Ключ для дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="10c80-135">The key for the WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="10c80-136">displayName</span><span class="sxs-lookup"><span data-stu-id="10c80-136">displayName</span></span>|<span data-ttu-id="10c80-137">Строка</span><span class="sxs-lookup"><span data-stu-id="10c80-137">String</span></span>|<span data-ttu-id="10c80-138">Отображаемое имя дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="10c80-138">The display name of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="10c80-139">description</span><span class="sxs-lookup"><span data-stu-id="10c80-139">description</span></span>|<span data-ttu-id="10c80-140">Строка</span><span class="sxs-lookup"><span data-stu-id="10c80-140">String</span></span>|<span data-ttu-id="10c80-141">Описание дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="10c80-141">The description of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="10c80-142">содержимое</span><span class="sxs-lookup"><span data-stu-id="10c80-142">content</span></span>|<span data-ttu-id="10c80-143">Binary</span><span class="sxs-lookup"><span data-stu-id="10c80-143">Binary</span></span>|<span data-ttu-id="10c80-144">Содержимое дополнительной политики Виндовсдефендераппликатионконтрол в формате массива байтов.</span><span class="sxs-lookup"><span data-stu-id="10c80-144">The WindowsDefenderApplicationControl supplemental policy content in byte array format.</span></span>|
|<span data-ttu-id="10c80-145">контентфиленаме</span><span class="sxs-lookup"><span data-stu-id="10c80-145">contentFileName</span></span>|<span data-ttu-id="10c80-146">Строка</span><span class="sxs-lookup"><span data-stu-id="10c80-146">String</span></span>|<span data-ttu-id="10c80-147">Имя файла дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="10c80-147">The WindowsDefenderApplicationControl supplemental policy content's file name.</span></span>|
|<span data-ttu-id="10c80-148">version</span><span class="sxs-lookup"><span data-stu-id="10c80-148">version</span></span>|<span data-ttu-id="10c80-149">String</span><span class="sxs-lookup"><span data-stu-id="10c80-149">String</span></span>|<span data-ttu-id="10c80-150">Версия дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="10c80-150">The WindowsDefenderApplicationControl supplemental policy's version.</span></span>|
|<span data-ttu-id="10c80-151">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="10c80-151">creationDateTime</span></span>|<span data-ttu-id="10c80-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10c80-152">DateTimeOffset</span></span>|<span data-ttu-id="10c80-153">Дата и время отправки дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="10c80-153">The date and time when the WindowsDefenderApplicationControl supplemental policy was uploaded.</span></span>|
|<span data-ttu-id="10c80-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10c80-154">lastModifiedDateTime</span></span>|<span data-ttu-id="10c80-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10c80-155">DateTimeOffset</span></span>|<span data-ttu-id="10c80-156">Дата и время последнего изменения дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="10c80-156">The date and time when the WindowsDefenderApplicationControl supplemental policy was last modified.</span></span>|
|<span data-ttu-id="10c80-157">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="10c80-157">roleScopeTagIds</span></span>|<span data-ttu-id="10c80-158">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="10c80-158">String collection</span></span>|<span data-ttu-id="10c80-159">Список тегов областей для данной дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="10c80-159">List of Scope Tags for this WindowsDefenderApplicationControl supplemental policy entity.</span></span>|



## <a name="response"></a><span data-ttu-id="10c80-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="10c80-160">Response</span></span>
<span data-ttu-id="10c80-161">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10c80-161">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10c80-162">Пример</span><span class="sxs-lookup"><span data-stu-id="10c80-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="10c80-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="10c80-163">Request</span></span>
<span data-ttu-id="10c80-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10c80-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="10c80-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="10c80-165">Response</span></span>
<span data-ttu-id="10c80-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10c80-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






