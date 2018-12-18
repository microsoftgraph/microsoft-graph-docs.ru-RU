---
title: Действие beginOnboarding
description: Н/Д
author: tfitzmac
ms.openlocfilehash: e5d9d164e359484f6823c67c80169dbcef5116c5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337312"
---
# <a name="beginonboarding-action"></a><span data-ttu-id="36884-103">Действие beginOnboarding</span><span class="sxs-lookup"><span data-stu-id="36884-103">beginOnboarding action</span></span>

> <span data-ttu-id="36884-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="36884-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36884-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="36884-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36884-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="36884-106">Prerequisites</span></span>
<span data-ttu-id="36884-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36884-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36884-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36884-109">Permission type</span></span>|<span data-ttu-id="36884-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="36884-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36884-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36884-111">Delegated (work or school account)</span></span>|<span data-ttu-id="36884-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36884-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="36884-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36884-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36884-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36884-114">Not supported.</span></span>|
|<span data-ttu-id="36884-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36884-115">Application</span></span>|<span data-ttu-id="36884-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36884-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36884-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36884-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

## <a name="request-headers"></a><span data-ttu-id="36884-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36884-118">Request headers</span></span>
|<span data-ttu-id="36884-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36884-119">Header</span></span>|<span data-ttu-id="36884-120">Значение</span><span class="sxs-lookup"><span data-stu-id="36884-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36884-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36884-121">Authorization</span></span>|<span data-ttu-id="36884-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="36884-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36884-123">Accept</span><span class="sxs-lookup"><span data-stu-id="36884-123">Accept</span></span>|<span data-ttu-id="36884-124">application/json</span><span class="sxs-lookup"><span data-stu-id="36884-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36884-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36884-125">Request body</span></span>
<span data-ttu-id="36884-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36884-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36884-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="36884-127">Response</span></span>
<span data-ttu-id="36884-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="36884-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="36884-129">Пример</span><span class="sxs-lookup"><span data-stu-id="36884-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="36884-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="36884-130">Request</span></span>
<span data-ttu-id="36884-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36884-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}/beginOnboarding
```

### <a name="response"></a><span data-ttu-id="36884-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="36884-132">Response</span></span>
<span data-ttu-id="36884-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="36884-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



