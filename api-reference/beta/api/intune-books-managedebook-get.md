---
title: Get managedEBook
description: Чтение свойств и связей объекта managedEBook.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 32848bfd81dbc94b74a99f505f95482732451457
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43392497"
---
# <a name="get-managedebook"></a><span data-ttu-id="f96a0-103">Get managedEBook</span><span class="sxs-lookup"><span data-stu-id="f96a0-103">Get managedEBook</span></span>

<span data-ttu-id="f96a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f96a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f96a0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f96a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f96a0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f96a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f96a0-107">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="f96a0-107">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f96a0-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f96a0-108">Prerequisites</span></span>
<span data-ttu-id="f96a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f96a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f96a0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f96a0-111">Permission type</span></span>|<span data-ttu-id="f96a0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f96a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f96a0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f96a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f96a0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f96a0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f96a0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f96a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f96a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f96a0-116">Not supported.</span></span>|
|<span data-ttu-id="f96a0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f96a0-117">Application</span></span>|<span data-ttu-id="f96a0-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f96a0-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f96a0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f96a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f96a0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f96a0-120">Optional query parameters</span></span>
<span data-ttu-id="f96a0-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f96a0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f96a0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f96a0-122">Request headers</span></span>
|<span data-ttu-id="f96a0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f96a0-123">Header</span></span>|<span data-ttu-id="f96a0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f96a0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f96a0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f96a0-125">Authorization</span></span>|<span data-ttu-id="f96a0-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f96a0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f96a0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f96a0-127">Accept</span></span>|<span data-ttu-id="f96a0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f96a0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f96a0-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f96a0-129">Request body</span></span>
<span data-ttu-id="f96a0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f96a0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f96a0-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f96a0-131">Response</span></span>
<span data-ttu-id="f96a0-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [managedEBook](../resources/intune-books-managedebook.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f96a0-132">If successful, this method returns a `200 OK` response code and [managedEBook](../resources/intune-books-managedebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f96a0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f96a0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f96a0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f96a0-134">Request</span></span>
<span data-ttu-id="f96a0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f96a0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="f96a0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f96a0-136">Response</span></span>
<span data-ttu-id="f96a0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f96a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



