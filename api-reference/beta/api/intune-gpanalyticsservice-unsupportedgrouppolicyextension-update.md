---
title: Обновление Унсуппортедграупполициекстенсион
description: Обновление свойств объекта Унсуппортедграупполициекстенсион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b4e7d5656d78178a445d98c789d70246919ee07
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804543"
---
# <a name="update-unsupportedgrouppolicyextension"></a><span data-ttu-id="08cef-103">Обновление Унсуппортедграупполициекстенсион</span><span class="sxs-lookup"><span data-stu-id="08cef-103">Update unsupportedGroupPolicyExtension</span></span>

> <span data-ttu-id="08cef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08cef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08cef-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08cef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08cef-106">Обновление свойств объекта [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .</span><span class="sxs-lookup"><span data-stu-id="08cef-106">Update the properties of a [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08cef-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="08cef-107">Prerequisites</span></span>
<span data-ttu-id="08cef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08cef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08cef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08cef-110">Permission type</span></span>|<span data-ttu-id="08cef-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="08cef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08cef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08cef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08cef-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08cef-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08cef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08cef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08cef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08cef-115">Not supported.</span></span>|
|<span data-ttu-id="08cef-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="08cef-116">Application</span></span>|<span data-ttu-id="08cef-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08cef-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08cef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08cef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions/{unsupportedGroupPolicyExtensionId}
```

## <a name="request-headers"></a><span data-ttu-id="08cef-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="08cef-119">Request headers</span></span>
|<span data-ttu-id="08cef-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08cef-120">Header</span></span>|<span data-ttu-id="08cef-121">Значение</span><span class="sxs-lookup"><span data-stu-id="08cef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08cef-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08cef-122">Authorization</span></span>|<span data-ttu-id="08cef-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08cef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08cef-124">Accept</span><span class="sxs-lookup"><span data-stu-id="08cef-124">Accept</span></span>|<span data-ttu-id="08cef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08cef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08cef-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08cef-126">Request body</span></span>
<span data-ttu-id="08cef-127">В тексте запроса добавьте представление объекта [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08cef-127">In the request body, supply a JSON representation for the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

<span data-ttu-id="08cef-128">В следующей таблице приведены свойства, необходимые при создании [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md).</span><span class="sxs-lookup"><span data-stu-id="08cef-128">The following table shows the properties that are required when you create the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md).</span></span>

|<span data-ttu-id="08cef-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="08cef-129">Property</span></span>|<span data-ttu-id="08cef-130">Тип</span><span class="sxs-lookup"><span data-stu-id="08cef-130">Type</span></span>|<span data-ttu-id="08cef-131">Описание</span><span class="sxs-lookup"><span data-stu-id="08cef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08cef-132">id</span><span class="sxs-lookup"><span data-stu-id="08cef-132">id</span></span>|<span data-ttu-id="08cef-133">String</span><span class="sxs-lookup"><span data-stu-id="08cef-133">String</span></span>|<span data-ttu-id="08cef-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="08cef-134">Not yet documented</span></span>|
|<span data-ttu-id="08cef-135">сеттингскопе</span><span class="sxs-lookup"><span data-stu-id="08cef-135">settingScope</span></span>|[<span data-ttu-id="08cef-136">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="08cef-136">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="08cef-137">Задание области для неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="08cef-137">Setting Scope of the unsupported extension.</span></span> <span data-ttu-id="08cef-138">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="08cef-138">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="08cef-139">намеспацеурл</span><span class="sxs-lookup"><span data-stu-id="08cef-139">namespaceUrl</span></span>|<span data-ttu-id="08cef-140">String</span><span class="sxs-lookup"><span data-stu-id="08cef-140">String</span></span>|<span data-ttu-id="08cef-141">URL-адрес пространства имен неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="08cef-141">Namespace Url of the unsupported extension.</span></span>|
|<span data-ttu-id="08cef-142">екстенсионтипе</span><span class="sxs-lookup"><span data-stu-id="08cef-142">extensionType</span></span>|<span data-ttu-id="08cef-143">String</span><span class="sxs-lookup"><span data-stu-id="08cef-143">String</span></span>|<span data-ttu-id="08cef-144">Екстенсионтипе неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="08cef-144">ExtensionType of the unsupported extension.</span></span>|
|<span data-ttu-id="08cef-145">nodeName</span><span class="sxs-lookup"><span data-stu-id="08cef-145">nodeName</span></span>|<span data-ttu-id="08cef-146">String</span><span class="sxs-lookup"><span data-stu-id="08cef-146">String</span></span>|<span data-ttu-id="08cef-147">Имя узла неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="08cef-147">Node name of the unsupported extension.</span></span>|



## <a name="response"></a><span data-ttu-id="08cef-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="08cef-148">Response</span></span>
<span data-ttu-id="08cef-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08cef-149">If successful, this method returns a `200 OK` response code and an updated [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08cef-150">Пример</span><span class="sxs-lookup"><span data-stu-id="08cef-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="08cef-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="08cef-151">Request</span></span>
<span data-ttu-id="08cef-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08cef-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions/{unsupportedGroupPolicyExtensionId}
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
  "settingScope": "device",
  "namespaceUrl": "https://example.com/namespaceUrl/",
  "extensionType": "Extension Type value",
  "nodeName": "Node Name value"
}
```

### <a name="response"></a><span data-ttu-id="08cef-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="08cef-153">Response</span></span>
<span data-ttu-id="08cef-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08cef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
  "id": "e59ecce2-cce2-e59e-e2cc-9ee5e2cc9ee5",
  "settingScope": "device",
  "namespaceUrl": "https://example.com/namespaceUrl/",
  "extensionType": "Extension Type value",
  "nodeName": "Node Name value"
}
```




