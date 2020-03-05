---
title: действие Креатемигратионрепорт
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e4aef4926934673586391cebffdf9156e257fe7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465508"
---
# <a name="createmigrationreport-action"></a><span data-ttu-id="5abba-103">действие Креатемигратионрепорт</span><span class="sxs-lookup"><span data-stu-id="5abba-103">createMigrationReport action</span></span>

<span data-ttu-id="5abba-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5abba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5abba-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5abba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5abba-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5abba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5abba-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5abba-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5abba-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5abba-108">Prerequisites</span></span>
<span data-ttu-id="5abba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5abba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5abba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5abba-111">Permission type</span></span>|<span data-ttu-id="5abba-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5abba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5abba-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5abba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5abba-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5abba-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5abba-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5abba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5abba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5abba-116">Not supported.</span></span>|
|<span data-ttu-id="5abba-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5abba-117">Application</span></span>|<span data-ttu-id="5abba-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5abba-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5abba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5abba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/createMigrationReport
```

## <a name="request-headers"></a><span data-ttu-id="5abba-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5abba-120">Request headers</span></span>
|<span data-ttu-id="5abba-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5abba-121">Header</span></span>|<span data-ttu-id="5abba-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5abba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5abba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5abba-123">Authorization</span></span>|<span data-ttu-id="5abba-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5abba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5abba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5abba-125">Accept</span></span>|<span data-ttu-id="5abba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5abba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5abba-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5abba-127">Request body</span></span>
<span data-ttu-id="5abba-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5abba-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5abba-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="5abba-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5abba-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5abba-130">Property</span></span>|<span data-ttu-id="5abba-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5abba-131">Type</span></span>|<span data-ttu-id="5abba-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5abba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5abba-133">groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="5abba-133">groupPolicyObjectFile</span></span>|[<span data-ttu-id="5abba-134">groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="5abba-134">groupPolicyObjectFile</span></span>](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|<span data-ttu-id="5abba-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5abba-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5abba-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5abba-136">Response</span></span>
<span data-ttu-id="5abba-137">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5abba-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5abba-138">Пример</span><span class="sxs-lookup"><span data-stu-id="5abba-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="5abba-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="5abba-139">Request</span></span>
<span data-ttu-id="5abba-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5abba-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/createMigrationReport

Content-type: application/json
Content-length: 191

{
  "groupPolicyObjectFile": {
    "@odata.type": "microsoft.graph.groupPolicyObjectFile",
    "ouDistinguishedName": "Ou Distinguished Name value",
    "content": "Content value"
  }
}
```

### <a name="response"></a><span data-ttu-id="5abba-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5abba-141">Response</span></span>
<span data-ttu-id="5abba-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5abba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Create Migration Report value"
}
```





