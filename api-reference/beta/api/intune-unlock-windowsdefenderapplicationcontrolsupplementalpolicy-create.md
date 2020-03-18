---
title: Создание Виндовсдефендераппликатионконтролсупплементалполици
description: Создание нового объекта Виндовсдефендераппликатионконтролсупплементалполици.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d207aaced3212111cc40c78576fffe3ceb9d21ad
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800076"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicy"></a><span data-ttu-id="b1cbd-103">Создание Виндовсдефендераппликатионконтролсупплементалполици</span><span class="sxs-lookup"><span data-stu-id="b1cbd-103">Create windowsDefenderApplicationControlSupplementalPolicy</span></span>

> <span data-ttu-id="b1cbd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1cbd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1cbd-106">Создание нового объекта [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="b1cbd-106">Create a new [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1cbd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b1cbd-107">Prerequisites</span></span>
<span data-ttu-id="b1cbd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1cbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1cbd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1cbd-110">Permission type</span></span>|<span data-ttu-id="b1cbd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1cbd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1cbd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1cbd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1cbd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1cbd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b1cbd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1cbd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1cbd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-115">Not supported.</span></span>|
|<span data-ttu-id="b1cbd-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b1cbd-116">Application</span></span>|<span data-ttu-id="b1cbd-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1cbd-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1cbd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1cbd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies
```

## <a name="request-headers"></a><span data-ttu-id="b1cbd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b1cbd-119">Request headers</span></span>
|<span data-ttu-id="b1cbd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1cbd-120">Header</span></span>|<span data-ttu-id="b1cbd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b1cbd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1cbd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1cbd-122">Authorization</span></span>|<span data-ttu-id="b1cbd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1cbd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b1cbd-124">Accept</span></span>|<span data-ttu-id="b1cbd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b1cbd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1cbd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1cbd-126">Request body</span></span>
<span data-ttu-id="b1cbd-127">В тексте запроса добавьте представление объекта Виндовсдефендераппликатионконтролсупплементалполици в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-127">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicy object.</span></span>

<span data-ttu-id="b1cbd-128">В следующей таблице приведены свойства, необходимые при создании Виндовсдефендераппликатионконтролсупплементалполици.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-128">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicy.</span></span>

|<span data-ttu-id="b1cbd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1cbd-129">Property</span></span>|<span data-ttu-id="b1cbd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b1cbd-130">Type</span></span>|<span data-ttu-id="b1cbd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b1cbd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1cbd-132">id</span><span class="sxs-lookup"><span data-stu-id="b1cbd-132">id</span></span>|<span data-ttu-id="b1cbd-133">String</span><span class="sxs-lookup"><span data-stu-id="b1cbd-133">String</span></span>|<span data-ttu-id="b1cbd-134">Ключ для дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-134">The key for the WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="b1cbd-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b1cbd-135">displayName</span></span>|<span data-ttu-id="b1cbd-136">Строка</span><span class="sxs-lookup"><span data-stu-id="b1cbd-136">String</span></span>|<span data-ttu-id="b1cbd-137">Отображаемое имя дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-137">The display name of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="b1cbd-138">description</span><span class="sxs-lookup"><span data-stu-id="b1cbd-138">description</span></span>|<span data-ttu-id="b1cbd-139">String</span><span class="sxs-lookup"><span data-stu-id="b1cbd-139">String</span></span>|<span data-ttu-id="b1cbd-140">Описание дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-140">The description of WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="b1cbd-141">содержимое</span><span class="sxs-lookup"><span data-stu-id="b1cbd-141">content</span></span>|<span data-ttu-id="b1cbd-142">Binary</span><span class="sxs-lookup"><span data-stu-id="b1cbd-142">Binary</span></span>|<span data-ttu-id="b1cbd-143">Содержимое дополнительной политики Виндовсдефендераппликатионконтрол в формате массива байтов.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-143">The WindowsDefenderApplicationControl supplemental policy content in byte array format.</span></span>|
|<span data-ttu-id="b1cbd-144">контентфиленаме</span><span class="sxs-lookup"><span data-stu-id="b1cbd-144">contentFileName</span></span>|<span data-ttu-id="b1cbd-145">String</span><span class="sxs-lookup"><span data-stu-id="b1cbd-145">String</span></span>|<span data-ttu-id="b1cbd-146">Имя файла дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-146">The WindowsDefenderApplicationControl supplemental policy content's file name.</span></span>|
|<span data-ttu-id="b1cbd-147">version</span><span class="sxs-lookup"><span data-stu-id="b1cbd-147">version</span></span>|<span data-ttu-id="b1cbd-148">String</span><span class="sxs-lookup"><span data-stu-id="b1cbd-148">String</span></span>|<span data-ttu-id="b1cbd-149">Версия дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-149">The WindowsDefenderApplicationControl supplemental policy's version.</span></span>|
|<span data-ttu-id="b1cbd-150">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="b1cbd-150">creationDateTime</span></span>|<span data-ttu-id="b1cbd-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1cbd-151">DateTimeOffset</span></span>|<span data-ttu-id="b1cbd-152">Дата и время отправки дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-152">The date and time when the WindowsDefenderApplicationControl supplemental policy was uploaded.</span></span>|
|<span data-ttu-id="b1cbd-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1cbd-153">lastModifiedDateTime</span></span>|<span data-ttu-id="b1cbd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1cbd-154">DateTimeOffset</span></span>|<span data-ttu-id="b1cbd-155">Дата и время последнего изменения дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-155">The date and time when the WindowsDefenderApplicationControl supplemental policy was last modified.</span></span>|
|<span data-ttu-id="b1cbd-156">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b1cbd-156">roleScopeTagIds</span></span>|<span data-ttu-id="b1cbd-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b1cbd-157">String collection</span></span>|<span data-ttu-id="b1cbd-158">Список тегов областей для данной дополнительной политики Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-158">List of Scope Tags for this WindowsDefenderApplicationControl supplemental policy entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b1cbd-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1cbd-159">Response</span></span>
<span data-ttu-id="b1cbd-160">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсдефендераппликатионконтролсупплементалполици](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-160">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1cbd-161">Пример</span><span class="sxs-lookup"><span data-stu-id="b1cbd-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1cbd-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1cbd-162">Request</span></span>
<span data-ttu-id="b1cbd-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies
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

### <a name="response"></a><span data-ttu-id="b1cbd-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1cbd-164">Response</span></span>
<span data-ttu-id="b1cbd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1cbd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




