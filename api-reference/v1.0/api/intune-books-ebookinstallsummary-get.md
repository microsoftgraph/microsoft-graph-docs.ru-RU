---
title: Get eBookInstallSummary
description: Чтение свойств и связей объекта eBookInstallSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b62a12a1b8a616bfd9ef9d8188d4ebe53cf23092
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570535"
---
# <a name="get-ebookinstallsummary"></a><span data-ttu-id="c758f-103">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="c758f-103">Get eBookInstallSummary</span></span>

> <span data-ttu-id="c758f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c758f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c758f-105">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c758f-105">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c758f-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c758f-106">Prerequisites</span></span>
<span data-ttu-id="c758f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c758f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c758f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c758f-109">Permission type</span></span>|<span data-ttu-id="c758f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c758f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c758f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c758f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c758f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c758f-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c758f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c758f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c758f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c758f-114">Not supported.</span></span>|
|<span data-ttu-id="c758f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c758f-115">Application</span></span>|<span data-ttu-id="c758f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c758f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c758f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c758f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c758f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c758f-118">Optional query parameters</span></span>
<span data-ttu-id="c758f-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c758f-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c758f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c758f-120">Request headers</span></span>
|<span data-ttu-id="c758f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c758f-121">Header</span></span>|<span data-ttu-id="c758f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c758f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c758f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c758f-123">Authorization</span></span>|<span data-ttu-id="c758f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c758f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c758f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c758f-125">Accept</span></span>|<span data-ttu-id="c758f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c758f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c758f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c758f-127">Request body</span></span>
<span data-ttu-id="c758f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c758f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c758f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c758f-129">Response</span></span>
<span data-ttu-id="c758f-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c758f-130">If successful, this method returns a `200 OK` response code and [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c758f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c758f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c758f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c758f-132">Request</span></span>
<span data-ttu-id="c758f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c758f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

### <a name="response"></a><span data-ttu-id="c758f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c758f-134">Response</span></span>
<span data-ttu-id="c758f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c758f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



