---
title: Получение Манажедебуккатегори
description: Чтение свойств и связей объекта Манажедебуккатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b16a596e2b913fd6e2b69c2fef9d5360611cb05d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972160"
---
# <a name="get-managedebookcategory"></a><span data-ttu-id="8e356-103">Получение Манажедебуккатегори</span><span class="sxs-lookup"><span data-stu-id="8e356-103">Get managedEBookCategory</span></span>

> <span data-ttu-id="8e356-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e356-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e356-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e356-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e356-106">Чтение свойств и связей объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="8e356-106">Read properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e356-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8e356-107">Prerequisites</span></span>
<span data-ttu-id="8e356-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e356-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e356-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e356-110">Permission type</span></span>|<span data-ttu-id="8e356-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e356-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e356-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e356-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e356-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8e356-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8e356-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e356-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e356-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e356-115">Not supported.</span></span>|
|<span data-ttu-id="8e356-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e356-116">Application</span></span>|<span data-ttu-id="8e356-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e356-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e356-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e356-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
GET /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e356-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8e356-119">Optional query parameters</span></span>
<span data-ttu-id="8e356-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8e356-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e356-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e356-121">Request headers</span></span>
|<span data-ttu-id="8e356-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e356-122">Header</span></span>|<span data-ttu-id="8e356-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8e356-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e356-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e356-124">Authorization</span></span>|<span data-ttu-id="8e356-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e356-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e356-126">Accept</span><span class="sxs-lookup"><span data-stu-id="8e356-126">Accept</span></span>|<span data-ttu-id="8e356-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8e356-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e356-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8e356-128">Request body</span></span>
<span data-ttu-id="8e356-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e356-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e356-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e356-130">Response</span></span>
<span data-ttu-id="8e356-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e356-131">If successful, this method returns a `200 OK` response code and [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e356-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8e356-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e356-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e356-133">Request</span></span>
<span data-ttu-id="8e356-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e356-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
```

### <a name="response"></a><span data-ttu-id="8e356-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e356-135">Response</span></span>
<span data-ttu-id="8e356-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e356-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "value": {
    "@odata.type": "#microsoft.graph.managedEBookCategory",
    "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```





