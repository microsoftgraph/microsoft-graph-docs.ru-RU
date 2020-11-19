---
title: действие Креатемигратионрепорт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 27a73945b3b2ba060dafef0766fa2532d42369d5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49263094"
---
# <a name="createmigrationreport-action"></a><span data-ttu-id="f6c69-103">действие Креатемигратионрепорт</span><span class="sxs-lookup"><span data-stu-id="f6c69-103">createMigrationReport action</span></span>

<span data-ttu-id="f6c69-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6c69-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6c69-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6c69-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6c69-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6c69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6c69-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f6c69-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6c69-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f6c69-108">Prerequisites</span></span>
<span data-ttu-id="f6c69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6c69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6c69-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6c69-111">Permission type</span></span>|<span data-ttu-id="f6c69-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6c69-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6c69-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6c69-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f6c69-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c69-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f6c69-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6c69-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6c69-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6c69-116">Not supported.</span></span>|
|<span data-ttu-id="f6c69-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f6c69-117">Application</span></span>|<span data-ttu-id="f6c69-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c69-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6c69-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6c69-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports/createMigrationReport
```

## <a name="request-headers"></a><span data-ttu-id="f6c69-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f6c69-120">Request headers</span></span>
|<span data-ttu-id="f6c69-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6c69-121">Header</span></span>|<span data-ttu-id="f6c69-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f6c69-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6c69-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6c69-123">Authorization</span></span>|<span data-ttu-id="f6c69-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6c69-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6c69-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f6c69-125">Accept</span></span>|<span data-ttu-id="f6c69-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f6c69-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6c69-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6c69-127">Request body</span></span>
<span data-ttu-id="f6c69-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6c69-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f6c69-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f6c69-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f6c69-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6c69-130">Property</span></span>|<span data-ttu-id="f6c69-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f6c69-131">Type</span></span>|<span data-ttu-id="f6c69-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f6c69-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6c69-133">groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="f6c69-133">groupPolicyObjectFile</span></span>|[<span data-ttu-id="f6c69-134">groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="f6c69-134">groupPolicyObjectFile</span></span>](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|<span data-ttu-id="f6c69-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="f6c69-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f6c69-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6c69-136">Response</span></span>
<span data-ttu-id="f6c69-137">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6c69-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6c69-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f6c69-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6c69-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6c69-139">Request</span></span>
<span data-ttu-id="f6c69-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6c69-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/createMigrationReport

Content-type: application/json
Content-length: 438

{
  "groupPolicyObjectFile": {
    "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
    "id": "65c0499d-499d-65c0-9d49-c0659d49c065",
    "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
    "ouDistinguishedName": "Ou Distinguished Name value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "content": "Content value"
  }
}
```

### <a name="response"></a><span data-ttu-id="f6c69-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6c69-141">Response</span></span>
<span data-ttu-id="f6c69-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6c69-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 48

{
  "value": "Create Migration Report value"
}
```




