---
title: Обновление Виндовсдефендераппликатионконтролсупплементалполици
description: Обновление свойств объекта Виндовсдефендераппликатионконтролсупплементалполици.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6bcffdbcd4b1e18cd97262850ba3fc44c5e955c5
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536688"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicy"></a><span data-ttu-id="bef7c-103">Обновление Виндовсдефендераппликатионконтролсупплементалполици</span><span class="sxs-lookup"><span data-stu-id="bef7c-103">Update windowsDefenderApplicationControlSupplementalPolicy</span></span>

> <span data-ttu-id="bef7c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bef7c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bef7c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bef7c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bef7c-106">Обновление свойств объекта [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="bef7c-106">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bef7c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bef7c-107">Prerequisites</span></span>
<span data-ttu-id="bef7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bef7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bef7c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bef7c-110">Permission type</span></span>|<span data-ttu-id="bef7c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bef7c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bef7c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bef7c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bef7c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bef7c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bef7c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bef7c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bef7c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bef7c-115">Not supported.</span></span>|
|<span data-ttu-id="bef7c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="bef7c-116">Application</span></span>|<span data-ttu-id="bef7c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bef7c-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bef7c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bef7c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}/policy
```

## <a name="request-headers"></a><span data-ttu-id="bef7c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bef7c-119">Request headers</span></span>
|<span data-ttu-id="bef7c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bef7c-120">Header</span></span>|<span data-ttu-id="bef7c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bef7c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bef7c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bef7c-122">Authorization</span></span>|<span data-ttu-id="bef7c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bef7c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bef7c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bef7c-124">Accept</span></span>|<span data-ttu-id="bef7c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bef7c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bef7c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bef7c-126">Request body</span></span>
<span data-ttu-id="bef7c-127">В тексте запроса добавьте представление объекта [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bef7c-127">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

<span data-ttu-id="bef7c-128">В следующей таблице приведены свойства, необходимые при создании [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bef7c-128">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md).</span></span>

|<span data-ttu-id="bef7c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bef7c-129">Property</span></span>|<span data-ttu-id="bef7c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bef7c-130">Type</span></span>|<span data-ttu-id="bef7c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bef7c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bef7c-132">id</span><span class="sxs-lookup"><span data-stu-id="bef7c-132">id</span></span>|<span data-ttu-id="bef7c-133">String</span><span class="sxs-lookup"><span data-stu-id="bef7c-133">String</span></span>|<span data-ttu-id="bef7c-134">Ключ для дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="bef7c-134">The key for the WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="bef7c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="bef7c-135">displayName</span></span>|<span data-ttu-id="bef7c-136">Строка</span><span class="sxs-lookup"><span data-stu-id="bef7c-136">String</span></span>|<span data-ttu-id="bef7c-137">Отображаемое имя дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="bef7c-137">The display name of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="bef7c-138">description</span><span class="sxs-lookup"><span data-stu-id="bef7c-138">description</span></span>|<span data-ttu-id="bef7c-139">String</span><span class="sxs-lookup"><span data-stu-id="bef7c-139">String</span></span>|<span data-ttu-id="bef7c-140">Описание дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="bef7c-140">The description of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="bef7c-141">содержимое</span><span class="sxs-lookup"><span data-stu-id="bef7c-141">content</span></span>|<span data-ttu-id="bef7c-142">Binary</span><span class="sxs-lookup"><span data-stu-id="bef7c-142">Binary</span></span>|<span data-ttu-id="bef7c-143">Содержимое дополнительной политики Виндовсдефендераппликатионконтрол в формате массива байтов.</span><span class="sxs-lookup"><span data-stu-id="bef7c-143">The WindowsDefenderApplicationControl supplemental policy content in byte array format.</span></span>|
|<span data-ttu-id="bef7c-144">контентфиленаме</span><span class="sxs-lookup"><span data-stu-id="bef7c-144">contentFileName</span></span>|<span data-ttu-id="bef7c-145">String</span><span class="sxs-lookup"><span data-stu-id="bef7c-145">String</span></span>|<span data-ttu-id="bef7c-146">Имя файла дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="bef7c-146">The WindowsDefenderApplicationControl supplemental policy content's file name.</span></span>|
|<span data-ttu-id="bef7c-147">version</span><span class="sxs-lookup"><span data-stu-id="bef7c-147">version</span></span>|<span data-ttu-id="bef7c-148">String</span><span class="sxs-lookup"><span data-stu-id="bef7c-148">String</span></span>|<span data-ttu-id="bef7c-149">Версия дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="bef7c-149">The WindowsDefenderApplicationControl supplemental policy's version.</span></span>|
|<span data-ttu-id="bef7c-150">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="bef7c-150">creationDateTime</span></span>|<span data-ttu-id="bef7c-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bef7c-151">DateTimeOffset</span></span>|<span data-ttu-id="bef7c-152">Дата и время отправки дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="bef7c-152">The date and time when the WindowsDefenderApplicationControl supplemental policy was uploaded.</span></span>|
|<span data-ttu-id="bef7c-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bef7c-153">lastModifiedDateTime</span></span>|<span data-ttu-id="bef7c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bef7c-154">DateTimeOffset</span></span>|<span data-ttu-id="bef7c-155">Дата и время последнего изменения дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="bef7c-155">The date and time when the WindowsDefenderApplicationControl supplemental policy was last modified.</span></span>|
|<span data-ttu-id="bef7c-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bef7c-156">roleScopeTagIds</span></span>|<span data-ttu-id="bef7c-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bef7c-157">String collection</span></span>|<span data-ttu-id="bef7c-158">Список тегов областей для данной дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="bef7c-158">List of Scope Tags for this WindowsDefenderApplicationControl supplemental policy entity.</span></span>|



## <a name="response"></a><span data-ttu-id="bef7c-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="bef7c-159">Response</span></span>
<span data-ttu-id="bef7c-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bef7c-160">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bef7c-161">Пример</span><span class="sxs-lookup"><span data-stu-id="bef7c-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="bef7c-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="bef7c-162">Request</span></span>
<span data-ttu-id="bef7c-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bef7c-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bef7c-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="bef7c-164">Response</span></span>
<span data-ttu-id="bef7c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bef7c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






