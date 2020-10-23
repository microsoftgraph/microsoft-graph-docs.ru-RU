---
title: Создание Унсуппортедграупполициекстенсион
description: Создание нового объекта Унсуппортедграупполициекстенсион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 066adda1d6d6b66eb42984ab22c20f155b1f5ea7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696554"
---
# <a name="create-unsupportedgrouppolicyextension"></a><span data-ttu-id="bf41c-103">Создание Унсуппортедграупполициекстенсион</span><span class="sxs-lookup"><span data-stu-id="bf41c-103">Create unsupportedGroupPolicyExtension</span></span>

<span data-ttu-id="bf41c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf41c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf41c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf41c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf41c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf41c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf41c-107">Создание нового объекта [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .</span><span class="sxs-lookup"><span data-stu-id="bf41c-107">Create a new [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf41c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bf41c-108">Prerequisites</span></span>
<span data-ttu-id="bf41c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf41c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf41c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf41c-111">Permission type</span></span>|<span data-ttu-id="bf41c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf41c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf41c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf41c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf41c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf41c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bf41c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf41c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf41c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf41c-116">Not supported.</span></span>|
|<span data-ttu-id="bf41c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf41c-117">Application</span></span>|<span data-ttu-id="bf41c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf41c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf41c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf41c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
```

## <a name="request-headers"></a><span data-ttu-id="bf41c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bf41c-120">Request headers</span></span>
|<span data-ttu-id="bf41c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf41c-121">Header</span></span>|<span data-ttu-id="bf41c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bf41c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf41c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf41c-123">Authorization</span></span>|<span data-ttu-id="bf41c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf41c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf41c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bf41c-125">Accept</span></span>|<span data-ttu-id="bf41c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bf41c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf41c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bf41c-127">Request body</span></span>
<span data-ttu-id="bf41c-128">В тексте запроса добавьте представление объекта Унсуппортедграупполициекстенсион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf41c-128">In the request body, supply a JSON representation for the unsupportedGroupPolicyExtension object.</span></span>

<span data-ttu-id="bf41c-129">В следующей таблице приведены свойства, необходимые при создании Унсуппортедграупполициекстенсион.</span><span class="sxs-lookup"><span data-stu-id="bf41c-129">The following table shows the properties that are required when you create the unsupportedGroupPolicyExtension.</span></span>

|<span data-ttu-id="bf41c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf41c-130">Property</span></span>|<span data-ttu-id="bf41c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bf41c-131">Type</span></span>|<span data-ttu-id="bf41c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bf41c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf41c-133">id</span><span class="sxs-lookup"><span data-stu-id="bf41c-133">id</span></span>|<span data-ttu-id="bf41c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="bf41c-134">String</span></span>|<span data-ttu-id="bf41c-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="bf41c-135">Not yet documented</span></span>|
|<span data-ttu-id="bf41c-136">сеттингскопе</span><span class="sxs-lookup"><span data-stu-id="bf41c-136">settingScope</span></span>|[<span data-ttu-id="bf41c-137">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="bf41c-137">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="bf41c-138">Задание области для неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="bf41c-138">Setting Scope of the unsupported extension.</span></span> <span data-ttu-id="bf41c-139">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="bf41c-139">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="bf41c-140">намеспацеурл</span><span class="sxs-lookup"><span data-stu-id="bf41c-140">namespaceUrl</span></span>|<span data-ttu-id="bf41c-141">Строка</span><span class="sxs-lookup"><span data-stu-id="bf41c-141">String</span></span>|<span data-ttu-id="bf41c-142">URL-адрес пространства имен неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="bf41c-142">Namespace Url of the unsupported extension.</span></span>|
|<span data-ttu-id="bf41c-143">екстенсионтипе</span><span class="sxs-lookup"><span data-stu-id="bf41c-143">extensionType</span></span>|<span data-ttu-id="bf41c-144">Строка</span><span class="sxs-lookup"><span data-stu-id="bf41c-144">String</span></span>|<span data-ttu-id="bf41c-145">Екстенсионтипе неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="bf41c-145">ExtensionType of the unsupported extension.</span></span>|
|<span data-ttu-id="bf41c-146">nodeName</span><span class="sxs-lookup"><span data-stu-id="bf41c-146">nodeName</span></span>|<span data-ttu-id="bf41c-147">Строка</span><span class="sxs-lookup"><span data-stu-id="bf41c-147">String</span></span>|<span data-ttu-id="bf41c-148">Имя узла неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="bf41c-148">Node name of the unsupported extension.</span></span>|



## <a name="response"></a><span data-ttu-id="bf41c-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf41c-149">Response</span></span>
<span data-ttu-id="bf41c-150">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bf41c-150">If successful, this method returns a `201 Created` response code and a [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf41c-151">Пример</span><span class="sxs-lookup"><span data-stu-id="bf41c-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf41c-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf41c-152">Request</span></span>
<span data-ttu-id="bf41c-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf41c-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bf41c-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf41c-154">Response</span></span>
<span data-ttu-id="bf41c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf41c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





