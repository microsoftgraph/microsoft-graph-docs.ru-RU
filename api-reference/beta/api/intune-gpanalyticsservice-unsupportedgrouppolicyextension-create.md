---
title: Создание неподтвердимойGroupPolicyExtension
description: Создайте новый объект UnsupportedGroupPolicyExtension.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ccee92daa5d468dcebebd59acaa764bd65297195
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149823"
---
# <a name="create-unsupportedgrouppolicyextension"></a><span data-ttu-id="1ef65-103">Создание неподтвердимойGroupPolicyExtension</span><span class="sxs-lookup"><span data-stu-id="1ef65-103">Create unsupportedGroupPolicyExtension</span></span>

<span data-ttu-id="1ef65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ef65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ef65-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ef65-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ef65-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ef65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ef65-107">Создайте новый [объект UnsupportedGroupPolicyExtension.](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)</span><span class="sxs-lookup"><span data-stu-id="1ef65-107">Create a new [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ef65-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1ef65-108">Prerequisites</span></span>
<span data-ttu-id="1ef65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ef65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ef65-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ef65-111">Permission type</span></span>|<span data-ttu-id="1ef65-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ef65-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ef65-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ef65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ef65-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ef65-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ef65-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ef65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ef65-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ef65-116">Not supported.</span></span>|
|<span data-ttu-id="1ef65-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1ef65-117">Application</span></span>|<span data-ttu-id="1ef65-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ef65-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ef65-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ef65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/unsupportedGroupPolicyExtensions
```

## <a name="request-headers"></a><span data-ttu-id="1ef65-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1ef65-120">Request headers</span></span>
|<span data-ttu-id="1ef65-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ef65-121">Header</span></span>|<span data-ttu-id="1ef65-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1ef65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ef65-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ef65-123">Authorization</span></span>|<span data-ttu-id="1ef65-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ef65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ef65-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1ef65-125">Accept</span></span>|<span data-ttu-id="1ef65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ef65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ef65-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ef65-127">Request body</span></span>
<span data-ttu-id="1ef65-128">В теле запроса поставляем представление JSON для неподдерживаемого объектаGroupPolicyExtension.</span><span class="sxs-lookup"><span data-stu-id="1ef65-128">In the request body, supply a JSON representation for the unsupportedGroupPolicyExtension object.</span></span>

<span data-ttu-id="1ef65-129">В следующей таблице показаны свойства, необходимые при создании неподтвершеннойGroupPolicyExtension.</span><span class="sxs-lookup"><span data-stu-id="1ef65-129">The following table shows the properties that are required when you create the unsupportedGroupPolicyExtension.</span></span>

|<span data-ttu-id="1ef65-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ef65-130">Property</span></span>|<span data-ttu-id="1ef65-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1ef65-131">Type</span></span>|<span data-ttu-id="1ef65-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1ef65-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ef65-133">id</span><span class="sxs-lookup"><span data-stu-id="1ef65-133">id</span></span>|<span data-ttu-id="1ef65-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1ef65-134">String</span></span>|<span data-ttu-id="1ef65-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1ef65-135">Not yet documented</span></span>|
|<span data-ttu-id="1ef65-136">settingScope</span><span class="sxs-lookup"><span data-stu-id="1ef65-136">settingScope</span></span>|[<span data-ttu-id="1ef65-137">groupPolicySettingScope</span><span class="sxs-lookup"><span data-stu-id="1ef65-137">groupPolicySettingScope</span></span>](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|<span data-ttu-id="1ef65-138">Настройка области неподтверченного расширения.</span><span class="sxs-lookup"><span data-stu-id="1ef65-138">Setting Scope of the unsupported extension.</span></span> <span data-ttu-id="1ef65-139">Возможные значения: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="1ef65-139">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="1ef65-140">namespaceUrl</span><span class="sxs-lookup"><span data-stu-id="1ef65-140">namespaceUrl</span></span>|<span data-ttu-id="1ef65-141">Строка</span><span class="sxs-lookup"><span data-stu-id="1ef65-141">String</span></span>|<span data-ttu-id="1ef65-142">Url-адрес пространства имен неподтверченного расширения.</span><span class="sxs-lookup"><span data-stu-id="1ef65-142">Namespace Url of the unsupported extension.</span></span>|
|<span data-ttu-id="1ef65-143">extensionType</span><span class="sxs-lookup"><span data-stu-id="1ef65-143">extensionType</span></span>|<span data-ttu-id="1ef65-144">Строка</span><span class="sxs-lookup"><span data-stu-id="1ef65-144">String</span></span>|<span data-ttu-id="1ef65-145">ExtensionType неподтверченного расширения.</span><span class="sxs-lookup"><span data-stu-id="1ef65-145">ExtensionType of the unsupported extension.</span></span>|
|<span data-ttu-id="1ef65-146">nodeName</span><span class="sxs-lookup"><span data-stu-id="1ef65-146">nodeName</span></span>|<span data-ttu-id="1ef65-147">Строка</span><span class="sxs-lookup"><span data-stu-id="1ef65-147">String</span></span>|<span data-ttu-id="1ef65-148">Имя узла неподтверченного расширения.</span><span class="sxs-lookup"><span data-stu-id="1ef65-148">Node name of the unsupported extension.</span></span>|



## <a name="response"></a><span data-ttu-id="1ef65-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ef65-149">Response</span></span>
<span data-ttu-id="1ef65-150">В случае успешной работы этот метод возвращает код ответа и неподтвердимый `201 Created` [объектGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1ef65-150">If successful, this method returns a `201 Created` response code and a [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ef65-151">Пример</span><span class="sxs-lookup"><span data-stu-id="1ef65-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ef65-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ef65-152">Request</span></span>
<span data-ttu-id="1ef65-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ef65-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1ef65-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ef65-154">Response</span></span>
<span data-ttu-id="1ef65-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ef65-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




