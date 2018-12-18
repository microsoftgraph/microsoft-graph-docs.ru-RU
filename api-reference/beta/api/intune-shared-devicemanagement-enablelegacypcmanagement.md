---
title: Действие enableLegacyPcManagement
description: Н/Д
author: tfitzmac
ms.openlocfilehash: d24ca863e0b4cfb061cebc7ca805439d3cbcff17
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351928"
---
# <a name="enablelegacypcmanagement-action"></a><span data-ttu-id="40016-103">Действие enableLegacyPcManagement</span><span class="sxs-lookup"><span data-stu-id="40016-103">enableLegacyPcManagement action</span></span>

> <span data-ttu-id="40016-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="40016-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40016-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40016-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40016-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="40016-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40016-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="40016-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40016-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="40016-108">Prerequisites</span></span>
<span data-ttu-id="40016-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40016-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40016-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40016-111">Permission type</span></span>|<span data-ttu-id="40016-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40016-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40016-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40016-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="40016-114">&nbsp;&nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="40016-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="40016-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40016-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="40016-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40016-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40016-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40016-117">Not supported.</span></span>|
|<span data-ttu-id="40016-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40016-118">Application</span></span>|<span data-ttu-id="40016-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40016-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40016-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40016-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableLegacyPcManagement
```

## <a name="request-headers"></a><span data-ttu-id="40016-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40016-121">Request headers</span></span>
|<span data-ttu-id="40016-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40016-122">Header</span></span>|<span data-ttu-id="40016-123">Значение</span><span class="sxs-lookup"><span data-stu-id="40016-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40016-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40016-124">Authorization</span></span>|<span data-ttu-id="40016-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="40016-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40016-126">Accept</span><span class="sxs-lookup"><span data-stu-id="40016-126">Accept</span></span>|<span data-ttu-id="40016-127">application/json</span><span class="sxs-lookup"><span data-stu-id="40016-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40016-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40016-128">Request body</span></span>
<span data-ttu-id="40016-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40016-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40016-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="40016-130">Response</span></span>
<span data-ttu-id="40016-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="40016-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="40016-132">Пример</span><span class="sxs-lookup"><span data-stu-id="40016-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="40016-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="40016-133">Request</span></span>
<span data-ttu-id="40016-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40016-134">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableLegacyPcManagement
```

### <a name="response"></a><span data-ttu-id="40016-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="40016-135">Response</span></span>
<span data-ttu-id="40016-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="40016-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





