---
title: Перечисление объектов mobileAppContent
description: Список свойств и связей объектов mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: afd38f27587ff7c92afb1a839f5233c30ac39de2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945883"
---
# <a name="list-mobileappcontents"></a><span data-ttu-id="f86ad-103">Перечисление объектов mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="f86ad-103">List mobileAppContents</span></span>

> <span data-ttu-id="f86ad-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f86ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f86ad-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f86ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f86ad-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f86ad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f86ad-107">Список свойств и связей объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="f86ad-107">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f86ad-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f86ad-108">Prerequisites</span></span>
<span data-ttu-id="f86ad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f86ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f86ad-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f86ad-111">Permission type</span></span>|<span data-ttu-id="f86ad-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f86ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f86ad-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f86ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f86ad-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f86ad-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f86ad-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f86ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f86ad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f86ad-116">Not supported.</span></span>|
|<span data-ttu-id="f86ad-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f86ad-117">Application</span></span>|<span data-ttu-id="f86ad-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f86ad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f86ad-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f86ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="f86ad-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f86ad-120">Request headers</span></span>
|<span data-ttu-id="f86ad-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f86ad-121">Header</span></span>|<span data-ttu-id="f86ad-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f86ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f86ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f86ad-123">Authorization</span></span>|<span data-ttu-id="f86ad-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f86ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f86ad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f86ad-125">Accept</span></span>|<span data-ttu-id="f86ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f86ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f86ad-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f86ad-127">Request body</span></span>
<span data-ttu-id="f86ad-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f86ad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f86ad-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f86ad-129">Response</span></span>
<span data-ttu-id="f86ad-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContent](../resources/intune-apps-mobileappcontent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f86ad-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f86ad-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f86ad-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f86ad-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f86ad-132">Request</span></span>
<span data-ttu-id="f86ad-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f86ad-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
```

### <a name="response"></a><span data-ttu-id="f86ad-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f86ad-134">Response</span></span>
<span data-ttu-id="f86ad-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f86ad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 148

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppContent",
      "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
    }
  ]
}
```





