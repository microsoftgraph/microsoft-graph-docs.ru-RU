---
title: Действие syncMicrosoftStoreForBusinessApps
description: Синхронизирует учетную запись Intune с Microsoft Store для бизнеса
author: tfitzmac
ms.openlocfilehash: b26b379631cf5b28594e3cf247b735d6118e9b40
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354336"
---
# <a name="syncmicrosoftstoreforbusinessapps-action"></a><span data-ttu-id="8abeb-103">Действие syncMicrosoftStoreForBusinessApps</span><span class="sxs-lookup"><span data-stu-id="8abeb-103">syncMicrosoftStoreForBusinessApps action</span></span>

> <span data-ttu-id="8abeb-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8abeb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8abeb-105">Синхронизирует учетную запись Intune с Microsoft Store для бизнеса</span><span class="sxs-lookup"><span data-stu-id="8abeb-105">Syncs Intune account with Microsoft Store For Business</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8abeb-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8abeb-106">Prerequisites</span></span>
<span data-ttu-id="8abeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8abeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8abeb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8abeb-109">Permission type</span></span>|<span data-ttu-id="8abeb-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8abeb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8abeb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8abeb-111">Delegated (work or school account)</span></span>| 
| <span data-ttu-id="8abeb-112">&nbsp;&nbsp; _Адаптация новых сотрудников_</span><span class="sxs-lookup"><span data-stu-id="8abeb-112">&nbsp; &nbsp; _Onboarding_</span></span> | <span data-ttu-id="8abeb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8abeb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8abeb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8abeb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8abeb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8abeb-115">Not supported.</span></span>|
|<span data-ttu-id="8abeb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8abeb-116">Application</span></span>|<span data-ttu-id="8abeb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8abeb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8abeb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8abeb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

## <a name="request-headers"></a><span data-ttu-id="8abeb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8abeb-119">Request headers</span></span>
|<span data-ttu-id="8abeb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8abeb-120">Header</span></span>|<span data-ttu-id="8abeb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8abeb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8abeb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8abeb-122">Authorization</span></span>|<span data-ttu-id="8abeb-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8abeb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8abeb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8abeb-124">Accept</span></span>|<span data-ttu-id="8abeb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8abeb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8abeb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8abeb-126">Request body</span></span>
<span data-ttu-id="8abeb-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8abeb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8abeb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="8abeb-128">Response</span></span>
<span data-ttu-id="8abeb-129">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8abeb-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example-request"></a><span data-ttu-id="8abeb-130">Пример запроса</span><span class="sxs-lookup"><span data-stu-id="8abeb-130">Example request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/syncMicrosoftStoreForBusinessApps
```

### <a name="response"></a><span data-ttu-id="8abeb-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="8abeb-131">Response</span></span>

<span data-ttu-id="8abeb-132">Для краткости может усекаться объект ответа, показано ниже.</span><span class="sxs-lookup"><span data-stu-id="8abeb-132">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8abeb-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8abeb-133">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



