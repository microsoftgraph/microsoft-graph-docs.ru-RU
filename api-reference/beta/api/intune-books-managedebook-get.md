---
title: Get managedEBook
description: Чтение свойств и связей объекта managedEBook.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cd574060ae085f64543434ff6eeda81d5c634046
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817684"
---
# <a name="get-managedebook"></a><span data-ttu-id="03d55-103">Get managedEBook</span><span class="sxs-lookup"><span data-stu-id="03d55-103">Get managedEBook</span></span>

> <span data-ttu-id="03d55-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="03d55-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03d55-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03d55-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03d55-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="03d55-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03d55-107">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="03d55-107">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="03d55-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="03d55-108">Prerequisites</span></span>
<span data-ttu-id="03d55-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03d55-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03d55-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03d55-111">Permission type</span></span>|<span data-ttu-id="03d55-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03d55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03d55-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03d55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03d55-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="03d55-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="03d55-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03d55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03d55-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03d55-116">Not supported.</span></span>|
|<span data-ttu-id="03d55-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03d55-117">Application</span></span>|<span data-ttu-id="03d55-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03d55-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03d55-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03d55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="03d55-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="03d55-120">Optional query parameters</span></span>
<span data-ttu-id="03d55-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="03d55-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="03d55-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03d55-122">Request headers</span></span>
|<span data-ttu-id="03d55-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03d55-123">Header</span></span>|<span data-ttu-id="03d55-124">Значение</span><span class="sxs-lookup"><span data-stu-id="03d55-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03d55-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="03d55-125">Authorization</span></span>|<span data-ttu-id="03d55-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="03d55-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03d55-127">Accept</span><span class="sxs-lookup"><span data-stu-id="03d55-127">Accept</span></span>|<span data-ttu-id="03d55-128">application/json</span><span class="sxs-lookup"><span data-stu-id="03d55-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03d55-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03d55-129">Request body</span></span>
<span data-ttu-id="03d55-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03d55-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03d55-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="03d55-131">Response</span></span>
<span data-ttu-id="03d55-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedEBook](../resources/intune-books-managedebook.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="03d55-132">If successful, this method returns a `200 OK` response code and [managedEBook](../resources/intune-books-managedebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03d55-133">Пример</span><span class="sxs-lookup"><span data-stu-id="03d55-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="03d55-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="03d55-134">Request</span></span>
<span data-ttu-id="03d55-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03d55-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="03d55-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="03d55-136">Response</span></span>
<span data-ttu-id="03d55-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="03d55-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "value": {
    "@odata.type": "#microsoft.graph.managedEBook",
    "id": "1fbd3558-3558-1fbd-5835-bd1f5835bd1f",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
    "largeCover": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "informationUrl": "https://example.com/informationUrl/",
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
  }
}
```





