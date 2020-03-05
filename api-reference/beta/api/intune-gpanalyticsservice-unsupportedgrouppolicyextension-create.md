---
title: Создание Унсуппортедграупполициекстенсион
description: Создание нового объекта Унсуппортедграупполициекстенсион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 550e0b2f34c658e1cc3f49f9f2d75cedd031fffd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465410"
---
# <a name="create-unsupportedgrouppolicyextension"></a><span data-ttu-id="57d8a-103">Создание Унсуппортедграупполициекстенсион</span><span class="sxs-lookup"><span data-stu-id="57d8a-103">Create unsupportedGroupPolicyExtension</span></span>

<span data-ttu-id="57d8a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="57d8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57d8a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57d8a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57d8a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57d8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57d8a-107">Создание нового объекта [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .</span><span class="sxs-lookup"><span data-stu-id="57d8a-107">Create a new [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57d8a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="57d8a-108">Prerequisites</span></span>
<span data-ttu-id="57d8a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57d8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57d8a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57d8a-111">Permission type</span></span>|<span data-ttu-id="57d8a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="57d8a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57d8a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57d8a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57d8a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57d8a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57d8a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57d8a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57d8a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57d8a-116">Not supported.</span></span>|
|<span data-ttu-id="57d8a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57d8a-117">Application</span></span>|<span data-ttu-id="57d8a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57d8a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57d8a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57d8a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
```

## <a name="request-headers"></a><span data-ttu-id="57d8a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="57d8a-120">Request headers</span></span>
|<span data-ttu-id="57d8a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57d8a-121">Header</span></span>|<span data-ttu-id="57d8a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="57d8a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57d8a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="57d8a-123">Authorization</span></span>|<span data-ttu-id="57d8a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57d8a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57d8a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="57d8a-125">Accept</span></span>|<span data-ttu-id="57d8a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57d8a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57d8a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57d8a-127">Request body</span></span>
<span data-ttu-id="57d8a-128">В тексте запроса добавьте представление объекта Унсуппортедграупполициекстенсион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57d8a-128">In the request body, supply a JSON representation for the unsupportedGroupPolicyExtension object.</span></span>

<span data-ttu-id="57d8a-129">В следующей таблице приведены свойства, необходимые при создании Унсуппортедграупполициекстенсион.</span><span class="sxs-lookup"><span data-stu-id="57d8a-129">The following table shows the properties that are required when you create the unsupportedGroupPolicyExtension.</span></span>

|<span data-ttu-id="57d8a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="57d8a-130">Property</span></span>|<span data-ttu-id="57d8a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="57d8a-131">Type</span></span>|<span data-ttu-id="57d8a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="57d8a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57d8a-133">id</span><span class="sxs-lookup"><span data-stu-id="57d8a-133">id</span></span>|<span data-ttu-id="57d8a-134">String</span><span class="sxs-lookup"><span data-stu-id="57d8a-134">String</span></span>|<span data-ttu-id="57d8a-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="57d8a-135">Not yet documented</span></span>|
|<span data-ttu-id="57d8a-136">сеттингскопе</span><span class="sxs-lookup"><span data-stu-id="57d8a-136">settingScope</span></span>|[<span data-ttu-id="57d8a-137">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="57d8a-137">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="57d8a-138">Задание области для неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="57d8a-138">Setting Scope of the unsupported extension.</span></span> <span data-ttu-id="57d8a-139">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="57d8a-139">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="57d8a-140">намеспацеурл</span><span class="sxs-lookup"><span data-stu-id="57d8a-140">namespaceUrl</span></span>|<span data-ttu-id="57d8a-141">String</span><span class="sxs-lookup"><span data-stu-id="57d8a-141">String</span></span>|<span data-ttu-id="57d8a-142">URL-адрес пространства имен неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="57d8a-142">Namespace Url of the unsupported extension.</span></span>|
|<span data-ttu-id="57d8a-143">екстенсионтипе</span><span class="sxs-lookup"><span data-stu-id="57d8a-143">extensionType</span></span>|<span data-ttu-id="57d8a-144">String</span><span class="sxs-lookup"><span data-stu-id="57d8a-144">String</span></span>|<span data-ttu-id="57d8a-145">Екстенсионтипе неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="57d8a-145">ExtensionType of the unsupported extension.</span></span>|
|<span data-ttu-id="57d8a-146">nodeName</span><span class="sxs-lookup"><span data-stu-id="57d8a-146">nodeName</span></span>|<span data-ttu-id="57d8a-147">String</span><span class="sxs-lookup"><span data-stu-id="57d8a-147">String</span></span>|<span data-ttu-id="57d8a-148">Имя узла неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="57d8a-148">Node name of the unsupported extension.</span></span>|



## <a name="response"></a><span data-ttu-id="57d8a-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="57d8a-149">Response</span></span>
<span data-ttu-id="57d8a-150">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57d8a-150">If successful, this method returns a `201 Created` response code and a [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57d8a-151">Пример</span><span class="sxs-lookup"><span data-stu-id="57d8a-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="57d8a-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="57d8a-152">Request</span></span>
<span data-ttu-id="57d8a-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57d8a-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
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

### <a name="response"></a><span data-ttu-id="57d8a-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="57d8a-154">Response</span></span>
<span data-ttu-id="57d8a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57d8a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





