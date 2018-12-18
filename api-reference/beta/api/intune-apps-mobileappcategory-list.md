---
title: Перечисление объектов mobileAppCategory
description: Список свойств и связей объектов mobileAppCategory.
author: tfitzmac
ms.openlocfilehash: 1776a4c563a283a592d2a0ad37dc215423e91d0d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304825"
---
# <a name="list-mobileappcategories"></a><span data-ttu-id="af92b-103">Перечисление объектов mobileAppCategory</span><span class="sxs-lookup"><span data-stu-id="af92b-103">List mobileAppCategories</span></span>

> <span data-ttu-id="af92b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="af92b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af92b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af92b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af92b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="af92b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af92b-107">Список свойств и связей объектов [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).</span><span class="sxs-lookup"><span data-stu-id="af92b-107">List properties and relationships of the [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af92b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="af92b-108">Prerequisites</span></span>
<span data-ttu-id="af92b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af92b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af92b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af92b-111">Permission type</span></span>|<span data-ttu-id="af92b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af92b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af92b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af92b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af92b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="af92b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="af92b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af92b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af92b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af92b-116">Not supported.</span></span>|
|<span data-ttu-id="af92b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af92b-117">Application</span></span>|<span data-ttu-id="af92b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af92b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af92b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af92b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppCategories
GET /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="af92b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af92b-120">Request headers</span></span>
|<span data-ttu-id="af92b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af92b-121">Header</span></span>|<span data-ttu-id="af92b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="af92b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af92b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af92b-123">Authorization</span></span>|<span data-ttu-id="af92b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="af92b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af92b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="af92b-125">Accept</span></span>|<span data-ttu-id="af92b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af92b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af92b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af92b-127">Request body</span></span>
<span data-ttu-id="af92b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="af92b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af92b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="af92b-129">Response</span></span>
<span data-ttu-id="af92b-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="af92b-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af92b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="af92b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="af92b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="af92b-132">Request</span></span>
<span data-ttu-id="af92b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af92b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppCategories
```

### <a name="response"></a><span data-ttu-id="af92b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="af92b-134">Response</span></span>
<span data-ttu-id="af92b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="af92b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppCategory",
      "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```





