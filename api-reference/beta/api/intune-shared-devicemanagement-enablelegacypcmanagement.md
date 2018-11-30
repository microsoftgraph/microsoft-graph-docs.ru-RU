---
title: Действие enableLegacyPcManagement
description: Н/Д
ms.openlocfilehash: c9feaaea9e8b3c9573db95b6dd3f9aaae91243e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081696"
---
# <a name="enablelegacypcmanagement-action"></a><span data-ttu-id="cdd67-103">Действие enableLegacyPcManagement</span><span class="sxs-lookup"><span data-stu-id="cdd67-103">enableLegacyPcManagement action</span></span>

> <span data-ttu-id="cdd67-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cdd67-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cdd67-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdd67-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cdd67-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cdd67-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cdd67-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cdd67-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cdd67-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cdd67-108">Prerequisites</span></span>
<span data-ttu-id="cdd67-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdd67-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdd67-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdd67-111">Permission type</span></span>|<span data-ttu-id="cdd67-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdd67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdd67-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdd67-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cdd67-114">&nbsp;&nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="cdd67-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="cdd67-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdd67-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cdd67-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdd67-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdd67-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdd67-117">Not supported.</span></span>|
|<span data-ttu-id="cdd67-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdd67-118">Application</span></span>|<span data-ttu-id="cdd67-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdd67-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdd67-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdd67-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableLegacyPcManagement
```

## <a name="request-headers"></a><span data-ttu-id="cdd67-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdd67-121">Request headers</span></span>
|<span data-ttu-id="cdd67-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cdd67-122">Header</span></span>|<span data-ttu-id="cdd67-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cdd67-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdd67-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdd67-124">Authorization</span></span>|<span data-ttu-id="cdd67-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cdd67-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdd67-126">Accept</span><span class="sxs-lookup"><span data-stu-id="cdd67-126">Accept</span></span>|<span data-ttu-id="cdd67-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cdd67-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdd67-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdd67-128">Request body</span></span>
<span data-ttu-id="cdd67-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cdd67-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdd67-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="cdd67-130">Response</span></span>
<span data-ttu-id="cdd67-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cdd67-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cdd67-132">Пример</span><span class="sxs-lookup"><span data-stu-id="cdd67-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="cdd67-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdd67-133">Request</span></span>
<span data-ttu-id="cdd67-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdd67-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableLegacyPcManagement
```

### <a name="response"></a><span data-ttu-id="cdd67-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="cdd67-135">Response</span></span>
<span data-ttu-id="cdd67-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cdd67-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





