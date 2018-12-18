---
title: Удаление объекта microsoftStoreForBusinessApp
description: Удаляет объект microsoftStoreForBusinessApp.
author: tfitzmac
ms.openlocfilehash: f84057191462268e6c51c3b1fa1336d2cb89d371
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326259"
---
# <a name="delete-microsoftstoreforbusinessapp"></a><span data-ttu-id="28356-103">Удаление объекта microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="28356-103">Delete microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="28356-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="28356-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28356-105">Удаляет объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="28356-105">Deletes a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="28356-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="28356-106">Prerequisites</span></span>
<span data-ttu-id="28356-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28356-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28356-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28356-109">Permission type</span></span>|<span data-ttu-id="28356-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="28356-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28356-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28356-111">Delegated (work or school account)</span></span>|<span data-ttu-id="28356-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28356-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="28356-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28356-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28356-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28356-114">Not supported.</span></span>|
|<span data-ttu-id="28356-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28356-115">Application</span></span>|<span data-ttu-id="28356-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28356-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28356-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28356-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="28356-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28356-118">Request headers</span></span>
|<span data-ttu-id="28356-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28356-119">Header</span></span>|<span data-ttu-id="28356-120">Значение</span><span class="sxs-lookup"><span data-stu-id="28356-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28356-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28356-121">Authorization</span></span>|<span data-ttu-id="28356-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="28356-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28356-123">Accept</span><span class="sxs-lookup"><span data-stu-id="28356-123">Accept</span></span>|<span data-ttu-id="28356-124">application/json</span><span class="sxs-lookup"><span data-stu-id="28356-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28356-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28356-125">Request body</span></span>
<span data-ttu-id="28356-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28356-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28356-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="28356-127">Response</span></span>
<span data-ttu-id="28356-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="28356-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="28356-129">Пример</span><span class="sxs-lookup"><span data-stu-id="28356-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="28356-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="28356-130">Request</span></span>
<span data-ttu-id="28356-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28356-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="28356-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="28356-132">Response</span></span>
<span data-ttu-id="28356-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="28356-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



