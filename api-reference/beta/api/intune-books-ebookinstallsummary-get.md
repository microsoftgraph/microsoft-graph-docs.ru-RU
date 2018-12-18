---
title: Get eBookInstallSummary
description: Чтение свойств и связей объекта eBookInstallSummary.
author: tfitzmac
ms.openlocfilehash: 3147148562bfd9fbb751ffcfb316367f0bb5baeb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324467"
---
# <a name="get-ebookinstallsummary"></a><span data-ttu-id="870ad-103">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="870ad-103">Get eBookInstallSummary</span></span>

> <span data-ttu-id="870ad-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="870ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="870ad-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="870ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="870ad-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="870ad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="870ad-107">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="870ad-107">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="870ad-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="870ad-108">Prerequisites</span></span>
<span data-ttu-id="870ad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="870ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="870ad-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="870ad-111">Permission type</span></span>|<span data-ttu-id="870ad-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="870ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="870ad-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="870ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="870ad-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="870ad-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="870ad-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="870ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="870ad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="870ad-116">Not supported.</span></span>|
|<span data-ttu-id="870ad-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="870ad-117">Application</span></span>|<span data-ttu-id="870ad-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="870ad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="870ad-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="870ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="870ad-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="870ad-120">Optional query parameters</span></span>
<span data-ttu-id="870ad-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="870ad-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="870ad-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="870ad-122">Request headers</span></span>
|<span data-ttu-id="870ad-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="870ad-123">Header</span></span>|<span data-ttu-id="870ad-124">Значение</span><span class="sxs-lookup"><span data-stu-id="870ad-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="870ad-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="870ad-125">Authorization</span></span>|<span data-ttu-id="870ad-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="870ad-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="870ad-127">Accept</span><span class="sxs-lookup"><span data-stu-id="870ad-127">Accept</span></span>|<span data-ttu-id="870ad-128">application/json</span><span class="sxs-lookup"><span data-stu-id="870ad-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="870ad-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="870ad-129">Request body</span></span>
<span data-ttu-id="870ad-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="870ad-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="870ad-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="870ad-131">Response</span></span>
<span data-ttu-id="870ad-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="870ad-132">If successful, this method returns a `200 OK` response code and [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="870ad-133">Пример</span><span class="sxs-lookup"><span data-stu-id="870ad-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="870ad-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="870ad-134">Request</span></span>
<span data-ttu-id="870ad-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="870ad-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

### <a name="response"></a><span data-ttu-id="870ad-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="870ad-136">Response</span></span>
<span data-ttu-id="870ad-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="870ad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 320

{
  "value": {
    "@odata.type": "#microsoft.graph.eBookInstallSummary",
    "id": "9708ad78-ad78-9708-78ad-089778ad0897",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7,
    "installedUserCount": 2,
    "failedUserCount": 15,
    "notInstalledUserCount": 5
  }
}
```





