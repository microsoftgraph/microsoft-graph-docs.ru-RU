---
title: Список Манажедебуккатегориес
description: Список свойств и связей объектов Манажедебуккатегори.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a02b69624664d74ae9fabaad1066ff1d625e144
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966973"
---
# <a name="list-managedebookcategories"></a><span data-ttu-id="65bc5-103">Список Манажедебуккатегориес</span><span class="sxs-lookup"><span data-stu-id="65bc5-103">List managedEBookCategories</span></span>

> <span data-ttu-id="65bc5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65bc5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65bc5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65bc5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65bc5-106">Список свойств и связей объектов [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="65bc5-106">List properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65bc5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="65bc5-107">Prerequisites</span></span>
<span data-ttu-id="65bc5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65bc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65bc5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65bc5-110">Permission type</span></span>|<span data-ttu-id="65bc5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="65bc5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65bc5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65bc5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65bc5-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="65bc5-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="65bc5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65bc5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65bc5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65bc5-115">Not supported.</span></span>|
|<span data-ttu-id="65bc5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65bc5-116">Application</span></span>|<span data-ttu-id="65bc5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65bc5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65bc5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65bc5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBookCategories
GET /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="65bc5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65bc5-119">Request headers</span></span>
|<span data-ttu-id="65bc5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65bc5-120">Header</span></span>|<span data-ttu-id="65bc5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="65bc5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65bc5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65bc5-122">Authorization</span></span>|<span data-ttu-id="65bc5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65bc5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65bc5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="65bc5-124">Accept</span></span>|<span data-ttu-id="65bc5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65bc5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65bc5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65bc5-126">Request body</span></span>
<span data-ttu-id="65bc5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="65bc5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65bc5-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="65bc5-128">Response</span></span>
<span data-ttu-id="65bc5-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="65bc5-129">If successful, this method returns a `200 OK` response code and a collection of [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65bc5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="65bc5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="65bc5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="65bc5-131">Request</span></span>
<span data-ttu-id="65bc5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65bc5-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
```

### <a name="response"></a><span data-ttu-id="65bc5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="65bc5-133">Response</span></span>
<span data-ttu-id="65bc5-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65bc5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 264

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBookCategory",
      "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




