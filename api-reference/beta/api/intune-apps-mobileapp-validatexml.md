---
title: действие Валидатексмл
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 007f039988515cd99b40fa314b9baec12afd7d02
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177963"
---
# <a name="validatexml-action"></a><span data-ttu-id="18878-103">действие Валидатексмл</span><span class="sxs-lookup"><span data-stu-id="18878-103">validateXml action</span></span>

<span data-ttu-id="18878-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18878-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18878-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18878-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18878-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18878-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18878-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="18878-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18878-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="18878-108">Prerequisites</span></span>
<span data-ttu-id="18878-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18878-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18878-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18878-111">Permission type</span></span>|<span data-ttu-id="18878-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18878-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18878-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18878-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18878-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18878-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="18878-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18878-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18878-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18878-116">Not supported.</span></span>|
|<span data-ttu-id="18878-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18878-117">Application</span></span>|<span data-ttu-id="18878-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18878-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18878-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18878-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/validateXml
```

## <a name="request-headers"></a><span data-ttu-id="18878-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="18878-120">Request headers</span></span>
|<span data-ttu-id="18878-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18878-121">Header</span></span>|<span data-ttu-id="18878-122">Значение</span><span class="sxs-lookup"><span data-stu-id="18878-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18878-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18878-123">Authorization</span></span>|<span data-ttu-id="18878-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18878-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18878-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18878-125">Accept</span></span>|<span data-ttu-id="18878-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18878-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18878-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18878-127">Request body</span></span>
<span data-ttu-id="18878-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18878-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="18878-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="18878-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="18878-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="18878-130">Property</span></span>|<span data-ttu-id="18878-131">Тип</span><span class="sxs-lookup"><span data-stu-id="18878-131">Type</span></span>|<span data-ttu-id="18878-132">Описание</span><span class="sxs-lookup"><span data-stu-id="18878-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18878-133">оффицеконфигуратионксмл</span><span class="sxs-lookup"><span data-stu-id="18878-133">officeConfigurationXml</span></span>|<span data-ttu-id="18878-134">Binary</span><span class="sxs-lookup"><span data-stu-id="18878-134">Binary</span></span>|<span data-ttu-id="18878-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="18878-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="18878-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="18878-136">Response</span></span>
<span data-ttu-id="18878-137">При успешном выполнении это действие возвращает код отклика `200 OK` и объект String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18878-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18878-138">Пример</span><span class="sxs-lookup"><span data-stu-id="18878-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="18878-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="18878-139">Request</span></span>
<span data-ttu-id="18878-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18878-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/validateXml

Content-type: application/json
Content-length: 68

{
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="18878-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="18878-141">Response</span></span>
<span data-ttu-id="18878-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18878-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 37

{
  "value": "Validate Xml value"
}
```



