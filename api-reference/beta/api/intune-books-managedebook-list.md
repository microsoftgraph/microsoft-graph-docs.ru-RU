---
title: Перечисление объектов managedEBook
description: Список свойств и связей объектов managedEBook.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ed8c5ef0d0e308a6fe241bc8b73516e69af3cc97
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43392490"
---
# <a name="list-managedebooks"></a><span data-ttu-id="c6201-103">Перечисление объектов managedEBook</span><span class="sxs-lookup"><span data-stu-id="c6201-103">List managedEBooks</span></span>

<span data-ttu-id="c6201-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6201-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6201-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6201-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6201-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6201-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6201-107">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="c6201-107">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6201-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c6201-108">Prerequisites</span></span>
<span data-ttu-id="c6201-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6201-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6201-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6201-111">Permission type</span></span>|<span data-ttu-id="c6201-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6201-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6201-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6201-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6201-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6201-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c6201-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6201-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6201-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6201-116">Not supported.</span></span>|
|<span data-ttu-id="c6201-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="c6201-117">Application</span></span>|<span data-ttu-id="c6201-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6201-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6201-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6201-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="c6201-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c6201-120">Request headers</span></span>
|<span data-ttu-id="c6201-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c6201-121">Header</span></span>|<span data-ttu-id="c6201-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c6201-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6201-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6201-123">Authorization</span></span>|<span data-ttu-id="c6201-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6201-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6201-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c6201-125">Accept</span></span>|<span data-ttu-id="c6201-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6201-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6201-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6201-127">Request body</span></span>
<span data-ttu-id="c6201-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6201-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6201-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6201-129">Response</span></span>
<span data-ttu-id="c6201-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedEBook](../resources/intune-books-managedebook.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c6201-130">If successful, this method returns a `200 OK` response code and a collection of [managedEBook](../resources/intune-books-managedebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6201-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c6201-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6201-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6201-132">Request</span></span>
<span data-ttu-id="c6201-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6201-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="c6201-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6201-134">Response</span></span>
<span data-ttu-id="c6201-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c6201-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



