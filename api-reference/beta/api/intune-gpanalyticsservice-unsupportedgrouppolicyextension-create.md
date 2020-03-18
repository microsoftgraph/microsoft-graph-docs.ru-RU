---
title: Создание Унсуппортедграупполициекстенсион
description: Создание нового объекта Унсуппортедграупполициекстенсион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5a7826e00c2b0bccb6fa7e3832995fa67ea9dbd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804571"
---
# <a name="create-unsupportedgrouppolicyextension"></a><span data-ttu-id="824fb-103">Создание Унсуппортедграупполициекстенсион</span><span class="sxs-lookup"><span data-stu-id="824fb-103">Create unsupportedGroupPolicyExtension</span></span>

> <span data-ttu-id="824fb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="824fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="824fb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="824fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="824fb-106">Создание нового объекта [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) .</span><span class="sxs-lookup"><span data-stu-id="824fb-106">Create a new [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="824fb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="824fb-107">Prerequisites</span></span>
<span data-ttu-id="824fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="824fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="824fb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="824fb-110">Permission type</span></span>|<span data-ttu-id="824fb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="824fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="824fb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="824fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="824fb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="824fb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="824fb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="824fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="824fb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="824fb-115">Not supported.</span></span>|
|<span data-ttu-id="824fb-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="824fb-116">Application</span></span>|<span data-ttu-id="824fb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="824fb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="824fb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="824fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
```

## <a name="request-headers"></a><span data-ttu-id="824fb-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="824fb-119">Request headers</span></span>
|<span data-ttu-id="824fb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="824fb-120">Header</span></span>|<span data-ttu-id="824fb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="824fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="824fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="824fb-122">Authorization</span></span>|<span data-ttu-id="824fb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="824fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="824fb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="824fb-124">Accept</span></span>|<span data-ttu-id="824fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="824fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="824fb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="824fb-126">Request body</span></span>
<span data-ttu-id="824fb-127">В тексте запроса добавьте представление объекта Унсуппортедграупполициекстенсион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="824fb-127">In the request body, supply a JSON representation for the unsupportedGroupPolicyExtension object.</span></span>

<span data-ttu-id="824fb-128">В следующей таблице приведены свойства, необходимые при создании Унсуппортедграупполициекстенсион.</span><span class="sxs-lookup"><span data-stu-id="824fb-128">The following table shows the properties that are required when you create the unsupportedGroupPolicyExtension.</span></span>

|<span data-ttu-id="824fb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="824fb-129">Property</span></span>|<span data-ttu-id="824fb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="824fb-130">Type</span></span>|<span data-ttu-id="824fb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="824fb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="824fb-132">id</span><span class="sxs-lookup"><span data-stu-id="824fb-132">id</span></span>|<span data-ttu-id="824fb-133">String</span><span class="sxs-lookup"><span data-stu-id="824fb-133">String</span></span>|<span data-ttu-id="824fb-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="824fb-134">Not yet documented</span></span>|
|<span data-ttu-id="824fb-135">сеттингскопе</span><span class="sxs-lookup"><span data-stu-id="824fb-135">settingScope</span></span>|[<span data-ttu-id="824fb-136">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="824fb-136">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="824fb-137">Задание области для неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="824fb-137">Setting Scope of the unsupported extension.</span></span> <span data-ttu-id="824fb-138">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="824fb-138">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="824fb-139">намеспацеурл</span><span class="sxs-lookup"><span data-stu-id="824fb-139">namespaceUrl</span></span>|<span data-ttu-id="824fb-140">String</span><span class="sxs-lookup"><span data-stu-id="824fb-140">String</span></span>|<span data-ttu-id="824fb-141">URL-адрес пространства имен неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="824fb-141">Namespace Url of the unsupported extension.</span></span>|
|<span data-ttu-id="824fb-142">екстенсионтипе</span><span class="sxs-lookup"><span data-stu-id="824fb-142">extensionType</span></span>|<span data-ttu-id="824fb-143">String</span><span class="sxs-lookup"><span data-stu-id="824fb-143">String</span></span>|<span data-ttu-id="824fb-144">Екстенсионтипе неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="824fb-144">ExtensionType of the unsupported extension.</span></span>|
|<span data-ttu-id="824fb-145">nodeName</span><span class="sxs-lookup"><span data-stu-id="824fb-145">nodeName</span></span>|<span data-ttu-id="824fb-146">String</span><span class="sxs-lookup"><span data-stu-id="824fb-146">String</span></span>|<span data-ttu-id="824fb-147">Имя узла неподдерживаемого расширения.</span><span class="sxs-lookup"><span data-stu-id="824fb-147">Node name of the unsupported extension.</span></span>|



## <a name="response"></a><span data-ttu-id="824fb-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="824fb-148">Response</span></span>
<span data-ttu-id="824fb-149">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [унсуппортедграупполициекстенсион](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="824fb-149">If successful, this method returns a `201 Created` response code and a [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="824fb-150">Пример</span><span class="sxs-lookup"><span data-stu-id="824fb-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="824fb-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="824fb-151">Request</span></span>
<span data-ttu-id="824fb-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="824fb-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="824fb-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="824fb-153">Response</span></span>
<span data-ttu-id="824fb-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="824fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




