---
title: Удалить vppToken
description: Удаляет vppToken.
ms.openlocfilehash: 7ff527010292ba42618d523b32b8b30133f7fdc0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077616"
---
# <a name="delete-vpptoken"></a><span data-ttu-id="a34e9-103">Удалить vppToken</span><span class="sxs-lookup"><span data-stu-id="a34e9-103">Delete vppToken</span></span>

> <span data-ttu-id="a34e9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a34e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a34e9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a34e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a34e9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a34e9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a34e9-107">Удаляет [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="a34e9-107">Deletes a [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a34e9-108">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="a34e9-108">Prerequisites</span></span>
<span data-ttu-id="a34e9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a34e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a34e9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a34e9-111">Permission type</span></span>|<span data-ttu-id="a34e9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a34e9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a34e9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a34e9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a34e9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a34e9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a34e9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a34e9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a34e9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a34e9-116">Not supported.</span></span>|
|<span data-ttu-id="a34e9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a34e9-117">Application</span></span>|<span data-ttu-id="a34e9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a34e9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a34e9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a34e9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="a34e9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a34e9-120">Request headers</span></span>
|<span data-ttu-id="a34e9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a34e9-121">Header</span></span>|<span data-ttu-id="a34e9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a34e9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a34e9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a34e9-123">Authorization</span></span>|<span data-ttu-id="a34e9-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a34e9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a34e9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a34e9-125">Accept</span></span>|<span data-ttu-id="a34e9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a34e9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a34e9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a34e9-127">Request body</span></span>
<span data-ttu-id="a34e9-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a34e9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a34e9-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a34e9-129">Response</span></span>
<span data-ttu-id="a34e9-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a34e9-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a34e9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a34e9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a34e9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a34e9-132">Request</span></span>
<span data-ttu-id="a34e9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a34e9-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
```

### <a name="response"></a><span data-ttu-id="a34e9-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a34e9-134">Response</span></span>
<span data-ttu-id="a34e9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="a34e9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





