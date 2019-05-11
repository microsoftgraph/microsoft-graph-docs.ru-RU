---
title: Список Секуритибаселинетемплатес
description: Список свойств и связей объектов Секуритибаселинетемплате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6276cfe94eac8db637ce50738dc27e667f1106f2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33911688"
---
# <a name="list-securitybaselinetemplates"></a><span data-ttu-id="9f2af-103">Список Секуритибаселинетемплатес</span><span class="sxs-lookup"><span data-stu-id="9f2af-103">List securityBaselineTemplates</span></span>

> <span data-ttu-id="9f2af-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f2af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f2af-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f2af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f2af-106">Список свойств и связей объектов [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="9f2af-106">List properties and relationships of the [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f2af-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f2af-107">Prerequisites</span></span>
<span data-ttu-id="9f2af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f2af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f2af-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f2af-110">Permission type</span></span>|<span data-ttu-id="9f2af-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f2af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f2af-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f2af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f2af-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f2af-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9f2af-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f2af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f2af-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f2af-115">Not supported.</span></span>|
|<span data-ttu-id="9f2af-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f2af-116">Application</span></span>|<span data-ttu-id="9f2af-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f2af-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f2af-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f2af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="9f2af-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f2af-119">Request headers</span></span>
|<span data-ttu-id="9f2af-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f2af-120">Header</span></span>|<span data-ttu-id="9f2af-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9f2af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f2af-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f2af-122">Authorization</span></span>|<span data-ttu-id="9f2af-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f2af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f2af-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9f2af-124">Accept</span></span>|<span data-ttu-id="9f2af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f2af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f2af-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f2af-126">Request body</span></span>
<span data-ttu-id="9f2af-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f2af-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f2af-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f2af-128">Response</span></span>
<span data-ttu-id="9f2af-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f2af-129">If successful, this method returns a `200 OK` response code and a collection of [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f2af-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9f2af-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f2af-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f2af-131">Request</span></span>
<span data-ttu-id="9f2af-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f2af-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates
```

### <a name="response"></a><span data-ttu-id="9f2af-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f2af-133">Response</span></span>
<span data-ttu-id="9f2af-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f2af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityBaselineTemplate",
      "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
      "displayName": "Display Name value",
      "description": "Description value",
      "versionInfo": "Version Info value",
      "isDeprecated": true,
      "intentCount": 11
    }
  ]
}
```




