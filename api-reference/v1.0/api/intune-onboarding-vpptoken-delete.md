---
title: Удалить vppToken
description: Удаляет vppToken.
author: tfitzmac
ms.openlocfilehash: 34d079883344f0725b87d4c1b46c92a37000fb40
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302858"
---
# <a name="delete-vpptoken"></a><span data-ttu-id="d1a02-103">Удалить vppToken</span><span class="sxs-lookup"><span data-stu-id="d1a02-103">Delete vppToken</span></span>

> <span data-ttu-id="d1a02-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d1a02-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1a02-105">Удаляет [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="d1a02-105">Deletes a [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d1a02-106">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="d1a02-106">Prerequisites</span></span>
<span data-ttu-id="d1a02-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1a02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1a02-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1a02-109">Permission type</span></span>|<span data-ttu-id="d1a02-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1a02-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1a02-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1a02-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d1a02-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1a02-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d1a02-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1a02-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1a02-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1a02-114">Not supported.</span></span>|
|<span data-ttu-id="d1a02-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1a02-115">Application</span></span>|<span data-ttu-id="d1a02-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1a02-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1a02-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1a02-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="d1a02-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1a02-118">Request headers</span></span>
|<span data-ttu-id="d1a02-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1a02-119">Header</span></span>|<span data-ttu-id="d1a02-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d1a02-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1a02-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1a02-121">Authorization</span></span>|<span data-ttu-id="d1a02-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d1a02-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1a02-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d1a02-123">Accept</span></span>|<span data-ttu-id="d1a02-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d1a02-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1a02-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1a02-125">Request body</span></span>
<span data-ttu-id="d1a02-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1a02-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1a02-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1a02-127">Response</span></span>
<span data-ttu-id="d1a02-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d1a02-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d1a02-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d1a02-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d1a02-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1a02-130">Request</span></span>
<span data-ttu-id="d1a02-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1a02-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
```

### <a name="response"></a><span data-ttu-id="d1a02-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1a02-132">Response</span></span>
<span data-ttu-id="d1a02-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d1a02-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



