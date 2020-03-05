---
title: Обновление Унсуппортедграупполициекстенсион
description: Обновление свойств объекта Унсуппортедграупполициекстенсион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dd6843a1d899a2e65b95ada5eb6ee29f07f2f40d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465312"
---
# <a name="update-unsupportedgrouppolicyextension"></a><span data-ttu-id="72d42-103">Обновление Унсуппортедграупполициекстенсион</span><span class="sxs-lookup"><span data-stu-id="72d42-103">Update unsupportedGroupPolicyExtension</span></span>

<span data-ttu-id="72d42-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="72d42-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72d42-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72d42-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72d42-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72d42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72d42-107">Обновление свойств объекта [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .</span><span class="sxs-lookup"><span data-stu-id="72d42-107">Update the properties of a [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72d42-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="72d42-108">Prerequisites</span></span>
<span data-ttu-id="72d42-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72d42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72d42-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72d42-111">Permission type</span></span>|<span data-ttu-id="72d42-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="72d42-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72d42-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72d42-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72d42-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72d42-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72d42-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72d42-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72d42-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72d42-116">Not supported.</span></span>|
|<span data-ttu-id="72d42-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72d42-117">Application</span></span>|<span data-ttu-id="72d42-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72d42-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72d42-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72d42-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions/{unsupportedGroupPolicyExtensionId}
```

## <a name="request-headers"></a><span data-ttu-id="72d42-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="72d42-120">Request headers</span></span>
|<span data-ttu-id="72d42-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72d42-121">Header</span></span>|<span data-ttu-id="72d42-122">Значение</span><span class="sxs-lookup"><span data-stu-id="72d42-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72d42-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="72d42-123">Authorization</span></span>|<span data-ttu-id="72d42-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72d42-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72d42-125">Accept</span><span class="sxs-lookup"><span data-stu-id="72d42-125">Accept</span></span>|<span data-ttu-id="72d42-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72d42-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72d42-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72d42-127">Request body</span></span>
<span data-ttu-id="72d42-128">В тексте запроса добавьте представление объекта [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72d42-128">In the request body, supply a JSON representation for the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

<span data-ttu-id="72d42-129">В следующей таблице приведены свойства, необходимые при создании [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md).</span><span class="sxs-lookup"><span data-stu-id="72d42-129">The following table shows the properties that are required when you create the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md).</span></span>

|<span data-ttu-id="72d42-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="72d42-130">Property</span></span>|<span data-ttu-id="72d42-131">Тип</span><span class="sxs-lookup"><span data-stu-id="72d42-131">Type</span></span>|<span data-ttu-id="72d42-132">Описание</span><span class="sxs-lookup"><span data-stu-id="72d42-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72d42-133">id</span><span class="sxs-lookup"><span data-stu-id="72d42-133">id</span></span>|<span data-ttu-id="72d42-134">String</span><span class="sxs-lookup"><span data-stu-id="72d42-134">String</span></span>|<span data-ttu-id="72d42-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="72d42-135">Not yet documented</span></span>|
|<span data-ttu-id="72d42-136">сеттингскопе</span><span class="sxs-lookup"><span data-stu-id="72d42-136">settingScope</span></span>|[<span data-ttu-id="72d42-137">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="72d42-137">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="72d42-138">Задание области для неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="72d42-138">Setting Scope of the unsupported extension.</span></span> <span data-ttu-id="72d42-139">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="72d42-139">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="72d42-140">намеспацеурл</span><span class="sxs-lookup"><span data-stu-id="72d42-140">namespaceUrl</span></span>|<span data-ttu-id="72d42-141">String</span><span class="sxs-lookup"><span data-stu-id="72d42-141">String</span></span>|<span data-ttu-id="72d42-142">URL-адрес пространства имен неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="72d42-142">Namespace Url of the unsupported extension.</span></span>|
|<span data-ttu-id="72d42-143">екстенсионтипе</span><span class="sxs-lookup"><span data-stu-id="72d42-143">extensionType</span></span>|<span data-ttu-id="72d42-144">String</span><span class="sxs-lookup"><span data-stu-id="72d42-144">String</span></span>|<span data-ttu-id="72d42-145">Екстенсионтипе неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="72d42-145">ExtensionType of the unsupported extension.</span></span>|
|<span data-ttu-id="72d42-146">nodeName</span><span class="sxs-lookup"><span data-stu-id="72d42-146">nodeName</span></span>|<span data-ttu-id="72d42-147">String</span><span class="sxs-lookup"><span data-stu-id="72d42-147">String</span></span>|<span data-ttu-id="72d42-148">Имя узла неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="72d42-148">Node name of the unsupported extension.</span></span>|



## <a name="response"></a><span data-ttu-id="72d42-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="72d42-149">Response</span></span>
<span data-ttu-id="72d42-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72d42-150">If successful, this method returns a `200 OK` response code and an updated [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72d42-151">Пример</span><span class="sxs-lookup"><span data-stu-id="72d42-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="72d42-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="72d42-152">Request</span></span>
<span data-ttu-id="72d42-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72d42-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="72d42-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="72d42-154">Response</span></span>
<span data-ttu-id="72d42-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72d42-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





