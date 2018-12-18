---
title: Перечисление объектов managedEBook
description: Список свойств и связей объектов managedEBook.
author: tfitzmac
ms.openlocfilehash: dcfc293bb6b4d201af2f38dce5773b196281f51e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316487"
---
# <a name="list-managedebooks"></a><span data-ttu-id="cf400-103">Перечисление объектов managedEBook</span><span class="sxs-lookup"><span data-stu-id="cf400-103">List managedEBooks</span></span>

> <span data-ttu-id="cf400-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cf400-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf400-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf400-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf400-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cf400-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf400-107">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="cf400-107">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf400-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cf400-108">Prerequisites</span></span>
<span data-ttu-id="cf400-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf400-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf400-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf400-111">Permission type</span></span>|<span data-ttu-id="cf400-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf400-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf400-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf400-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf400-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf400-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cf400-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf400-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf400-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf400-116">Not supported.</span></span>|
|<span data-ttu-id="cf400-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf400-117">Application</span></span>|<span data-ttu-id="cf400-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf400-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf400-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf400-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="cf400-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf400-120">Request headers</span></span>
|<span data-ttu-id="cf400-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf400-121">Header</span></span>|<span data-ttu-id="cf400-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cf400-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf400-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf400-123">Authorization</span></span>|<span data-ttu-id="cf400-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cf400-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf400-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf400-125">Accept</span></span>|<span data-ttu-id="cf400-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf400-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf400-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf400-127">Request body</span></span>
<span data-ttu-id="cf400-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf400-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf400-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf400-129">Response</span></span>
<span data-ttu-id="cf400-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedEBook](../resources/intune-books-managedebook.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cf400-130">If successful, this method returns a `200 OK` response code and a collection of [managedEBook](../resources/intune-books-managedebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf400-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cf400-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf400-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf400-132">Request</span></span>
<span data-ttu-id="cf400-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf400-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="cf400-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf400-134">Response</span></span>
<span data-ttu-id="cf400-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cf400-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": [
    {
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
  ]
}
```





