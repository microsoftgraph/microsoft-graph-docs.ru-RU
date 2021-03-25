---
title: Обновление неподтвершеннойGroupPolicyExtension
description: Обновление свойств неподтвершенного объектаGroupPolicyExtension.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 569610e52d58c7a5eb8a8d18d8d5f43e03444f8a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153526"
---
# <a name="update-unsupportedgrouppolicyextension"></a><span data-ttu-id="12b90-103">Обновление неподтвершеннойGroupPolicyExtension</span><span class="sxs-lookup"><span data-stu-id="12b90-103">Update unsupportedGroupPolicyExtension</span></span>

<span data-ttu-id="12b90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12b90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12b90-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12b90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12b90-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12b90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12b90-107">Обновление свойств неподтвершенного [объектаGroupPolicyExtension.](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)</span><span class="sxs-lookup"><span data-stu-id="12b90-107">Update the properties of a [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12b90-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="12b90-108">Prerequisites</span></span>
<span data-ttu-id="12b90-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12b90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12b90-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12b90-111">Permission type</span></span>|<span data-ttu-id="12b90-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12b90-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12b90-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12b90-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12b90-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12b90-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12b90-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12b90-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12b90-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12b90-116">Not supported.</span></span>|
|<span data-ttu-id="12b90-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="12b90-117">Application</span></span>|<span data-ttu-id="12b90-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12b90-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12b90-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12b90-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions/{unsupportedGroupPolicyExtensionId}
```

## <a name="request-headers"></a><span data-ttu-id="12b90-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="12b90-120">Request headers</span></span>
|<span data-ttu-id="12b90-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12b90-121">Header</span></span>|<span data-ttu-id="12b90-122">Значение</span><span class="sxs-lookup"><span data-stu-id="12b90-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12b90-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12b90-123">Authorization</span></span>|<span data-ttu-id="12b90-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12b90-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12b90-125">Accept</span><span class="sxs-lookup"><span data-stu-id="12b90-125">Accept</span></span>|<span data-ttu-id="12b90-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12b90-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12b90-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12b90-127">Request body</span></span>
<span data-ttu-id="12b90-128">В теле запроса поставляем представление JSON для неподдерживаемого [объектаGroupPolicyExtension.](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)</span><span class="sxs-lookup"><span data-stu-id="12b90-128">In the request body, supply a JSON representation for the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

<span data-ttu-id="12b90-129">В следующей таблице показаны свойства, необходимые при создании [неподтвершеннойGroupPolicyExtension.](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)</span><span class="sxs-lookup"><span data-stu-id="12b90-129">The following table shows the properties that are required when you create the [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md).</span></span>

|<span data-ttu-id="12b90-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="12b90-130">Property</span></span>|<span data-ttu-id="12b90-131">Тип</span><span class="sxs-lookup"><span data-stu-id="12b90-131">Type</span></span>|<span data-ttu-id="12b90-132">Описание</span><span class="sxs-lookup"><span data-stu-id="12b90-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12b90-133">id</span><span class="sxs-lookup"><span data-stu-id="12b90-133">id</span></span>|<span data-ttu-id="12b90-134">Строка</span><span class="sxs-lookup"><span data-stu-id="12b90-134">String</span></span>|<span data-ttu-id="12b90-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="12b90-135">Not yet documented</span></span>|
|<span data-ttu-id="12b90-136">settingScope</span><span class="sxs-lookup"><span data-stu-id="12b90-136">settingScope</span></span>|[<span data-ttu-id="12b90-137">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="12b90-137">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="12b90-138">Настройка области неподтверченного расширения.</span><span class="sxs-lookup"><span data-stu-id="12b90-138">Setting Scope of the unsupported extension.</span></span> <span data-ttu-id="12b90-139">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="12b90-139">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="12b90-140">namespaceUrl</span><span class="sxs-lookup"><span data-stu-id="12b90-140">namespaceUrl</span></span>|<span data-ttu-id="12b90-141">Строка</span><span class="sxs-lookup"><span data-stu-id="12b90-141">String</span></span>|<span data-ttu-id="12b90-142">Url-адрес пространства имен неподтверченного расширения.</span><span class="sxs-lookup"><span data-stu-id="12b90-142">Namespace Url of the unsupported extension.</span></span>|
|<span data-ttu-id="12b90-143">extensionType</span><span class="sxs-lookup"><span data-stu-id="12b90-143">extensionType</span></span>|<span data-ttu-id="12b90-144">Строка</span><span class="sxs-lookup"><span data-stu-id="12b90-144">String</span></span>|<span data-ttu-id="12b90-145">ExtensionType неподтверченного расширения.</span><span class="sxs-lookup"><span data-stu-id="12b90-145">ExtensionType of the unsupported extension.</span></span>|
|<span data-ttu-id="12b90-146">nodeName</span><span class="sxs-lookup"><span data-stu-id="12b90-146">nodeName</span></span>|<span data-ttu-id="12b90-147">Строка</span><span class="sxs-lookup"><span data-stu-id="12b90-147">String</span></span>|<span data-ttu-id="12b90-148">Имя узла неподтверченного расширения.</span><span class="sxs-lookup"><span data-stu-id="12b90-148">Node name of the unsupported extension.</span></span>|



## <a name="response"></a><span data-ttu-id="12b90-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="12b90-149">Response</span></span>
<span data-ttu-id="12b90-150">В случае успешной работы этот метод возвращает код ответа и обновленный неподтвердимый `200 OK` [объектGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="12b90-150">If successful, this method returns a `200 OK` response code and an updated [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12b90-151">Пример</span><span class="sxs-lookup"><span data-stu-id="12b90-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="12b90-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="12b90-152">Request</span></span>
<span data-ttu-id="12b90-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12b90-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="12b90-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="12b90-154">Response</span></span>
<span data-ttu-id="12b90-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12b90-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




